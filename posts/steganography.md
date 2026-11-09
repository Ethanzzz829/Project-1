---
title: "Hidden in Plain Sight: Hiding Text Inside a PNG Image"
tags: [steganography, PNG, least significant bit, data hiding, cybersecurity]
---

## Introduction

When someone opens a picture on their computer, they usually only think about what the picture shows. However, an image can also contain a hidden message that is not obvious just from looking at it. My blog topic is steganography, which is the practice of hiding information inside something else. For this project, I will focus on hiding a text message inside a PNG image using least significant bit, or LSB, steganography. I want to explore how this works through a small experiment and explain the results in a way that someone new to the topic can understand.

Digital images contain pixels, and those pixels use numbers to represent colors. With LSB steganography, a tool changes the lowest-value bits of some of those numbers to store a message. These changes can be small enough that the image still looks the same to a person viewing it. PNG is useful for this investigation because it uses lossless compression, which preserves the image's pixel values when it is saved without other changes. However, preserving the picture's appearance does not necessarily mean the file will have the same size.

This topic matters because the visible contents of a file do not always tell the whole story. Learning about hidden information can help people understand why cybersecurity involves examining data beyond what appears on the screen. It also shows an important difference between hiding information and encrypting it. Encryption protects the meaning of a message, while steganography tries to hide the fact that the message exists. A hidden message is not automatically encrypted or protected from someone who knows how to extract it. The Stegano documentation makes this distinction clear when explaining its message-hiding tools.

The main question my blog will answer is: How can a text message be hidden inside a PNG image, and how does hiding it affect the image's appearance and file size? To investigate, I plan to keep an unchanged original image and create copies containing messages of different lengths. I will compare their appearance and file sizes, then try to recover each message to check whether it matches the original text. I will also capture screenshots of the process and record my observations. These comparisons will help me explain what changed, what stayed visually similar, and why appearance alone cannot prove that a file contains no hidden information.

## References

1. Kaspersky. "What is steganography? Definition and explanation."
   https://www.kaspersky.com/resource-center/definitions/what-is-steganography

2. World Wide Web Consortium (W3C). "Portable Network Graphics (PNG) Specification (Third Edition)."
   https://www.w3.org/TR/png/

3. Stegano. "Presentation."
   https://stegano.readthedocs.io/en/latest/
