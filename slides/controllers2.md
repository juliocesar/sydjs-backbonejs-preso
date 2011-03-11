    var Controller = Backbone.Controller.extend({
      routes: {
        '!/'        : 'root',   // localhost/#!/
        '!/books'   : 'books'   // localhost/#!/books
      },
  
      root: function() {
        // stuff that happens on the home page
      },
  
      books: function() {
        // books list
      },
      ...
    });