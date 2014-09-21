table-resize
============

Adds basic functionality to html tables: resizing.

###Samples

See [here](http://irhc.github.io/table-resize) for some samples.

###Description

table-resize a small and simple javascript component which adds basic functionality to html tables: resizing. It is completely independent from other javascript libraries but should work side-by-side with libraries like jQuery, etc.

Any html tables which have at least one tr tag can be used (a thead or tbody tag is not mandatory), e.g.

```html
<table id="example">
    <tbody>
        <tr>
            <th>Name</th>
            <th>&Auml;nderungsdatum</th>
            <th>Typ</th>
            <th>Gr&ouml;&szlig;e</th>
        </tr>
        <tr>
            <td>libraries</td>
            <td>08.10.2013 12:38</td>
            <td>Dateiordner</td>
            <td></td>
        </tr>
        <tr>
            <td>views</td>
            <td>08.10.2013 12:38</td>
            <td>Dateiordner</td>
            <td></td>
        </tr>
        <tr>
            <td>css</td>
            <td>18.05.2014 11:08</td>
            <td>Dateiordner</td>
            <td></td>
        </tr>
        <tr>
            <td>.htaccess</td>
            <td>03.06.2013 14:29</td>
            <td>HTACCESS-Datei</td>
            <td>1 KB</td>
        </tr>
        <tr>
            <td>config.php</td>
            <td>03.06.2013 14:29</td>
            <td>PHP-Datei</td>
            <td>3 KB</td>
        </tr>
        <tr>
            <td>blank.html</td>
            <td>18.05.2014 11:08</td>
            <td>HTLM-Datei</td>
            <td>1 KB</td>
        </tr>
    </tbody>
</table>
```

###Options

distance (default 0): Sets the radius of a circle, where no drag action is triggered as long as mouse movements are within the circle.
minWidth (default 30): Sets the minimum width of the cells.
restoreState (default true): localStorage is used to remember the last width of the cells if true.

###How to use

In the head section of your html file put

```html
<link href='table-resize.css' rel='stylesheet'>
```

Just before the end of your body section put

```html
<script src='table-resize.min.js'></script>
<script>
  new TableResize(document.getElementById('example'));
  //new TableResize(document.getElementById('example'), {distance: 100, minWidth: 60, restoreState: true});
</script>
```

###Supported browsers

- Internet Explorer 8 and newer
- Opera
- Chrome
- Firefox
- Safari 5.1.7 (and highly possible newer)

###References

This small javascript component uses or is based on other javascript projects and code snippets:

- [Resizable Table Columns Demo](http://bz.var.ru/comp/web/resizable.html)
- [mouse.js by jQuery](https://github.com/jquery/jquery-ui/blob/master/ui/mouse.js)
- [addEvent() recoding contest entry](http://ejohn.org/apps/jselect/event.html)

### Licence

MIT


