# Day 3 – File Copy (`cp`)

## Project Structure

```text
Linux-Journey/
└── devops/
    ├── file1.txt
    ├── linux/
    │   ├── file1.txt
    │   └── app.txt
    └── backup/
        └── file1.txt
```

## Commands Practiced

```bash
cp devops/file1.txt linux/              # Copy file to another directory

cp file1.txt linux/app.txt       # Copy and rename at the same time

cp -v file1.txt linux/           # Verbose output

cp -i file1.txt linux/           # Ask before overwrite

cp -r linux backup/              # Copy directory recursively
```

## Options Learned

- `-v` → Show what `cp` is doing
- `-i` → Ask permission before overwrite
- `-r` → Copy directories recursively

**Status:** ✅ Day 3 Completed
