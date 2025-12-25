class Library:
    def __init__(self):
        self.books = []

    def add_book(self, book):
        self.books.append(book)
        print("Book added")

    def remove_book(self, book):
        if book in self.books:
            self.books.remove(book)
            print("Book removed")
        else:
            print("Book not found")

    def display_books(self):
        print("Available Books:")
        for book in self.books:
            print(book)

lib = Library()
lib.add_book("Python Basics")
lib.add_book("Java Programming")
lib.display_books()
