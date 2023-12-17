# My Poster

## Software

To setup, clone then:

```bash
git submodule init
quarto add quarto-ext/fontawesome
```

## Printing

```bash
docker run --rm -t --net=host -v `pwd`:/slides astefanutti/decktape http://host.docker.internal:4200 slides.pdf
```

## Figures

RevealJS doesn't like figures that are in PDF format.
We can use `imagemagick` to convert:

```bash
convert input.pdf output.svg
# or
convert -density 300 -quality 100 input.pdf output.jpg
```
