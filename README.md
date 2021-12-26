# SHUN - SIMPLE FLEX-BOX BASED FRAMEWORK
![Shun](https://github.com/yadibolt/shun/blob/main/Shun.png)
> Shun is a framework that is designed to have basic functionality
> based around flex-box containing few repeating css properties dumped to classes
> to decrease the time spent working on web projects.

## Why "Shun"?
> As stated here: https://www.dictionary.com/browse/shun, shun means *to avoid*.
> In this case we are avoiding overcomplicated solutions when it comes to flex-box.

**Shun features**
- Simple row/column based layout
- Reset for all HTML Elements
- Few classes for ordering, aligning etc.
- No padding nor margin added by default to storer( container ), wrapper( row ) and col( columns )
- Shun has its breakpoints, currently supporting from 195px ( width ) to 1400px ( width ) and from 1400px ( width ) to infinite px
- Layout is based on 24 columns


## Basic usage of Storer, Wrapper, Cols
- using *.rev-wrapper* instead of *.wrapper* will reverse the wrapper

**Example**
```html
<div class="storer">
  <div class="flex wrapper">
      <div class="flex col-8">
        <p>FLEX COL 8 J-START</p>
      </div>
      <div class="flex col-8">
        <p>FLEX COL 8 J-END</p>
      </div>
      <div class="flex col-8">
        <p>FLEX COL 8 J-CENTER</p>
      </div>
   </div>
</div>
```

## Breakpoints
```
.col-{prefix}-{number_of_columns} | usage of columns with breakpoints
```
- from **195px** to **320px** | XS | prefix = xs
- from **321px** to **576px** | S | prefix = s
- from **577px** to **768px** | M | prefix = m
- from **769px** to **992px** | L | prefix = l
- from **993px** to **1200px** | XL | prefix = xl
- from **1201px** to **1400px** | H | prefix = h
- from **1401px** to **infinite px** | XH | prefix = xh

**Example**
```html
<div class="storer">
  <div class="flex wrapper">
    <div class="flex col-xs-24 col-s-12">
      <p>FLEX COL 24 on XS & FLEX COL 12 on S</p>
    </div>
  </div>
</div>
```

## Alignment of elements
```
.{prefix}-{aligment} | usage of alignment classes
```
Others:
- Justify Content, prefix **j** | Alignments: start, end, center, between, around
- Align Items, prefix: **a** | Alignments: start, end, center, stretch
- Align Self, prefix: **s** | Alignments: start, end, center
- Align Content, prefix: **c** | Alignments: start, end, center, between

**Example**
```html
<div class="storer">
  <div class="flex wrapper">
      <div class="flex col-8 j-start">
        <p>FLEX COL 8 J-START</p>
      </div>
      <div class="flex col-8 j-end">
        <p>FLEX COL 8 J-END</p>
      </div>
      <div class="flex col-8 j-center">
        <p>FLEX COL 8 J-CENTER</p>
      </div>
   </div>
</div>
```

## Ordering
```
.ord-{breakpoint_prefix}-{order_number} | usage of order classes based on breakpoints
```
**Example**
```html
<div class="storer">
  <div class="flex wrapper">
      <div class="flex col-8 ord-s-1">
        <p>FIRST</p>
      </div>
      <div class="flex col-8 ord-s-3">
        <p>SECOND</p>
      </div>
      <div class="flex col-8 ord-s-2">
        <p>THIRD</p>
      </div>
   </div>
</div>
```

## Spacing
```
.m{direction}-{spacing-number} | usage of margin classes based on breakpoints
.p{direction}-{spacing-number} | usage of padding classes based on breakpoints

{direction} = t, b, s, e
{spacing-number} = from 0 to 5
*t = top
*b = bottom
*s = start
*e = end
```
**Example**
```html
<div class="storer">
  <div class="flex wrapper mt-5 py-3">
    <div class="flex col-24 px-5 me-5">
      <p>FLEX COL 24 on XS & FLEX COL 12 on S</p>
    </div>
  </div>
</div>
```

## Other utility classes
```scss
.flex {
    display: flex !important;
}
.w-100 {
    width: 100%;
}
.h-100 {
    height: 100%;
}
.vw-100 {
    width: 100vw;
}
.vh-100 {
    height: 100vh;
}
.of-hidden {
    overflow: hidden;
}
.of-scroll {
    overflow: scroll;
}
.of-visible {
    overflow: visible;
}
```
# Summary
You are free to use this unless you remove credits or share/claim this under your name.

Any improvements are welcome!

Source for colors I've used:

https://flatuicolors.com/palette/se
