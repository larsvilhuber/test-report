# test-report

This will demonstrate a simple RMarkdown report

To run with Docker do this:

```
cd where/you/cloned/test-report
docker run -it --rm \
   -v $(pwd):/code \
   -w /code \
   larsvilhuber/rmarkdown:v2021-08-19 \
   R -e rmarkdown::render('index.Rmd')
```

If on Windows, use the Command Prompt:
```
cd where\you\cloned\test-report
docker run -it --rm ^
  -v %cd%:/code ^
  -w /code ^
  larsvilhuber/rmarkdown:v2021-08-19 ^
   R -e rmarkdown::render('index.Rmd')
```
