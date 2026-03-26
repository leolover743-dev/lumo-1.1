<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Lumo</title>

<!-- ⭐ Favicon (small logo for browser tabs & favourites) -->
<link rel="icon" type="image/png" href="https://upload.wikimedia.org/wikipedia/commons/thumb/3/36/Emoji_u1f331.svg/240px-Emoji_u1f331.svg.png">

<style>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    background: #d8f3dc;
    text-align: center;
}

/* Removed black background + changed text to black */
.top-bar {
    background: transparent;
    color: black;
    padding: 10px;
    font-weight: bold;
}

body::before {
    content: "LUMO LUMO LUMO LUMO";
    position: fixed;
    width: 200%;
    height: 200%;
    opacity: 0.04;
    font-size: 90px;
    transform: rotate(-30deg);
    pointer-events: none;
}

.container {
    padding: 20px;
}

.card {
    background: white;
    padding: 20px;
    margin: 20px auto;
    border-radius: 12px;
    max-width: 400px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

button {
    padding: 12px 18px;
    border: none;
    background: #2e7d32;
    color: white;
    border-radius: 6px;
    cursor: pointer;
    font-size: 16px;
}

button:hover {
    background: #1b5e20;
}

input {
    padding: 10px;
    width: 90%;
    margin: 5px;
}

.product img {
    width: 100%;
    border-radius: 10px;
    margin-bottom: 10px;
}

.map iframe {
    border-radius: 10px;
}
</style>

</head>
<body>

<div class="top-bar">
    Phone number: +44 7541 447305
</div>

<div class="container">

<h1>🌿 Lumo</h1>
<p><strong>Plants & Treats that make you smile</strong></p>

<div class="card product">
    <h2>🌱 Spider Plant</h2>

    <a href="https://www.google.com/search?q=spider+plant&tbm=isch" target="_blank">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2c/Chlorophytum_comosum0.jpg/640px-Chlorophytum_comosum0.jpg" alt="Spider Plant">
    </a>

    <p>"Low maintenance, high charm — like your dream bestie, but leafy."</p>
    <p>Small: £2.50<br>Medium: £3.50<br>Large: £5.00</p>

    <button onclick="checkout('plant')">Buy Now</button>
</div>

<div class="card">
    <div class="card product">
    <h2>🧁 Cupcakes</h2>

    <!-- Image (clickable like the plant) -->
    <a href="https://www.google.com/search?q=cupcakes&tbm=isch" target="_blank">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/0b/Cupcakes_chocolate.jpg/640px-Cupcakes_chocolate.jpg" alt="Cupcakes">
    </a>

    <p>"Sweet, soft, and guaranteed to make your day 10× better."</p>

    <!-- Pricing added exactly like the plant card -->
    <p>Single: £2.50<br>Box of 4: £8.00<br>Box of 6: £11.00</p>

    <!-- Order button identical to plant button -->
    <button onclick="checkout('cupcake')">Order Now</button>
</div>

