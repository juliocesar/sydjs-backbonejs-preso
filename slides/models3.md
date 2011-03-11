Now we can go

    var book = Books.create();
    book.set({'title', 'changed'});
    book.save();
    
That will "commit" the new book to the server via Ajax.