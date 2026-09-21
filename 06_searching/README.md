# Copy a book
curl -o linux_book.txt https://www.gutenberg.org/cache/epub/6527/pg6527.txt
# less 
less linux_book.txt
# find words in book
grep open linu_book.txt
# find word count -lines
grep -in ^the linux_book.txt | wc -l
# multiple greps
grep -i linux linux_book.txt | grep partition | wc -l 
