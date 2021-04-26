# heic-jpg-linux

How to convert Apple iPhone's .HEIC images to .jpg via Linux Terminal:

```
for file in *.HEIC; do heif-convert $file ${file/%.HEIC/.jpg}; done
```

Sources:
- https://askubuntu.com/questions/958355/any-app-on-ubuntu-to-open-and-or-convert-heif-pictures-heic-high-efficiency-i
- https://gist.github.com/bittercoder/f6601784ebe4f63e9b9e037e3344b960
