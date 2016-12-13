# Responsive CSS Grid

A 24 column percentage based responsive CSS grid scaling from the base 1008px, to:
- (xl) > 1200px
- (m) 768px - 1023px
- (s) 480px - 767px
- (xs) < 479px

## Benefits
- **Quicker development** - use the grid as scaffolding to quickly layout the website design, then style - you won't know yourself!
- **Be precise** - with more columns at your fingertips, you're able to be pixel perfect quicker
- **Flexibility** - hide something on mobile-portrait sized screens (.hidden_xs), only show on tablet sized screens (.visible_m) + more - very easy!
- **Compatible** back to IE8 (wow it doesn't break on Internet Explorer!)

## Features
- **.grid_x** - the grid columns (1 to 24)
- **.grid_x_y** - append _y (i.e. xs, s, m, l or xl) to a grid_x (eg. `<div class="grid_24 grid_12_m"></div>` is 24 columns everywhere except on m size, where it's 12 columns)
- **.prefix_x** - add white space before an element the width of column x
- **.hidden_y** - hide element on y (i.e. xs, s, m, l or xl) size screen
- **.visible_y** - only show element on y (i.e. xs, s, m, l or xl) size screen
- **Utility classes** - makes life easier with predefined classes such as .clear, .text_align_left (or center or right), .scale_with_grid (add to images to automatically scale as the grid scales)
- **HTML resets** - all included!

### Source Ordering
- Switch the position/order of divs in a row based on the media query. i.e. image right text left on desktop, image top text bottom on mobile.
- **.push_x** - push div x columns to the right
- **.push_x_y** - append _y (i.e. xs, s, m, l or xl) to a push_x (eg. `<div class="grid_12 push_12_m"></div>` is 12 columns wide and is pushed 12 columns to the right on size grid_m)
- **.pull_x** - pull div x columns to the left
- **.pull_x_y** - append _y (i.e. xs, s, m, l or xl) to a pull_x (eg. `<div class="grid_12 pull_12_m"></div>` is 12 columns wide and is pulled 12 columns to the left on size grid_m)

### .row class
- Inside your container_24 div add in a .row div to wrap all of your 'grid_x divs. This will auto clear all the floats within the row
- Add the class .outer to your .row div and it will add -10px margin to each side of the row. This is used to offset the outermost .inner margin added to .grid_12 inner divs. i.e. `<div class="row outer"><div class="grid_12 inner"></div><div class="grid_12 inner"></div></div>`

### Gutter Widths
- Add `.medium_gutters` or `.large_gutters` to your enclosing `.row` element to change the gutter widths to 15px or 20px respectively.

### .5ths grid class
- **Need to create a column layout that is 5 columns wide?** Then use .grid_5th or .grid_5th_y (where y is a grid size i.e. xs, s, m, l or xl) and it will line up nicely.

## Installation

### 1. Download & Link up the stylesheet

- Download the grid.css file and place within your scss directory

- Add grid.css to your SASS/SCSS structure as a SASS Partial (or minify it and include it in your HTML `<head>` as below) 

`<link rel="stylesheet" href="/css/grid.min.css">` (Matching your file structure of course!)

### 2. Meta tag

Add this meta tag within your HTML `<head>`:

`<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1" />`

### 3. Moderizr

Install Modernizr within your HTML `<head>` for backward compatibility (specifically IE7):

`<script src="http://ajax.aspnetcdn.com/ajax/modernizr/modernizr-2.6.2.js"></script>`:

### 4. Start using!

Simply nest your `.grid_x` within a `.container_24` div and you're away
