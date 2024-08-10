# PRODIGY_CS_02
Pixel Manipulation for Image Encryption 

Develop a simple image encryption tool using pixel manipulation. Perform operations like swapping pixel values or applying a basic mathematical operation to each pixel and allow users to encrypt and decrypt images.

Library - Here I have used PIL (Python Imaging Library) and NumPy libraries to for image encryption and decryption. It is done through XOR operation between the image array and generated a randomly encryption key. Then decryption is conducted by applying the same XOR operation and the same key.

If you haven't downloaded PIL then write in terminal - 'pip install pillow' 

Working - An image is typically represented as a grid of pixels, where each pixel has a color value. For example, in RGB images, each pixel has three values: Red, Green, and Blue. To manipulate these values, convert the image into a numerical format, such as a NumPy array, where each pixel's color values are stored as integers. A key is a value used for encryption and decryption. For XOR-based encryption, the key is also represented as a numerical value or an array of the same shape as the image array. The key should be kept secret, as it is essential for both encrypting and decrypting the image.

XOR is used as it is simple and reversible

Encrypt image - 
XOR each pixel's color values with the key.
Encrypted Pixel = Original Pixel ⊕ Key
After encryption, convert the numerical array back to an image format and save it.

Decrypt image - 
XOR the encrypted image with the same key used for encryption.
Original Pixel = Encrypted Pixel ⊕ Key
Convert the numerical array back to the image format and save it.
