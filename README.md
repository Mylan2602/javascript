<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="mang.js"></script>
</head>
<body>
    Custumer name:
    <input type="text" id="name">
    <br>
    ID: 
    <input type="text" id="id">
    Product name: 
    <input type="text" id="product">
    <br>
    Quantity:
    <input type="text" id="quantity">
    <br>
    Price:
    <input type="text" id="price">
    <br>
    <input type="button" value="save" onclick="save()">
    <input type="button" value="show" onclick="show()">
    <input type="button" value="reset" onclick="reset()">
    <table class="thead-dark">
        <thead>
            <tr>
                <th>Auto increment</th>
                <th>Custumer name</th>
                <th>ID</th>
                <th>Product name</th>
                <th>Quantity</th>
                <th>Price</th>
                <th>Total</th>
            </tr>
        </thead>
        <tbody id="tbl"></tbody>
    </table>
</body>
</html>
