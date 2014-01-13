What's this?
============

This is an advanced Liquid template for Jekyll's pagination. I made it for my [website](http://moroccanrubyist.com/)
and I think it can be useful for others.

![Jekyll Paginator Links](http://i.imgur.com/u9hec6c.png)

How can I use it?
=================

I used BootStrap 3 when making this, but you can use your own custom CSS rules if you want to. 

1. Put the "paginator.html" file inside your "_includes" directory
2. Make sure your "index.html" file looks a bit like this:

  ```html
  {% for post in paginator.posts %}
    ...
    ...
    ...
  {% endfor %}
  {% include paginator.html %}
  ```

3. If you're using BootStrap 3 too and wanted to change colors, you can do something like this:

  ```css
  .pagination>.active>a,
  .pagination>.active>span,
  .pagination>.active>a:hover,
  .pagination>.active>span:hover,
  .pagination>.active>a:focus,
  .pagination>.active>span:focus {
    background-color: #CC342D !important;
    border-color: #CC342D !important;
  }
  ```

4. You're done!
