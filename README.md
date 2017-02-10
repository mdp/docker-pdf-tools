# pdf-tools

Runs in Docker so you don't have to worry about all the dependencies:

- ImageMagick
- Ghostscript
- Ghostscript-Fonts
- PDFTk

## Usage

### Shrink

Shrink PDF's by compressing images to a reasonable resolution

`docker run -v "$(pwd)":/data --rm -it mpercival/pdf-tools shrink big.pdf small.pdf`

### Watermark

Watermarks a multipage PDF file

`docker run -v "$(pwd)":/data --rm -it mpercival/pdfkit watermark "Top Secret" secret.pdf  secret_watermark.pdf`
