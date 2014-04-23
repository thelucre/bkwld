# hot sauce

ok, bkwld. here's the beef. 

i created the grid from scratch. very interesting excerise. smart, on your part. i see why this could be a headache. 

i spent 3 hours making the grid work, 4 hours styling and pluggin in content, and a little extra to fix for ie 7/8

## how to use

every row needs a div wrapper with the row class. each column should have a row-* and col-* class added to choose the size you want.

### class options

1. Columns - specify width
  * .col-full
  * .col-53
  * .col-46
  * .col-26
2. Rows - specify height
  * .row-full
  * .row-xxlg
  * .row-xlg
  * .row-lg
  * .row-md
  * .row-sm
  * .row-xsm

_full header row example_

```html
<div class="row">
    <div id="header" class="col-full row-full">
        <h1 class="intro">Goodbye, <br/>Barbados!</h1>
    </div>
</div>
```

### nesting

when you have a nested row, add the .nested-right or .nested-left class. column classes should be added to the nested element, no the child.

_nesting example_

```html
<div class="row">
    <div id="pink-sky" class="col-46 row-xxlg photo-box">
        Left Pane Content
    </div>
    <div class="row col-53 nested-right">
        <div class="row-xsm pink">
             Right Pane Upper Content
        </div>
    </div>
    <div class="row col-53 nested-right">
        <div class="row-lg navy">
        	Right Pane Lower Content
        </div>
    </div>
</div>
```