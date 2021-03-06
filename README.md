# Heroku buildpack: Meteorite

This build pack allows you to easily deploy meteor apps to heroku using [meteorite](http://github.com/oortcloud/meteorite). It's easy to use different branches of meteor and any smart package you can lay your hands on.

_Coming soon_: Support for packages that rely on node modules, more goodies

## Usage

```bash
heroku create --stack cedar --buildpack https://github.com/oortcloud/heroku-buildpack-meteorite.git
```

Then `git push` to heroku as usual. 

## NOTES

1. You need to set the `ROOT_URL` environment variable:

```bash
heroku config:add ROOT_URL=your.domain.com
```

3. You need to have a verified account so the buildpack can add a `mongohq:sandbox` addon.
