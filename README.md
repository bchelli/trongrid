# Tron Grid
> The Grid. A digital frontier. I tried to picture clusters of information as they moved through the computer. What did they look like? Ships? Motorcycles? Were the circuits like freeways? I kept dreaming of a world I thought I'd never see. And then one day...
> - Kevin Flynn

And then one day, I have created yet a other grid system:
 - simple & light
 - responsive (four breakpoints)
 - fluid (percentage based)
 - pixel gutter (no variable gutter in %)
 - supports nested grid


## Breakpoints
|                       |Extra small devices Phones (≥0)|Small devices Tablets (≥790px)|Medium devices Desktops (≥992px)|Large devices Desktops (≥1200px)|
|----------------------:|:-----------------------------:|:----------------------------:|:------------------------------:|:------------------------------:|
| Breakpoint name       | xs                            | sm                           | md                             | lg                             |
| Container fixed width | None (auto)                   | 750px                        | 970px                          | 1170px                         |
| Class prefix          | ```.col-xs-```                | ```.col-sm-```               | ```.col-md-```                 | ```.col-lg-```                 |
| # of columns          | 12                            | 12                           | 12                             | 12                             |
| Gutter width          | 20px                          | 20px                         | 20px                           | 20px                           |
| Nestable              | Yes                           | Yes                          | Yes                            | Yes                            |


## API
### .row
Container for the grid columns.

### .col-*[breakpoint]*-*[size]*
Column of the size ```size``` for the breakpoint ```breakpoint```.

### .container-fixed
Create a fixed width container.

### .container-fluid
Create a fluid width container.

### .gutter-*[direction]*
Create a margin of the Gutter width, the margin can be on any of the following ```direction```:
   - ```top```
   - ```right```
   - ```bottom```
   - ```left```

### .no-gutter
Remove all the gutter from the columns


## Examples
### Simple
See full example in ```example/1-simple.html```
```html
<div class="container-fluid">
	<div class="row">
		<div class="col-xs-12">12</div>
		<div class="col-xs-2">2</div>
		<div class="col-xs-10">10</div>
		<div class="col-xs-4">4</div>
		<div class="col-xs-8">8</div>
		<div class="col-xs-6">6</div>
		<div class="col-xs-6">6</div>
	</div>
</div>
```

### Fixed width
See full example in ```example/2-fixed-width.html```
```html
<div class="container-fixed">
	<div class="row">
		<div class="col-xs-12">12</div>
		<div class="col-xs-2">2</div>
		<div class="col-xs-10">10</div>
		<div class="col-xs-4">4</div>
		<div class="col-xs-8">8</div>
		<div class="col-xs-6">6</div>
		<div class="col-xs-6">6</div>
	</div>
</div>
```

### Responsive
See full example in ```example/3-responsive.html```
```html
<div class="container-fluid">
	<div class="row">
		<div class="col-xs-12">12</div>
		<div class="col-md-2  col-sm-4  col-xs-6">2</div>
		<div class="col-md-10 col-sm-8  col-xs-6">10</div>
		<div class="col-sm-4  col-xs-6">4</div>
		<div class="col-sm-8  col-xs-6">8</div>
		<div class="col-xs-6">6</div>
		<div class="col-xs-6">6</div>
	</div>
</div>
```

### Nested
See full example in ```example/4-nested.html```
```html
<div class="container-fluid">
	<div class="row">
		<div class="col-xs-12">12</div>
		<div class="col-xs-2">2</div>
		<div class="col-xs-10">10</div>
		<div class="col-xs-4">
			4
			<div class="row">
				<div class="col-xs-6">6</div>
				<div class="col-xs-6">6</div>
			</div>
		</div>
		<div class="col-xs-8">
			8
			<div class="row">
				<div class="col-xs-4">4</div>
				<div class="col-xs-4">4</div>
				<div class="col-xs-4">4</div>
			</div>
		</div>
	</div>
</div>
```

### No gutter
See full example in ```example/5-no-gutter.html```
```html
<div class="container-fluid no-gutter">
	<div class="row">
		<div class="col-xs-12">12</div>
		<div class="col-xs-2">2</div>
		<div class="col-xs-10">10</div>
		<div class="col-xs-4">4</div>
		<div class="col-xs-8">8</div>
		<div class="col-xs-6">6</div>
		<div class="col-xs-6">6</div>
	</div>
</div>
```


## Inspirations
 - [Bootstrap - Grid system](http://getbootstrap.com/css/#grid)
 - [Gridpak - The Responsive grid generator](http://gridpak.com/)
 - [Skeleton: Responsive CSS Boilerplate](http://getskeleton.com/)