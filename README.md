# mikechester.ca

Source for [mikechester.ca](https://mikechester.ca). The whole site is the `static/` directory:
`index.html`, `style.css` and images. There is no build step.

Pushing to `build` runs `.github/workflows/main.yml`, which publishes `static/` to `main`. GitHub
Pages serves `main`. Don't edit `main` directly: each deploy replaces it.

The page is dark by default. A small script in `index.html` adds a toggle to switch to light and
remembers the choice; without JavaScript the page stays dark.

To preview locally:

```sh
python3 -m http.server -d static
```
