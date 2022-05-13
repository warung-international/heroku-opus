# heroku-opus

[![Test](https://github.com/warung-international/heroku-opus/workflows/Test/badge.svg?branch=master&event=push)](https://github.com/warung-international/heroku-opus/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster)  

> This is a fork of the [original repository](https://github.com/xrisk/heroku-opus). All thanks to the past contributors.

Installs the opus codec for usage with heroku apps. 

## Usage

Run the following from the heroku command line:

```
heroku buildpacks:add --index 1 https://github.com/warung-international/heroku-opus.git
```

Note: This buildpack should be added before the main language buildpack (by using --index 1), since the application process types are calculated from the last buildpack in the list if no Procfile is specified.