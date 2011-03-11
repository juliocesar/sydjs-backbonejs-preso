# Re: State Machine

See what I did there?

    initialize: function() {
      this.model.bind('remove', this.remove);
      this.model.view = this;
    }

Removing the model removes the view (or table row, in this example).

Assigning the view to the model so we can easily reference it.

Screw separation. This stuff should be easy, not "proper".