**SHUN - SIMPLE FLEX-BOX BASED FRAMEWORK**
> Shun is a framework that is designed to have basic functionality
> based around flex-box containing few repeating css properties dumped to classes
> to decrease the time spent working on web projects.

**Why "Shun"?**
> As stated here: https://www.dictionary.com/browse/shun, shun means *to avoid*.
> In this case we are avoiding overcomplicated solutions when it comes to flex-box.

**Shun features**
- Simple row/column based layout
- Reset for all HTML Elements
- Few classes for ordering, aligning etc.
- No padding nor margin added by default to storer( container ), wrapper( row ) and col( columns )
- Shun has its breakpoints, currently supporting from 195px ( width ) to 1400px ( width ) and from 1400px ( width ) to infinite px
- Layout is based on 24 columns

**Some examples of code...**

exp* = *(Note that adding this will require display: flex, or already defined class in Shun: flex)*

Basic usage of Storer, Wrapper, Cols
```
<div class="storer">
  <div class="flex wrapper">
      <div class="flex col-8">
        <p>FLEX COL 8 J-START</p>
      </div>
      <div class="flex col-8">
        FLEX COL 8 J-END
      </div>
      <div class="flex col-8">
        FLEX COL 8 J-CENTER
      </div>
   </div>
</div>
```
Justify Content usage: (exp*)
```
.j-{aligment}

{alignment} = start, end, center, between, around
```
Example:
```
<div class="storer">
  <div class="flex wrapper">
      <div class="flex col-8 j-start">
        <p>FLEX COL 8 J-START</p>
      </div>
      <div class="flex col-8 j-end">
        FLEX COL 8 J-END
      </div>
      <div class="flex col-8 j-center">
        FLEX COL 8 J-CENTER
      </div>
   </div>
</div>
```

Align Items usage: (exp*)
```
.a-{aligment}

{alignment} = start, end, center, stretch
```


Align Self usage: (exp*)
```
.s-{aligment}

{alignment} = start, end, center
```

Align Content usage: (exp*)
```
.c-{aligment}

{alignment} = start, end, center, between
```


https://flatuicolors.com/palette/se
