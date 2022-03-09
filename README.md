# heic-jpg-convert-linux

How to convert Apple iPhone's .HEIC images to .jpg via Linux Terminal.

These commands can be used in Ubuntu versions >= 18.04.

Open a terminal and paste this command:
```
sudo apt install libheif-examples
```

Open the folder containing the .HEIC images in the terminal (e.g. navigate there by using `cd` and `ls`). Then use the following command:
```
for file in *.HEIC; do heif-convert $file ${file/%.HEIC/.jpg}; done
```

Sources:
- https://askubuntu.com/questions/958355/any-app-on-ubuntu-to-open-and-or-convert-heif-pictures-heic-high-efficiency-i
- https://gist.github.com/bittercoder/f6601784ebe4f63e9b9e037e3344b960
