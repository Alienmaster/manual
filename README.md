# Manual

The Uberspace 7 manual aims to provide reference documentation
on how to operate an uberspace on U7. Pushing to this repositorys
stable branch publishes the content to https://manual.uberspace.de.
Pushing to any other branch publishes the content to https://branchname.manual.corona.uberspace.de.

## Development

Pushing for each and every change is fun, but can take some
time. To speed up your development process, the manual can
be built locally.

### Initial Setup

```
$ virtualenv venv --python=python2.7
$ source venv/bin/activate
$ pip install -r requirements.txt
```

### Building

```
$ source venv/bin/activate
$ make html
```

The HTML views are now present in `build/html`. To build automatically
on each change execute use `sphinx-autobuild`:

```
$ make serve
```

This will start a local webserver on http://127.0.0.1:8000, which
always serves the most recent version.
