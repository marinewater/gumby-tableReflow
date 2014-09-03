Gumby tableReflow Module
=================

This UI module is an implementation of the [JQuery Mobile Table Reflow Widget](http://demos.jquerymobile.com/1.4.3/table-reflow/) for the Gumby Framework.

Installation
------------

A bower package is available to install this repo into your project. We recommend using this method to install Gumby and any extra UI modules, however you can alternatively move the individuals files into your project.

```bash
$ bower install gumby-tableReflow
```

Include gumby.tablereflow.js in the same fashion as your other UI modules, after gumby.js and before gumby.init.js. In production you should minify JavaScript files into a single optimized gumby.min.js file, ensuring the order (gumby.js, UI modules, gumby.init.js) is retained. 

```html
<!--
Include gumby.js followed by UI modules.
Or concatenate and minify into a single file-->
<script src="js/libs/gumby.js"></script>
<script src="js/libs/ui/gumby.skiplink.js"></script>
<script src="js/libs/ui/gumby.toggleswitch.js"></script>
<!-- included from Bower's components directory -->
<script src="components/gumby.tablereflow.js"></script>
<script src="js/libs/gumby.init.js"></script>

<!-- In production minifiy and combine the above files into gumby.min.js -->
<script src="js/libs/gumby.min.js"></script>
<script src="js/plugins.js"></script>
<script src="js/main.js"></script>
```
	
Import the _reflow.scss partial in the same fashion as your other imports. Once you compile sass you are good to go.

```scss
// imported from Bower's components directory
@import "../components/reflow";
```


Usage
-----

Using the parallax module is simple. Add a class of `reflow` to a table (the table has to use tbody and thead):

```html
<table class="reflow">
	<thead>
		<tr>
			<th>Lorem.</th>
			<th>Voluptas.</th>
			<th>At.</th>
			<th>Esse.</th>
			<th>Odio!</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Lorem ipsum.</td>
			<td>Quisquam, ipsa.</td>
			<td>Quo, hic?</td>
			<td>Reiciendis, minima.</td>
			<td>Totam, necessitatibus.</td>
		</tr>
		<tr>
			<td>Lorem ipsum.</td>
			<td>Nesciunt, neque.</td>
			<td>Quo, ullam.</td>
			<td>Facilis, omnis.</td>
			<td>Quisquam, iure.</td>
		</tr>
		<tr>
			<td>Lorem ipsum.</td>
			<td>Eius, error.</td>
			<td>A, quia!</td>
			<td>Sunt, obcaecati.</td>
			<td>Voluptates, est.</td>
		</tr>
		<tr>
			<td>Lorem ipsum.</td>
			<td>Sunt, aliquam.</td>
			<td>Nobis, dolor.</td>
			<td>Deserunt, autem.</td>
			<td>Quis, ipsa?</td>
		</tr>
		<tr>
			<td>Lorem ipsum.</td>
			<td>Necessitatibus, at!</td>
			<td>Debitis, recusandae.</td>
			<td>Molestias, quas.</td>
			<td>Praesentium, totam!</td>
		</tr>
	</tbody>
</table>
```

Now resize your browser window and see what happens.

There are three variables in the _reflow.scss you may want to override:
* `$table-reflow-breakpoint` This is the maximum screen size in which the table is displayed in reflow mode.
* `$table-reflow-row-margin` The margin between rows in table mode.
* `$table-reflow-header-min-width` Basicly the left column size in reflow mode.


**MIT Open Source License**

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

	
	

