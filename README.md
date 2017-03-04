# Simple CSS library

Visit [hosted website](http://simple-css.surge.sh/) for template example

## Features
- 12 column responsive grid layout
- Responsive for desktop, tablet and phone
- Horizontal and vertical text align
- Column offset
- Equal row column heights

## Grid layout (Cross browser compatible)
Prefix all grid columns with .col and specify the number of columns you would like your content to occupy (up to 12). Specify number of columns for small and medium screens `(.sm-col & .md-col)`.

Nest `.col` classes in a `.row` class if the number of columns are less than 12 (to prevent float bubbling).

You may nest your rows and columns within a `.container` class which provides padding in desktop view.

Add the `.offset` class with the number of cols you would like to offset by from the left.

Add .row-eq-height for equal column heights (Note: only use as needed, will sacrifice ability to set bottom margin and padding of col. Use div wrapper if needing to set these properties).

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

  <div class="row row-eq-height">
    <div class="col col-6">
      <p>Lorem ipsum.</p>
    </div>
    <div class="col col-6">
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quo, facere quia! Eius ipsa quae eos dolor dolorum optio nesciunt a.</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>

  </div>
</div>
```

## Text positioning
Add div class of `.left .right .center .justify` to align text within divs horizontally. For small and medium devices prefix with `.sm-left .md-left` etc.

## Author
Howie_Burger (2017)
