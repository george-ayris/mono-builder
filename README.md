Build [Mono runtime](http://www.mono-project.com/Main_Page) for use with the [Heroku .NET buildpack](https://github.com/friism/heroku-buildpack-mono).

To build:

```term
$ docker build -t george-ayris/mono-builder cedar-14/.
```

To build and upload new Mono version:

```term
$ docker run -v ${PWD}/cache:/var/cache -e VERSION=4.2.2.30 -e STACK=cedar-14 george-ayris/mono-builder
```
