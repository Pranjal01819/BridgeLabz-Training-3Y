# Question 2 — Product Catalog

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Online Store Product Catalog</title>
</head>
<body>

    <h1>Online Store Product Catalog</h1>

    <table border="1">
        <tr>
            <th colspan="5">Featured Products</th>
        </tr>
        <tr>
            <th>Image</th>
            <th>Product Name</th>
            <th>Description</th>
            <th>Price</th>
            <th>Availability</th>
        </tr>

        <tr>
            <td><img src="laptop.jpg" alt="Laptop" width="120"></td>
            <td>Laptop</td>
            <td>High-performance laptop for students and professionals.</td>
            <td>₹65,000</td>
            <td rowspan="2">In Stock</td>
        </tr>

        <tr>
            <td><img src="headphones.jpg" alt="Headphones" width="120"></td>
            <td>Wireless Headphones</td>
            <td>Noise-reducing wireless headphones.</td>
            <td>₹3,999</td>
        </tr>

        <tr>
            <td><img src="keyboard.jpg" alt="Keyboard" width="120"></td>
            <td>Mechanical Keyboard</td>
            <td>Compact mechanical keyboard with RGB lighting.</td>
            <td>₹2,499</td>
            <td>Limited Stock</td>
        </tr>

        <tr>
            <td colspan="4"><strong>Special Offer</strong></td>
            <td>Available</td>
        </tr>
    </table>

</body>
</html>
```
