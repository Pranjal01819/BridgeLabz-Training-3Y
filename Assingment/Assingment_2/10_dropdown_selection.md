# Question 10 — Dropdown-Based Selection

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Travel Selection</title>
</head>
<body>

    <h1>Select Your Travel Preferences</h1>

    <form>
        <label for="country">Country:</label>
        <select id="country" name="country">
            <option selected>India</option>
            <option>Japan</option>
            <option>France</option>
            <option>Australia</option>
        </select>
        <br><br>

        <label for="state">State:</label>
        <select id="state" name="state">
            <option selected>Uttar Pradesh</option>
            <option>Rajasthan</option>
            <option>Goa</option>
            <option>Himachal Pradesh</option>
        </select>
        <br><br>

        <label for="city">City:</label>
        <select id="city" name="city">
            <option selected>Mathura</option>
            <option>Jaipur</option>
            <option>Goa</option>
            <option>Manali</option>
        </select>
        <br><br>

        <label for="place">Favorite Tourist Place:</label>
        <select id="place" name="place">
            <option selected>Vrindavan</option>
            <option>Hawa Mahal</option>
            <option>Baga Beach</option>
            <option>Solang Valley</option>
        </select>
    </form>

    <p>
        My selected choices are India as the country, Uttar Pradesh as the state,
        Mathura as the city, and Vrindavan as my favorite tourist place.
    </p>

</body>
</html>
```
