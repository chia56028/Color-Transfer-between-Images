Color Transfer
===
Color transfer is a practical method to change the appearance of a source image according to the color patternof a target image.<br>
This program is the implementation of the paper [*Color Transfer between Images*](https://www.cs.tau.ac.il/~turkel/imagepapers/ColorTransfer.pdf) by Erik Reinhard, Michael Ashikhmin, Bruce Gooch and Peter Shirley.

## Features
- Read BMP file (source/target image)
- Calculate the mean and STD of each channel
- Implement the RGB color transfer algorithm
    - Convert images from RGB to ℓαβ color space
    - Statistics and color correction

<img src="https://i.imgur.com/2bFZvDi.png" width="400" height="60">

## Install Packages 
```bash
pip install numpy
pip install opencv-python
```
If you want to create `EXE file` after programming, also install this:
```bash
pip install pyinstaller
```

## Run the program
Put 6 source picture and 6 target picture inside the `source_and_target` folder, then execute the code:
```bash
python color_transfer.py
```
After that, your can find 6 result picture inside `result` folder.

Execute following instruction to create `EXE file` of this program:
```bash
pyinstaller -F color_transfer.py
```

### Example
Source / Target / Result

<p float="left">
    <img src="https://i.imgur.com/UqbFy34.jpg" width="250" height="170">
    <img src="https://i.imgur.com/piirZXC.png" width="250" height="170">
    <img src="https://i.imgur.com/zEb47kZ.jpg" width="250" height="170">
</p>
<br>
<p float="left">
	<img src="https://i.imgur.com/M1zPrJq.jpg" width="250" height="170">
	<img src="https://i.imgur.com/O62ubGC.jpg" width="250" height="170">
	<img src="https://i.imgur.com/XuzTKdf.jpg" width="250" height="170">
</p>

## References
- [Color Transfer between Images](https://www.cs.tau.ac.il/~turkel/imagepapers/ColorTransfer.pdf)
- [python opencv 实现Reinhard颜色迁移算法](https://www.cnblogs.com/likethanlove/p/6003677.html)
- [Content-Based Color Transfer](http://www.cs.albany.edu/~xmei/resource/pdf/color.pdf)