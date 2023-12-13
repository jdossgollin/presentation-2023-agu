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
