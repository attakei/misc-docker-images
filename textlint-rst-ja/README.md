# attakei/textlint-rst-ja

Docker image to run textlint for reStructuredText.

## Use case

* Check syntax of your blog sources based from Sphinx (ex: pelican, tinkerer)

## Usage

### Shorthand

Example: to use pelican project

```
$ cd /path/to/myproject
$ docker run -it --rm -v `pwd`/content:/app/content attakei/textlint-rst-ja
```
