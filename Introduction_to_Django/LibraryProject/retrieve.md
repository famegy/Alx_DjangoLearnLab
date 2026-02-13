# retrieve and display all books in the database

## python command use:

```python
from bookshelf.models import Book

books = Book.objects.all()
    for book in books:

```

## expected output:

```python
    <QuerySet [<Book: 1984>]>
```

