    var BookCollection = Backbone.Collection.extend({
      model : Book,
      url   : '/books',
      cheap : function() {
        return this.filter(function(book) { 
          return book.get('price') < 10.0; 
        });
      }
    });
    
    var Books = new BookCollection;