# ImageMagick

Repositório oficial: https://github.com/ImageMagick/ImageMagick

Instalação (Ubuntu/Zorin):
```
sudo apt update
sudo apt install imagemagick
```

Exemplos úteis:
- Redimensionar em lote mantendo qualidade:
```
magick mogrify -path ./out -strip -resize 2048x2048 -quality 88 ./in/*.jpg
```
- Converter para TIFF:
```
magick convert input.jpg -compress lzw output.tif
```
