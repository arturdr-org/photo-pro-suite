# ExifTool

Site oficial: https://exiftool.org/

Instalação (Ubuntu/Zorin):
```
sudo apt update
sudo apt install libimage-exiftool-perl
```

Exemplos:
- Ver metadados:
```
exiftool foto.jpg
```
- Alterar autor em lote:
```
exiftool -overwrite_original -Artist="Seu Nome" ./enhanced/jpg/*.jpg
```
- Copiar data de criação para saída final:
```
exiftool -overwrite_original -tagsFromFile ./raw/%f.CR2 -DateTimeOriginal ./final/ml-ready/*.jpg
```
