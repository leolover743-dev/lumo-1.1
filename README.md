# lumo-1.1
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Lumo</title>

<style>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    background: #d8f3dc;
    text-align: center;
}

.top-bar {
    background: #111;
    color: white;
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
    <h2>🧁 Cupcakes</h2>
    <p>You deserve a treat… and lucky for you, we’ve got the sweetest ones right here.</p>
    <p>Price: £2.50</p>
    <p>10% of money earned goes to charity ❤️</p>

    <button onclick="checkout('cupcake')">Order Now</button>
</div>

<!-- ✅ WORKING EMAIL FORM -->
<div class="card">
    <h2>Contact</h2>

    <form action="https://formsubmit.co/hugorb2@outlook.com" method="POST">
        <input type="text" name="name" placeholder="Your name" required>
        <input type="email" name="email" placeholder="Your email" required>

        <!-- Optional message -->
        <input type="text" name="message" placeholder="Your message">

        <!-- Disable captcha from FormSubmit -->
        <input type="hidden" name="_captcha" value="false">

        <button type="submit">Send</button>
    </form>
</div>

<div class="card map">
    <h2>📍 Find Us</h2>
    <p>Outside Newbury Train Station, Newbury, England</p>

    <iframe
        width="100%"
        height="250"
        loading="lazy"
        allowfullscreen
        src="https://www.google.com/maps?q=Newbury+Train+Station,+Newbury,+England&z=17&output=embed">
    </iframe>
</div>

<p>© 2026 Lumo — Making the world greener & sweeter 🌍</p>

</div>

<script>
function checkout(item) {
    if (item === 'plant') {
        window.location.href = "https://buy.stripe.com/test_plant_link";
    }
    if (item === 'cupcake') {
        window.location.href = "https://buy.stripe.com/test_cupcake_link";
    }
}
</script>

</body>
</html>
