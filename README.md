<div align="center">

# 🧂 My Favorite Ingredient — CTF Writeup

[![GPNCTF 2026](https://img.shields.io/badge/CTF-GPNCTF%202026-teal?style=for-the-badge)](https://gpn24.ctf.kitctf.de/)
[![Category: Reversing](https://img.shields.io/badge/Category-Reversing-purple?style=for-the-badge)](#)
[![Points: 79](https://img.shields.io/badge/Points-79-gold?style=for-the-badge)](#)

*How to make a binary confess its own secret transform — without reading a single line of assembly.*

</div>

<br/>

## 📖 Read the Writeup

Experience the full interactive writeup, complete with dynamic matrix demonstrations and sleek animations, right in your browser:

👉 **[Read the Full Writeup Online](https://AdvayBagaria.github.io/My_Favourite_Ingredient/)**

*(For local viewing, simply clone this repository and open `index.html` in any modern web browser.)*

## 🎯 Challenge Overview

This writeup details a complete black-box dynamic analysis approach to solving the **My Favorite Ingredient** reverse-engineering challenge. 

Instead of painstakingly reversing the assembly instructions, we take advantage of the transformation's **linearity**. By probing the binary exactly 65 times with carefully chosen inputs via GDB, we isolate and recover the hidden 64×64 transformation matrix. From there, we solve for the exact flag instantly using Gaussian elimination (Modulo 256 matrix inversion).

## 👨‍💻 Authors

- **Writeup Author:** optimus_prime (Team e0_) | Hosted by [Advay Bagaria](https://github.com/AdvayBagaria)
- **Challenge Creator:** intrigus (GPNCTF 2026)

---
*If you enjoyed this writeup, consider dropping a ⭐ on the repository!*
