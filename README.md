# Benjamin Meißner CV
Find live version via https://cv.masonen.de

## Run Docker

```bash
docker build Docker/. -t masonen-cv
docker run -v $(pwd):/data/ -p 4000:4000 masonen-cv serve --theme kendall
```