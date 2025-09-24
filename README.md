# photo-pro-suite

Suite aberta para fluxo de trabalho de fotos com GIMP, Darktable, RawTherapee, Inkscape, digiKam, ImageMagick e ExifTool, com automação via workflows.

## Objetivos
- Centralizar presets, plugins, scripts e documentação de ferramentas FOSS para fotografia.
- Padronizar workflows (pré-processamento RAW → aprimoramento → exportação final).
- Facilitar automação por linha de comando.

## Ferramentas incluídas
- GIMP: https://github.com/GNOME/gimp
- G'MIC: https://github.com/dtschump/gmic
- Resynthesizer: https://github.com/bootchk/resynthesizer
- Darktable: https://github.com/darktable-org/darktable
- RawTherapee: https://github.com/Beep6581/RawTherapee
- Inkscape: https://github.com/inkscape/inkscape
- digiKam: https://github.com/KDE/digikam
- ImageMagick: https://github.com/ImageMagick/ImageMagick
- ExifTool: https://exiftool.org/

Consulte os READMEs em cada subpasta para instruções específicas e links oficiais.

## Estrutura
```
photo-pro-suite/
├─ gimp/
├─ darktable/
├─ rawtherapee/
├─ inkscape/
├─ digikam/
├─ imagemagick/
├─ exiftool/
├─ workflows/
└─ docs/
```

## Requisitos
- Linux (testado em Ubuntu/Zorin)
- git e GitHub CLI (gh) opcionais para publicar no GitHub
- Ferramentas conforme seu uso: gimp, darktable, rawtherapee, inkscape, digikam, imagemagick, exiftool

## Instalação rápida (Ubuntu/Zorin)
Exemplos (verifique os READMEs por ferramenta):
- GIMP: `sudo apt install gimp`
- Darktable: `sudo apt install darktable`
- RawTherapee: `sudo apt install rawtherapee`
- Inkscape: `sudo apt install inkscape`
- digiKam: `sudo apt install digikam`
- ImageMagick: `sudo apt install imagemagick`
- ExifTool: `sudo apt install libimage-exiftool-perl`

## Workflows
Veja `workflows/edit-photos.yml` para um fluxo de exemplo:
- process_raw (RawTherapee)
- enhance_images (G'MIC)
- final_resize (ImageMagick)

Exemplo de execução conceitual:
```
warp run workflows/edit-photos.yml
```
A execução efetiva depende de você adaptar os caminhos/variáveis e ter as ferramentas instaladas no sistema.

## Contribuindo
- Abra issues e PRs descrevendo mudanças.
- Evite commitar arquivos binários pesados (veja .gitignore).

## Licença
MIT — veja o arquivo LICENSE.
