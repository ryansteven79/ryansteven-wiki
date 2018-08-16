<!-- TITLE: Sample Code -->
<!-- SUBTITLE: displayTable-test -->

# Header


```javascript
function displayTable() {
    connection.query("SELECT * FROM products", function (err, results) {
        console.table(results);
        connection.end();
    })
}
```
