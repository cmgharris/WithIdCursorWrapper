WithIdCursorWrapper
===================
Subclass of Android CursorWrapper wich adds an _id column to the result set of a cursor if there is not one already.
_id column is required by the CursorAdaptor for a ListFragment; this class is a means of providing it if not already present.
If not already present, _id will by default be added as the first column, or, using the optional constructor, 
can be specified as the last column.
If added by this class, the value of the column will be the position of the row in the result set.
