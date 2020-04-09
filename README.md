# Questions

## 1.How would we filter for all books with titles containing the word ‘Django’?
Book.objects.filter(title='Django')

## 2.How would we filter for all books with tag ‘Fiction’?
Book.objects.filter(tags='Fiction')

## 3.How would we filter for all authors who have written books containing the word ‘Django’? HINT: We can use the book field to refer to an author’s books, even though the Author model doesn’t explicitly contain it!
Author.objects.filter(Books.title='Django')

