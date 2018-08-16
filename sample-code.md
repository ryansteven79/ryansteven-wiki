<!-- TITLE: Sample Code -->
<!-- SUBTITLE: display table -->

# Header


```javascript
function displayTable() {
    connection.query("SELECT * FROM products", function (err, results) {
        console.table(results);
        connection.end();
    })
}
```
