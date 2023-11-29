# Conversion

To convert a presentation to PDF, use [decktape](https://github.com/astefanutti/decktape), which is best executed with Docker:

```bash
docker run --rm -t --net=host -v `pwd`:/slides astefanutti/decktape http://host.docker.internal:4200/ slides.pdf
```

or

```bash
docker run --rm -t -v `pwd`:/slides astefanutti/decktape https://jdossgollin.github.io/presentation-2023-agu/ slides2.pdf
```

or

```bash
docker run --rm -t  --volume="$(PWD):/slides" astefanutti/decktape /slides/_site/index.html slides2.pdf
```

or

```bash
docker run --rm -t  --volume="$(PWD):/slides" astefanutti/decktape /slides/_site/index.html slides2.pdf --screnshots-size=1400x788
```

```bash
docker run --rm -t -v `pwd`:/slides -v ~:/home/user astefanutti/decktape /home/user/index.html slides2.pdf
```
