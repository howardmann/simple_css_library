# Simple CSS library

Visit [hosted website](http://simple-css.surge.sh/) for template example

## Features
- 12 column responsive grid layout
- Responsive for desktop, tablet and phone
- Horizontal and vertical text align
- Column offset

## Updates Dec 2016
- Flexbox horizontal and vertical alignment (flex and flex-column | flex-center, flex-end, flex-space-betwen, flex-space-around)
- Flexbox ordering for horizontal divs (note this does not currently have support for vertical ordering)
- Sticky footer using flexbox. Add sticky-footer class to body and main
- Hiding divs based on tablet and phone media query (sm-hide, md-hide)

## Grid layout
Prefix all grid columns with .col and specify the number of columns you would like your content to occupy (up to 12). Specify number of columns for small and medium screens (.sm-col & .md-col).

Nest .col classes in a .row class if the number of columns are less than 12 (to prevent float bubbling).

You may nest your rows and columns within a .container class which provides padding in desktop view.

Add the .offset class with the number of cols you would like to offset by from the left.

```html
<div class="container">
  <div class="row">
    <div class="col sm-col-12 md-col-6 col-3">sm-col-12 md-col-6 col-3</div>
    <div class="col sm-col-12 md-col-6 col-3">sm-col-12 md-col-6 col-3 </div>
    <div class="col sm-col-12 md-col-6 col-3">sm-col-12 md-col-6 col-3 </div>
    <div class="col sm-col-12 md-col-6 col-3">sm-col-12 md-col-6 col-3 </div>
  </div>

  <div class="row">
    <div class="col col-4 offset-4">col-4 offset-4</div>
  </div>
</div>
```

## Text positioning
Add div class of .left .right .center .justify to align text within divs horizontally.

## Author
Howie_Burger (2016)
