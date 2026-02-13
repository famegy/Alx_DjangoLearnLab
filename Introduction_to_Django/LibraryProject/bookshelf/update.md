# Update the title of “1984” to “Nineteen Eighty-Four” and save the changes.

## python command use:

```python
from bookshelf.models import Book

book = Book.objects.get(title="1984")
book.title = "Nineteen Eighty-Four"
book.save()
```

## expected output:

```python 
'Nineteen Eighty-Four'
'George Orwell'
1949
```