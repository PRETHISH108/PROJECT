# Image-Based Message Encryption and Decryption

## Overview
This project allows you to hide a secret message inside an image and retrieve it later using a passcode. The message is embedded in the pixel values of the image and can only be decrypted using the correct passcode.

## Requirements
- Python 3.x
- OpenCV (`cv2`)

## Installation
1. Install Python from [python.org](https://www.python.org/downloads/)
2. Install OpenCV using pip:
   ```sh
   pip install opencv-python
   ```

## Usage
### Encryption
1. Place an image (`img.jpg`) in the specified path (`C:/Users/HP/OneDrive/Desktop/PROJECT/`)
2. Run the script:
   ```sh
   python script.py
   ```
3. Enter your secret message when prompted.
4. Enter a passcode for encryption.
5. The encrypted image will be saved as `encryptedImage.jpg` and automatically opened.

### Decryption
1. Run the script again.
2. Enter the passcode used during encryption.
3. If the passcode is correct, the hidden message will be displayed.
4. If incorrect, access is denied.

## Code Explanation
- The script reads an image using OpenCV.
- It converts each character of the secret message into ASCII values and embeds them into the pixel values of the image.
- During decryption, the pixel values are read and converted back to characters.
- A passcode is used to prevent unauthorized decryption.

## Notes
- This method modifies the image, so repeated encryptions may degrade its quality.
- The message length should be small enough to fit in the image pixels.
- The encoding method used is simple and not secure for highly sensitive data.

## Disclaimer
This project is for educational purposes only. Do not use it for encrypting sensitive information.

## Author
Prethish D

