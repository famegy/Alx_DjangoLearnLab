# Create a Book instance
## python command use:

```python

from bookshelf.models import Book

book = Book.objects.create(
    title="1984",
    author="George Orwell",
    publication_year=1949
)

```

## epected output:

```python
<Book: Book object (1)>

```