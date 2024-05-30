#HTML CODE
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amazon Clone</title>
    <link rel="stylesheet" href="style.css">

</head>
<body>
    <header>
        <div class="logo">
            <img src="C:\Users\pk956\Downloads\2062062_amazon_buy_logo_online_shop_icon.png" alt="Amazon Logo">
        </div>
        <div class="search-bar">
            <input type="text" placeholder="Search for products">
            <button>Search</button>
        </div>
        <div class="account">
            <a href="#">Sign In</a>
        </div>
        <div class="cart">
            <a href="#">Cart</a>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="#">Best Sellers</a></li>
            <li><a href="#">Customer Service</a></li>
            <li><a href="#">New Releases</a></li>
            <li><a href="#">Today's Deals</a></li>
            <li><a href="#">Gift Cards</a></li>
        </ul>
    </nav>

    <main>
        <section class="products">
            <div class="product">
                <img src="C:\Users\pk956\Downloads\63535b25b5de690b573a9ac2-airwrap-complete-styler-for-dyson.jpg" alt="Product 1">
                <h2>DYSON AIRWRAP</h2>
                <p>$19.99</p>
                <button>Add to Cart</button>
            </div>
            <div class="product">
                <img src="C:\Users\pk956\Downloads\refurb-macbook-air-m2-spacegray-202208.jpeg" alt="Product 2">
                <h2>MACBOOK AIR M2</h2>
                <p>$29.99</p>
                <button>Add to Cart</button>
            </div>
            <!-- Add more products as needed -->
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Amazon Clone</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
#css codebody {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

header {
    background-color: #232F3E;
    color: white;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px 20px;
}

.logo img {
    height: 50px;
}

.search-bar {
    display: flex;
    flex: 1;
    margin: 0 20px;
}

.search-bar input {
    width: 100%;
    padding: 10px;
}

.search-bar button {
    padding: 10px;
    background-color: #FF9900;
    border: none;
    cursor: pointer;
}

.account, .cart {
    margin-left: 20px;
}

nav {
    background-color: #131A22;
    padding: 10px 20px;
}

nav ul {
    list-style: none;
    display: flex;
    margin: 0;
    padding: 0;
}

nav ul li {
    margin-right: 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

main {
    padding: 20px;
}

.products {
    display: flex;
    flex-wrap: wrap;
}

.product {
    border: 1px solid #ddd;
    margin: 10px;
    padding: 20px;
    width: calc(33.333% - 40px);
    box-sizing: border-box;
    text-align: center;
}

.product img {
    max-width: 100%;
    height: auto;
}

.product h2 {
    font-size: 18px;
    margin: 10px 0;
}

.product p {
    font-size: 16px;
    color: #B12704;
}

.product button {
    padding: 10px;
    background-color: #FF9900;
    border: none;
    cursor: pointer;
}

footer {
    background-color: #232F3E;
    color: white;
    text-align: center;
    padding: 10px 20px;
    position: fixed;
    width: 100%;
    bottom: 0;
}
#js code
document.addEventListener("DOMContentLoaded", () => {
    const searchButton = document.querySelector(".search-bar button");
    const searchBar = document.querySelector(".search-bar input");

    searchButton.addEventListener("click", () => {
        const query = searchBar.value;
        alert(`You searched for: ${query}`);
    });
});

