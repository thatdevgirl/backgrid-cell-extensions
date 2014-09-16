Backgrid Cell Extensions
=========================

__Author:__ Joni Halabi (www.jhalabi.com)

Description
-----------

This library contains several Backgrid cell extensions that I have found useful for various projects.  You can learn more about Backgrid at http://backgridjs.com/.

StatusFormatterCell
-----------

This cell extends the Backgrid Cell so that it formats status cells appropriately.  Formatting is based on the model value of the given cell and relies on adding a class name to a given cell.  Example CSS is given.

Cell values and classes can be added or modified as necessary.  The cases given here are examples.

ImageCell
-----------

This cell extends the Backgrid Cell so that it inserts an image into the table cell.  Model data should contain the URI of the image.  The column data can optionally include a "class" property to add class name(s) to the image tag.

BooleanCell
-----------

This cell extends the Backgrid Cell so that it replaces a boolean model property value with either "yes" or "no".  Model data should (obviously) be a boolean value.

Usage
-----------

Use any of these extensions as the value of the <em>cell</em> property in the <em>columns</em> object for your Backgrid data table.

<pre>
var columns = [{
	name: 'status',
	label: 'Status',
	cell: StatusFormatterCell
},
{
	name: 'image',
	label: 'Image',
	cell: ImageCell,
	class: 'image-class' // optional
},
{
	name: 'yesno',
	label: 'Yes or No',
	cell: BooleanCell
}];
</pre>
