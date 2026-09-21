# Day 5 — File Viewing & Log Reading

## Commands Practiced

```bash
echo "Hello" > test.txt               # Create/overwrite file
echo "Hi" >> test.txt                 # Append text

cat app.log                           # Display file content
cat -n app.log                        # Show line numbers
cat file1.txt file2.txt               # Display multiple files

less app.log                          # Read large file page by page

head app.log                          # First 10 lines
head -n 3 app.log                     # First 3 lines

tail app.log                          # Last 10 lines
tail -n 2 app.log                     # Last 2 lines
tail -f app.log                       # Live log monitoring

grep "Error" app.log                  # Search exact word
grep -i "error" app.log               # Ignore case
grep -n "Error" app.log               # Show line numbers
grep -v "Error" app.log               # Exclude matches
grep -c "Error" app.log               # Count matches
grep -w "Error" app.log               # Match whole word
grep -r "Error" ~/devops-lab          # Search recursively
grep -e "Error" -e "Warning" app.log  # Multiple patterns
```

## Options Learned

- `>` → Overwrite / create file
- `>>` → Append text
- `-n` → Line numbers
- `-f` → Follow live logs
- `-i` → Ignore case
- `-v` → Invert match
- `-c` → Count matches
- `-w` → Whole word
- `-r` → Recursive search
- `-e` → Multiple search patterns

**Status:** ✅ Day 5 Completed
