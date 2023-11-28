To convert a presentation to PDF, use [decktape](https://github.com/astefanutti/decktape), which is best executed with Docker:

```bash
docker run --rm -t --net=host -v `pwd`:/slides astefanutti/decktape http://localhost:4200/slides-public/2023-12-10-agu.html _pdf/slides.pdf
```
