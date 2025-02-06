/* Basic Styling */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
}

/* Navbar Styling with Animation */
.navbar {
    background-color: #2c3e50;
    padding: 10px 20px;
    position: sticky;
    top: 0;
    z-index: 10;
    animation: slideDown 0.5s ease-out;
}

.navbar ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: space-around;
}

.navbar .nav-link {
    color: white;
    text-decoration: none;
    font-size: 18px;
    transition: color 0.3s ease;
}

.navbar .nav-link:hover {
    color: #3498db;
}

/* Page Content Styling */
.main-content {
    padding: 50px 20px;
    text-align: center;
}

h1 {
    font-size: 36px;
    margin-bottom: 20px;
}

/* Product Cards */
.product-cards {
    display: flex;
    justify-content: center;
    gap: 20px;
}

.product-card {
    background-color: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
    width: 250px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.product-card img {
    width: 100%;
    height: auto;
    border-radius: 8px;
}

.product-card h2 {
    font-size: 22px;
    margin: 10px 0;
}

.product-card p {
    font-size: 18px;
    color: #2c3e50;
}

.product-card .shop-now {
    background-color: #3498db;
    color: white;
    padding: 10px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 16px;
    transition: background-color 0.3s ease;
}

.product-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 15px rgba(0, 0, 0, 0.15);
}

.product-card .shop-now:hover {
    background-color: #2980b9;
}

/* Animation for Page Transitions */
@keyframes slideDown {
    from {
        opacity: 0;
        transform: translateY(-50px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}
