# Command line options

emadLoppo has some command line options.

## --dir, -d

`--dir` or `-d` sets the document directory which keeps the original Markdown files. `docs` is the default directory.

```bash
$ emad-loppo --dir my_docs
```

## --output, -o

`--output` or `-o` sets the output directory which keeps the generated documents. `dist` is the default directory.

```bash
$ emad-loppo --output my_site
```

##  --site, -s

`--site` or `-s` sets the site's name. `Documents` is the default.

```bash
$ emad-loppo --site "My Documents"
```

## --theme, -t

`--theme` or `-t` sets a site's theme. `emad-loppo-theme-oceandeep` is the default.

```bash
$ emad-loppo --theme oceandeep
```

##  --id

`--id` sets a site's ID (default is the dir name of the project).

## --direction

`--direction` sets the document's character direction. `ltr` is the default. It also could be setted as `rtl`.

The option needs the support of the site theme.

## --debug

`--debug` opens emadLoppo's debug mode.

##  --version, -v

`--version` or `-v` shows emadLoppo's version information.

## --help

`--help` gives emadLoppo's commandline usage.





示例：
  emad-loppo --dir docs --output dist
