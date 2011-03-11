    var BookView = Backbone.View.extend({
      tagName : 'tr',
      events  : {
        'click input[type="checkbox"]'  : 'toggleSelect'
      },
      template  : _.template($('#book-table-template').html()),
      initialize: function() {
        this.model.bind('remove', this.remove);
        this.model.view = this;
      },
      render: function() {
        $(this.el).html(this.template(this.model.toJSON()));
      },
      toggleSelect: function() {
        var total = Books.selected().length;
        $('#books-selected').html('Selected: ' + total);
      }
    });