# Sub-commands

Loppo supports two git-style subcommands.

- emad-loppo server
- emad-loppo count
- emad-loppo chapter

## emad-loppo server

`emad-loppo server` builds the document site at first, and thereafter launch a web server on 8080 port for `dist` sub-directory.

```bash
$ emad-loppo server
```

After running the comand, you could visit http://127.0.0.1:8080 in your browser.

This command is helpful for preview when you develop your documents.

## emad-loppo count

`emad-loppo count` will output statistic information of your documents.

```bash
$ emad-loppo count

[Files] 56
[Lines] 8885
[Words] 51555
[Chars] 362931
```

Attention, before using this command, `chapters.yml` must already be existed. Otherwise you will get an error.

`emad-loppo count` has two options.

```bash
# output every markdown file's statistic information
$ emad-loppo count --detail

# output a specified markdown file's statistic information
# the file path should be same as the corresponding item in chapters.yml
$ emad-loppo count -f some.md
```

## emad-loppo chapter

`emad-loppo chapter` will re-create `chapters.yml` and add new Markdown files into it.

Attention, the old `chapters.yml` will be deleted after running the command.

```bash
$ emad-loppo chapter

This command will delete your chapters.yml if existed.
Are you sure to continue? （Y/N）
```

If you want to skip the confirmation, use `--force` option.

```bash
$ emad-loppo chapter --force
```
