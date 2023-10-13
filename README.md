# ASCII-pictures
Convert pictures to ASCII graphics (character pictures)

When you press enter, the explorer opens with the possibility to select a photo with the extension *.bmp; *.png; *.jpg; *.JPEG.
Conversion algorithm:
-Any picture undergoes normalization (compression) to the specified dimensions in the MAX_WIDTH constant. When calculating the height, it is worth considering that the size of the console cell for the symbol is not proportional (the height is 2 times the width), this is compensated by the constant WIDTH_OFFSET.
-Further, the picture is converted to black and white format ((pixel.R + pixel.G + pixel.B) / 3).
-Walking through each grayscale pixel (from 0 to 255), we calculate a character from the array ( '.', ',', ':', '+', '*', '?', '%', 'S', '#', '@' ), where the characters are arranged by brightness. That is, the lightest pixel will take '.' and the darkest pixel will take '@'.
-Displaying characters on the screen
-The inverse array ( '.', ',', ':', '+', '*', '?', '%', 'S', '#', '@') is used for saving, since in a text document the background is white and the characters are black, unlike in the console.

### Settings-for-best-results

![img](https://github.com/Gooooosha/ASCII-pictures/blob/main/img_for_readme/4.png)

### Test-picture

![img](https://github.com/Gooooosha/ASCII-pictures/blob/main/img_for_readme/leo.jpeg)

### Conversion-result

![img](https://github.com/Gooooosha/ASCII-pictures/blob/main/img_for_readme/1.png)

### You-can-see-that-the-picture-is-made-up-of-characters

![img](https://github.com/Gooooosha/ASCII-pictures/blob/main/img_for_readme/2.png)

### Test-picture

![img](https://github.com/Gooooosha/ASCII-pictures/blob/main/img_for_readme/cat.jpeg)

### Conversion-result

![img](https://github.com/Gooooosha/ASCII-pictures/blob/main/img_for_readme/3.png)

### Saving-to-a-text-file

![img](https://github.com/Gooooosha/ASCII-pictures/blob/main/img_for_readme/5.png)
