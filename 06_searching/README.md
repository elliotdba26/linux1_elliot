```bash
# Download a book
curl -o linux_book.txt https://www.gutenberg.org/cache/epub/6527/pg6527.txt

# View the book
less linux_book.txt

# Find lines containing a word
grep open linux_book.txt

# Count lines that start with "the" (case-insensitive)
grep -in ^the linux_book.txt | wc -l

# Count lines that contain both "linux" and "partition" (case-insensitive)
grep -i linux linux_book.txt | grep partition | wc -l
```
