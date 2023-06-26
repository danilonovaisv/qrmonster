---
tags:
- stable-diffusion
- controlnet
- qrcode
license: openrail++
language:
- en
---

# Controlnet QR Code Monster v1 For SD-1.5

![QR code in shape of a tree, reading "https://huggingface.co/monster-labs"](images/tree.png)

##  Model Description

This model is made to generate creative QR codes that still scan.
Keep in mind that not all generated codes might be readable, but you can try different parameters and prompts to get the desired results.

You can try it in a space [Try it here!](https://huggingface.co/spaces/monster-labs/Controlnet-QRCode-Monster-V1) or use it localy.

We're already working on v2, which is much more powerful, you can try [an early version here](https://qrcodemonster.art) ! OR just scan the monster below !
![QR code in shape of a blue monster, reading "https://qrcodemonster.art"](images/monster.png)

## How to use

- **Condition**: QR codes are passed as condition images with a module size of 16px. Use a higher error correction level to make it easier to read (sometimes a lower level can be easier to read if smaller in size).

- **Prompts**: Use a prompt to guide the QR code generation. The output will highly depend on the given prompt. Some seem to be really easily accepted by the qr code process, some will require careful tweaking to get good results.

- **Controlnet guidance scale**: Set the controlnet guidance scale value:
   - High values: The generated QR code will be more readable.
   - Low values: The generated QR code will be more creative.

### Tips

- You might need to generate multiple QR codes with the same parameters to get a readable output (our new model greatly improves this).

- Use the Image-to-Image feature to improve the readability of a QR code:
  - Decrease the denoising strength to retain more of the original image.
  - Increase the controlnet guidance scale value for better readability.
  A typical workflow for "saving" a code would be :
  Max out the guidance scale and minimize the denoising strength, then bump the strength until the code scans.

## Example outputs

Here are some examples of creative and readable QR codes generated using this model:

![A gothic sculpture in shape of a QR code, reading "test"](images/skull_test.png)
![City ruins with a building facade in shape of a QR code, reading "sd is cool"](images/architecture.png)

Feel free to experiment with prompts, parameters, and the Image-to-Image feature to achieve the desired QR code output. Good luck and have fun!