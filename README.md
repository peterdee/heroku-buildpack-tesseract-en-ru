## Heroku Buildpack Tesseract EN-RU

This package provides a custom Heroku buildpack providing the [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) binary **(4.0)** and all the required libraries to Heroku apps. Training data for **English** and **Russian** languages included.

This version is a modification of https://github.com/pathwaysmedical/heroku-buildpack-tesseract with Russian language support. 

### Configuration

The first step consists in allowing your Heroku app to use multiple buildpacks. Heroku natively supports [multiple buildpacks per app](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app).

1. Setup your app:
```shell script
heroku buildpacks:set heroku/LANG
heroku buildpacks:add https://github.com/peterdee/heroku-buildpack-tesseract-en-ru
```

`LANG` is the language used by your app (e.g., `ruby`, `python`, or `nodejs`).

A complete list of Heroku buildpacks can be found [here](https://devcenter.heroku.com/articles/buildpacks).

 2. You can use the `tesseract` binary in your Heroku app!

 3. Deploy!

### License
MIT License.
