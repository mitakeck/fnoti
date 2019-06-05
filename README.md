# fnoti
fnoti: simple command line tool for detect file change


## Usage

```bash
$ fnoti [watch_file_path]
...
print updated file name(path)
...
```

```bash
$ fnoti ./**/*.md
/hoge/foo.md
/hoge/bar.md
...
```

```bash
# cat update file content
$ fnoti ./**/*.md | xargs cat
```

```bash
# convert Markdown to HTML
$ fnoti ./**/*.md | xargs -I@ pandoc @ @.html
```