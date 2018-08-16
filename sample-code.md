<!-- TITLE: Sample Code -->

# function displayTable


```javascript
function displayTable() {
    connection.query("SELECT * FROM products", function (err, results) {
        console.table(results);
        connection.end();
    })
}
```
