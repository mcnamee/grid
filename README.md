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
- **.grid_x** - the grid columns
- **.prefix_x** - add white space before an element the width of column x
- **.hidden_x** - hide element on x (predefined xs, s, m, l & xl) size screen
- **.visible_x** - only show element on x size screen
- **Utility classes** - makes life easier with predefined classes such as .clear, .text_align_left (or center or right), .scale_with_grid (add to images to automatically scale as the grid scales)
- **HTML resets** - all included!

## Installation

### 1. Download & Link up the stylesheet

- Download the grid.min.css (or grid.css if you prefer) file and place within your css directory

- Add the downloaded stylesheet within your HTML `<head>` (matching your file structure):

`<link rel="stylesheet" href="/css/grid.min.css">`

### 2. Meta tag

Add this meta tag within your HTML `<head>`:

`<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1" />`

### 3. Moderizr

Install Modernizr within your HTML `<head>` for backward compatibility (specifically IE7):

`<script src="http://ajax.aspnetcdn.com/ajax/modernizr/modernizr-2.6.2.js"></script>`:

### 4. Start using!

Simply nest your `.grid_x` within a `.container_24` div and you're away
