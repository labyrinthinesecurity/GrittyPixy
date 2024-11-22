# GrittyPixy
A Cloaked QR code prompt injection proof-of-concept

The main idea is to **carve** a QR code out of a special location in an image by modifying existing pixels, NOT by adding the QR code as an overlay.

We leverage the sensitivity of existing QR code readers and stretch them to their detection limit. The samples shown here were all successfully read by the Azure Computer Vision API, despite being hard to eyeball by a human.

In this PoC, we also want to debunk the idea that geometric codes are too small to contain dangerous payloads. We can make QR codes as big as we want, the DAN code shown belows has about 500 characters.

It is not difficult to craft very elaborated prompts and to inject them into QR codes. What is difficult is to make them inconspicuous as we attempt to do here with Gritty Pixy.

<img src="https://github.com/labyrinthinesecurity/GrittyPixy/blob/main/cover.png" alt="Cover Image" width="600">

<img src="https://github.com/labyrinthinesecurity/GrittyPixy/blob/main/prompt.png" alt="DAN 6 prompt" width="600">

## Samples

Take a look at the sample directories where you will see injected images along with their revealed QR code
 
