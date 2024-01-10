<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Full House / Order Food</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color: #ff4d4d;
            color: white;
            text-align: center;
            padding: 1em;
            font-family: 'Pacifico', cursive;
            font-size: 2em;
            font-weight: bold;
            letter-spacing: 2px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            display: flex;
            align-items: center;
            justify-content: center;
        }

        header img {
            width: 30px;
            height: 30px;
            margin-right: 10px;
        }

        section {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
            padding: 2em;
        }

        .item {
            border: 1px solid #ccc;
            border-radius: 12px;
            margin: 1em;
            padding: 1em;
            text-align: center;
            background-color: #fff;
            transition: transform 0.3s ease-in-out;
        }

        .item:hover {
            transform: scale(1.05);
        }

        img {
            max-width: 100%;
            height: auto;
            border-radius: 12px;
            max-height: 150px; /* Set maximum height for smaller images */
        }

        button {
            background-color: #ff4d4d;
            color: white;
            padding: 0.5em 1em;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s ease-in-out;
        }

        button:hover {
            background-color: #ff3333;
        }

        #cart {
            list-style: none;
            padding: 0;
        }

        #total {
            text-align: right;
            margin-top: 1em;
            font-size: 1.2em;
        }

        #buyButton {
            background-color: #ff4d4d;
            color: white;
            padding: 0.5em 1em;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s ease-in-out;
            margin-top: 1em;
        }

        #buyButton:hover {
            background-color: #ff3333;
        }

        #orderForm {
            margin-top: 1em;
            display: flex;
            flex-direction: column;
        }

        #orderForm label {
            margin-bottom: 0.5em;
        }

        #orderForm input {
            padding: 0.5em;
            margin-bottom: 1em;
        }

        /* Added styles for new elements */
        .htmlImage {
            width: 100%;
            height: auto;
            border-radius: 12px;
            max-height: 100px;
            margin-top: 1em;
        }

        .htmlList {
            margin-top: 1em;
        }

        .htmlBlock {
            background-color: #3498db;
            color: white;
            padding: 1em;
            border-radius: 12px;
            margin-top: 1em;
        }

        .htmlTable {
            width: 100%;
            border-collapse: collapse;
            margin-top: 1em;
        }

        .htmlTable th,
        .htmlTable td {
            border: 1px solid #ddd;
            padding: 0.5em;
            text-align: left;
        }

        .htmlForm {
            margin-top: 1em;
        }

        .htmlLink {
            display: block;
            background-color: #2ecc71;
            color: white;
            text-align: center;
            padding: 0.5em;
            text-decoration: none;
            border-radius: 8px;
            margin-top: 1em;
        }

        .htmlLink:hover {
            background-color: #27ae60;
        }
    </style>
</head>

<body>

    <header>
        <img src="https://cdn-icons-png.flaticon.com/512/6676/6676508.png" alt="Logo">FULL HOUSE
    </header>

    <section>
        <div class="item">
            <img src="https://static.vecteezy.com/system/resources/previews/022/598/687/original/tasty-beef-burger-png.png"
                alt="Burger">
            <h2 style="color: #e74c3c;">Burger</h2>
            <p>Delicious burger with all the fixings</p>
            <p style="color: #3498db;">Price: €5.99</p>
            <button onclick="order('Burger', 5.99)">Order</button>
        </div>

        <div class="item">
            <img src="https://png.pngtree.com/png-vector/20230321/ourmid/pngtree-modern-kitchen-food-boxed-cheese-lunch-pizza-png-image_6651523.png"
                alt="Pizza">
            <h2 style="color: #e74c3c;">Pizza</h2>
            <p>Classic pizza with your favorite toppings</p>
            <p style="color: #3498db;">Price: €8.99</p>
            <button onclick="order('Pizza', 8.99)">Order</button>
        </div>

        <div class="item">
            <img src="https://png.pngtree.com/png-clipart/20210418/original/pngtree-cooking-gourmet-snack-pasta-png-image_6241443.jpg"
                alt="Pasta">
            <h2 style="color: #e74c3c;">Pasta</h2>
            <p>Homemade pasta with rich tomato sauce</p>
            <p style="color: #3498db;">Price: €7.49</p>
            <button onclick="order('Pasta', 7.49)">Order</button>
        </div>

        <div class="item">
            <img src="https://www.plantbasedredhead.com/wp-content/uploads/2021/01/Jani-me-Fasule_Albanian-white-bean-soup_Albanische-weise-Bohnensuppe-_plantbasedredhead.com_1-720x720.jpg"
                alt="Pasul">
            <h2 style="color: #e74c3c;">Pasul</h2>
            <p>Traditional Albanian white bean soup</p>
            <p style="color: #3498db;">Price: €6.99</p>
            <button onclick="order('Pasul', 6.99)">Order</button>
        </div>

        <div class="item">
            <img src="https://i.pinimg.com/564x/94/70/55/9470553fe42f43afc0ce17b4e1203d93.jpg" alt="Fli">
            <h2 style="color: #e74c3c;">Fli</h2>
            <p>Traditional Albanian layered pastry</p>
            <p style="color: #3498db;">Price: €9.49</p>
            <button onclick="order('Fli', 9.49)">Order</button>
        </div>

        <div class="item">
            <img src="https://www.tiranaecho.com/wp-content/uploads/2017/05/a.jpg" alt="Laknur">
            <h2 style="color: #e74c3c;">Laknur</h2>
            <p>Traditional Albanian dish</p>
            <p style="color: #3498db;">Price: €11.99</p>
            <button onclick="order('Laknur', 11.99)">Order</button>
        </div>
    </section>

    <section>
        <h2 style="color: #ffcc00;">Order Summary</h2>
        <ul id="cart"></ul>
        <p id="total">Total: €<span id="totalAmount">0.00</span></p>
        <div id="orderForm">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name">

            <label for="address">Address:</label>
            <input type="text" id="address" name="address">
        </div>
        <button id="buyButton" onclick="buy()">Buy</button>
    </section>

    <script>
        let totalPrice = 0;

        function order(itemName, itemPrice) {
            const cartElement = document.getElementById('cart');
            const listItem = document.createElement('li');
            listItem.textContent = `${itemName} - €${itemPrice.toFixed(2)}`;
            cartElement.appendChild(listItem);

            totalPrice += itemPrice;
            document.getElementById('totalAmount').textContent = totalPrice.toFixed(2);
        }

        function buy() {
            const name = document.getElementById('name').value;
            const address = document.getElementById('address').value;

            if (!name || !address) {
                alert("Please enter your name and address before buying.");
            } else {
                alert(`Hello, ${name}! Your food has been sent to ${address}.`);
                // You can replace the alert with a more sophisticated notification system
                // with a 5-second duration.
            }
        }
    </script>
</body>

</html>

