# My Books Catalog
An catalog to keep my library organized and register my reading desires.

# The Problem
An website that store books data, making it easy to search through them and organize. It can be shown as cards with the infos. The search can look for titles and authors. Order by read/not read, number of pages ascending/descending and alphabetical (asc/desc) per author or per title. You can search only your favorited books. Display profile statistics like books and pages read.</br>
Bonus: a tag system for genre so the user can filter its search.</br>
Future: make a cloud and local save system so people can really use it. And add a Wishlist Category so you can add books you dont own but want to buy one day (add a button on wishlisted book that redirects to google shopping for that book with google.com/search?q=BOOK_NAME_HERE&tbm=shop)

# Organizing Ideas
- catalog is an Array of book objects.
- display is an Array that stores the current filter/search results. default is same as catalog. (store just reference, prob Index)
- Book info: title, author first name, author last name, number of pages, pages read, is_read bool, is_fav bool and genre array.
- Will need a forms that adds books to catalog. (on_submit)
- AddBook: create new book object and add as catalog array.
- everytime a book is added, deleted or edited, Update Stats.
- Search Form: search input for string, ordering menu,(genre filter), read filter, fav filter, submit button.
- Searching: go through every catalog object checking if it matches curent search settings.
- Filter object that stores all search info and its search function that returns an array of objects.
CARDS
- DeleteBook: get book index and delete from catalog array.
- a button on cards to mark is_read true or not
- Fav button to mark as is_fav
- an edit button on cards which call a forms that you can update anything, mainly used to update pages read and if you wrote something wrong.