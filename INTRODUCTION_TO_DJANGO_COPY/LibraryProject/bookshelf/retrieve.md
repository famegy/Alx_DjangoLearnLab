# retrieve and display all books in the database

## python command use:

```python
from bookshelf.models import Book

books = Book.objects.get(title="1984")
books.title
books.author    
books.publication_year

```

## expected output:

```python
'1984'
'George Orwell'
1949
```

