# Delete the book you created and confirm the deletion by trying to retrieve all books again.

## python command use:

```python
from bookshelf.models import Book
book = Book.objects.get(title="Nineteen Eighty-Four")
book.delete()
books = Book.objects.all()
```
## expected output:

```python 
<QuerySet []>
```