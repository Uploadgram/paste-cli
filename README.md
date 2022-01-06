# pastegram-cli

A CLI tool to use Pastegram from the terminal

## Installing

```bash
sudo pip install pastegram-cli # install globally
```

## Examples

### Uploading

```bash
pastegram-cli upload my-file.txt
```

or read from STDIN

```bash
# implicit upload
pastegram-cli < my-file.txt
```

or

```bash
cat my-file.txt | pastegram-cli
```

### Fetching a paste

```bash
pastegram-cli fetch "https://paste.uploadgram.me/61d7737a9ae36g#AmX76Y3RDgh_xfHB2ktgVYcT76jjCXMmMs7xPYSbqoc"
# outputs to STDOUT
```

or write the output to a file

```bash
pastegram-cli fetch "https://paste.uploadgram.me/61d7737a9ae36g#AmX76Y3RDgh_xfHB2ktgVYcT76jjCXMmMs7xPYSbqoc" -o the-paste.txt
```

### Deleting a paste

```bash
pastegram-cli delete TOKEN
# TOKEN is the 49 characters long string you get after uploading a paste
```
