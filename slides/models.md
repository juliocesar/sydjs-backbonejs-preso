    var Book = Backbone.Model.extend({
      initialize: function() {
        this.set({'title': 'a default title'});
      },
      give: function(user) {
        // gives book to a user
      },
      sell: function(user) {
        // sell a book to a user
      },
      clear: function() {
        this.destroy();     // #destroy is provided by Backbone.js
        this.view.remove(); // will explain in a few slides
      }
    });