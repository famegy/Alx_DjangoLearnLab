# CRUD Operations in Django Shell

## 1️⃣ CREATE

```python
from bookshelf.models import Book

book = Book.objects.create(
    title="1984",
    author="George Orwell",
    publication_year=1949
)

book
```

Output:
```
<Book: 1984>
```

The book instance was successfully created and saved to the database.

---

## 2️⃣ RETRIEVE

```python
Book.objects.all()
```

Output:
```
<QuerySet [<Book: 1984>]>
```

The book record was successfully retrieved.

---

## 3️⃣ UPDATE

```python
book = Book.objects.get(title="1984")
book.title = "Nineteen Eighty-Four"
book.save()

book
```

Output:
```
<Book: Nineteen Eighty-Four>
```

The book title was successfully updated.

---

## 4️⃣ DELETE

```python
book.delete()

Book.objects.all()
```

Output:
```
<QuerySet []>
```

The book was successfully deleted and no records remain in the database.
