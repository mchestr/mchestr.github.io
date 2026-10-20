# mikechester.ca

Source for [mikechester.ca](https://mikechester.ca). The whole site is the `static/` directory:
`index.html` and `style.css`, plus images and `resume.pdf`. There is no build step.

Pushing to `build` runs `.github/workflows/main.yml`, which publishes `static/` to `master`. GitHub
Pages serves `master`. Don't edit `master` directly: each deploy replaces it.

`static/resume.pdf` is updated automatically by the resume repository, which pushes to `build`.

To preview locally:

```sh
python3 -m http.server -d static
```
