<!DOCTYPE html>
<html>
<head>
    <title>The Latte Library - Full Menu</title>
    <style>
        body {
            font-family: 'Georgia', serif;
            background-color: #f7f1e3;
            color: #4b3f35;
            margin: 0;
            padding: 0;
            background-image: url('https://wallpaperaccess.com/full/9524787.jpg');
            background-size: cover;
            background-attachment: fixed;
            background-repeat: no-repeat;
        }

        header {
            background-color: rgba(245, 233, 215, 0.95);
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 50px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }

        header img {
            height: 60px;
        }

        nav {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        nav a {
            text-decoration: none;
            color: #4b3f35;
            font-weight: bold;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #8a6e4b;
        }

        .cart-icon {
            font-size: 22px;
            margin-left: 20px;
            cursor: pointer;
            color: #4b3f35;
            transition: color 0.3s;
            position: relative;
        }

        .cart-icon:hover {
            color: #8a6e4b;
        }

        #cartBadge {
            background: #b8996e;
            color: white;
            border-radius: 50%;
            padding: 2px 6px;
            font-size: 13px;
            position: absolute;
            top: -10px;
            right: -12px;
        }

        section {
            text-align: center;
            padding: 80px 20px;
            background-color: rgba(255, 255, 255, 0.9);
            margin: 40px;
            border-radius: 12px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        h1 {
            color: #3c2f2f;
            margin-bottom: 40px;
        }

        .menu-category {
            margin-bottom: 60px;
        }

        .menu-item {
            display: inline-block;
            width: 260px;
            margin: 15px;
            padding: 20px;
            background-color: #f1e3d3;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            vertical-align: top;
        }

        .menu-item img {
            border-radius: 10px;
            width: 200px;
            height: 190px;
        }

        .order-btn {
            display: inline-block;
            margin-top: 10px;
            padding: 10px 20px;
            background-color: #8a6e4b;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s;
            font-size: 14px;
            font-family: 'Georgia', serif;
        }

        .order-btn:hover {
            background-color: #b8996e;
        }

        .back-btn {
            display: inline-block;
            margin-top: 30px;
            padding: 12px 25px;
            background-color: #8a6e4b;
            color: white;
            border-radius: 8px;
            text-decoration: none;
            transition: background-color 0.3s;
        }

        .back-btn:hover {
            background-color: #b8996e;
        }

        footer {
            background-color: #e9dcc9;
            text-align: center;
            padding: 25px;
            color: #4b3f35;
        }

        /* ===== MODAL STYLES ===== */
        .modal {
            display: none;
            position: fixed;
            top: 0; left: 0; right: 0; bottom: 0;
            background: rgba(0,0,0,0.6);
            justify-content: center;
            align-items: center;
            z-index: 999;
        }

        .modal-content {
            background: #fffaf0;
            padding: 20px;
            border-radius: 12px;
            width: 350px;
            max-height: 80vh;
            overflow-y: auto;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
        }

        .modal-header {
            text-align: center;
            border-bottom: 2px solid #d6c4a1;
            margin-bottom: 10px;
        }

        .receipt-line {
            display: flex;
            justify-content: space-between;
            margin-bottom: 5px;
        }

        .controls {
            margin-top: 10px;
        }

        .checkout-btn, .close-btn {
            background: #8a6e4b;
            color: white;
            border: none;
            border-radius: 6px;
            padding: 8px 15px;
            margin-top: 10px;
            cursor: pointer;
        }

        .checkout-btn:hover, .close-btn:hover {
            background: #b8996e;
        }
    </style>
</head>
<body>

<header>
    <img src="https://uploads.onecompiler.io/43xg44j4q/444bsj7zz/LatteLibraryLogo.png" alt="The Latte Library Logo">
    <nav>
        <a href="file:///C:/Users/Acer/Desktop/Cruz,%20Paolo%20Gabriel/C++%20&%20HTML/group%204%20sample.html">Home</a>
        <a href="#coffee">Coffee</a>
        <a href="#frappe">Frappes</a>
        <a href="#pastries">Pastries</a>
        <a href="#Refreshers">Refreshers</a>
        <span class="cart-icon" title="View Cart" onclick="openReceipt()">🛒<span id="cartBadge">0</span></span>
    </nav>
</header>

<section id="coffee" class="menu-category">
    <h1>☕ Coffee Creations</h1>
    <div class="menu-item">
        <img src="https://uploads.onecompiler.io/43xg44j4q/444bsj7zz/HBRE_HotBrewedCoffee.jpg" alt="Hot Brewed Coffee">
        <h3>Hot Brewed Coffee</h3>
        <p>Swing by and warm up while enjoying any of our three roasts brewed daily</p>
		<p>150</p>
        <button class="order-btn" onclick="addItem('Hot Brewed Coffee',150)">Add to Order</button>
    </div>
    <div class="menu-item">
        <img src="https://uploads.onecompiler.io/43xg44j4q/444bsj7zz/CBRE_SaltedCaramelColdBrew.jpg" alt="Salted Caramel Cold Brew">
        <h3>Salted Caramel Cold Brew</h3>
        <p>Our Signature Starbucks Cold Brew flavored with salted caramel syrup, with a salted caramel flavored foam and drizzle of caramel syrup to finish the drink.</p>
		<p>140</p>
        <button class="order-btn" onclick="addItem('Salted Caramel Cold Brew',140)">Add to Order</button>
    </div>
    <div class="menu-item">
        <img src="https://uploads.onecompiler.io/43xg44j4q/444bsj7zz/CBRE_NitroVanillaSweetCreamColdBrew.jpg" alt="Nitro Vanilla Sweet Cream Cold Brew">
        <h3>Nitro Vanilla Sweet Cream Cold Brew</h3>
        <p>Served cold, straight from the tap, our Nitro Cold Brew is topped with a float of house-made vanilla sweet cream. The result: a cascade of velvety coffee that is more sippable than ever.</p>
		<p>130</p>
        <button class="order-btn" onclick="addItem('Nitro Vanilla Sweet Cream Cold Brew',130)">Add to Order</button>
    </div>
</section>

<section id="frappe" class="menu-category">
    <h1>🧊 Frappes & Iced Blends</h1>
    <div class="menu-item">
        <img src="https://uploads.onecompiler.io/43xg44j4q/43xg42p3j/FRAPCRE_GreenTeaCreamFrappuccino.jpg" alt="Pure Matcha Cream Frappuccino">
        <h3>Pure Matcha Cream Frappuccino</h3>
        <p>We blend sweetened premium matcha green tea, milk and ice and top it with sweetened whipped cream to give you a delicious boost of energy.</p>
		<p>150</p>
        <button class="order-btn" onclick="addItem('Pure Matcha Cream Frappuccino',150)">Add to Order</button>
    </div>
    <div class="menu-item">
        <img src="https://uploads.onecompiler.io/43xg44j4q/43xg42p3j/FRAPCRE_ChocolateCreamFrappuccino.jpg" alt="Chocolate Cream Frappuccino">
        <h3>Chocolate Cream Frappuccino</h3>
        <p>A rich and creamy blend of chocolate flavoured sauce, milk and ice. Topped with whipped cream.</p>
		<p>140</p>
        <button class="order-btn" onclick="addItem('Chocolate Cream Frappuccino',140)">Add to Order</button>
    </div>
    <div class="menu-item">
        <img src="https://uploads.onecompiler.io/43xg44j4q/43xg42p3j/FRAPCRE_StrawberriesandCreamFrappuccino.jpg" alt="Strawberries & Cream Frappuccino">
        <h3>Strawberries & Cream Frappuccino</h3>
        <p>Strawberries and milk are blended with ice and topped with a swirl of whipped cream. Sip on the crème of the crop.</p>
		<p>130</p>
        <button class="order-btn" onclick="addItem('Strawberries & Cream Frappuccino',130)">Add to Order</button>
    </div>
</section>

<section id="pastries" class="menu-category">
    <h1>🍰 Pastries & Desserts</h1>
    <div class="menu-item">
        <img src="https://uploads.onecompiler.io/43xg44j4q/444bsj7zz/Plant-BasedClassicLasagna.jpg" alt="Plant-Based Classic Lasagna">
        <h3>Plant-Based Classic Lasagna</h3>
        <p>This classic lasagna is the perfect Italian comfort food. Made with hearty plant-based ground patty Bolognese layered with plant based cheese and al-dente noodles.</p>
		<p>120</p>
        <button class="order-btn" onclick="addItem('Plant-Based Classic Lasagna',120)">Add to Order</button>
    </div>
    <div class="menu-item">
        <img src="https://uploads.onecompiler.io/43xg44j4q/444bsj7zz/BlueberryLiciousCheesecake.jpg" alt="Blueberry Licious Cheesecake">
        <h3>Blueberry Licious Cheesecake</h3>
        <p>A silken smooth, yet light cheesecake swirled with blueberries bursting with flavors. Finished with sweet-tangy blueberry compote. A refreshing dessert!</p>
		<p>180</p>
        <button class="order-btn" onclick="addItem('Blueberry Licious Cheesecake',180)">Add to Order</button>
    </div>
    <div class="menu-item">
        <img src="https://uploads.onecompiler.io/43xg44j4q/444bsj7zz/MNEJihQNNu9Bo0uJfv4CKLmE0BLiRQyVNW9gALg0.jpeg" alt="French Butter Croissant">
        <h3>French Butter Croissant</h3>
        <p>This croissant is pure pleasure. A beautiful golden color, crisp, moist and buttery, meltingly smooth, with a final note of caramel. It is made with 100% pure butter.
</p>
		<p>140</p>
        <button class="order-btn" onclick="addItem('French Butter Croissant',140)">Add to Order</button>
    </div>
</section>

<section id="Refreshers" class="menu-category">
    <h1>🍵 Refreshers</h1>
    <div class="menu-item">
        <img src="https://uploads.onecompiler.io/43xg44j4q/444bsj7zz/JcFQU4To3OtyYWJl6YulVXDPa5u2pc7CikwNVQuc.jpeg" alt="Strawberry Açaí with Lemonade">
        <h3>Strawberry Açaí with Lemonade</h3>
        <p>A combination of real fruit juice and flavors of sweet strawberry acai, with real strawberry slices and a pop of light energy boost balanced with delightful zing of lemonade..</p>
		<p>130</p>
        <button class="order-btn" onclick="addItem('Strawberry Açaí with Lemonade',130)">Add to Order</button>
    </div>
    <div class="menu-item">
        <img src="https://uploads.onecompiler.io/43xg44j4q/444bsj7zz/7bPOYfjrBAZ3PJFb6Pn0kOy1mVd1w3djqlD2YQ5P.jpeg" alt="Mango Dragonfruit with Lemonade">
        <h3>Mango Dragonfruit with Lemonade</h3>
        <p>This tropical-inspired Mango Dragonfruit has a clever combination of vibrant lemonade, sweet mango and refreshing dragonfruit flavors - with real fruit juice and real fruit pieces of Mango and Red Dragonfruit, giving you a pop of light energy boost, balanced with delightful zing of lemonade.</p>
		<p>120</p>
        <button class="order-btn" onclick="addItem('Mango Dragonfruit with Lemonade',120)">Add to Order</button>
    </div>
    <div class="menu-item">
        <img src="https://uploads.onecompiler.io/43xg44j4q/444bsj7zz/pz83LTYfwFhSpX1nIcKPgKdreaOCEuJijl1Xiz1P.jpeg" alt="Frozen Mango Dragonfruit Lemonade">
        <h3>Frozen Mango Dragonfruit Lemonade</h3>
        <p>The Frozen Mango Dragonfruit Lemonade and Frozen Dragon Drink from Starbucks Refreshers™ offer a vibrant mix of mango and dragonfruit flavors in a bright magenta, icy blend. Topped with freeze-dried fruit pieces for a tangy crunch, these tropical beverages are perfect summer pick-me-ups, available with either a refreshing lemonade base or a creamy coconut milk twist.</p>
		<p>110</p>
        <button class="order-btn" onclick="addItem('Frozen Mango Dragonfruit Lemonade',110)">Add to Order</button>
    </div>
</section>

<div style="text-align:center;">
    <a href="file:///C:/Users/Acer/Desktop/Cruz,%20Paolo%20Gabriel/C++%20&%20HTML/group%204%20sample.html" class="back-btn">← Back to Home</a>
</div>

<footer>
    <p>&copy; 2025 The Latte Library Coffee and Bookstore | All Rights Reserved</p>
</footer>

<!-- 🧾 RECEIPT MODAL -->
<div class="modal" id="receiptModal">
  <div class="modal-content">
    <div class="modal-header">
      <h3>🧾 LATTE LIBRARY</h3>
      <small>"TARA KAPE"</small>
    </div>
    <div class="receipt-body" id="receiptBody"></div>

    <div class="totals">
      Subtotal: ₱<span id="subtotal">0</span><br>
      Discount: ₱<span id="discount">0</span><br>
      Total: ₱<span id="grandTotal">0</span>
    </div>

    <div class="controls">
      <label>Discount:</label>
      <select id="discountType" onchange="updateTotals()">
        <option value="0">None</option>
        <option value="0.2">PWD (20%)</option>
        <option value="0.1">Senior (10%)</option>
      </select>

      <label>Payment Amount:</label>
      <input type="number" id="payment" oninput="computeChange()" placeholder="Enter payment...">

      <label>Change:</label>
      <input type="text" id="change" readonly>
    </div>

    <button class="checkout-btn" onclick="alertReceipt()">OK</button>
    <button class="close-btn" onclick="closeReceipt()">Close</button>
  </div>
</div>

<script>
let cart = [];
const cartBadge = document.getElementById('cartBadge');

function addItem(name, price) {
  const existing = cart.find(item => item.name === name);
  if (existing) existing.qty++;
  else cart.push({ name, price, qty: 1 });
  cartBadge.textContent = cart.reduce((a,b)=>a+b.qty,0);
}

function openReceipt() {
  renderReceipt();
  document.getElementById('receiptModal').style.display = 'flex';
}

function closeReceipt() {
  document.getElementById('receiptModal').style.display = 'none';
}

function renderReceipt() {
  const receiptBody = document.getElementById('receiptBody');
  receiptBody.innerHTML = '';
  let subtotal = 0;
  cart.forEach(item => {
    const total = item.price * item.qty;
    subtotal += total;
    const line = document.createElement('div');
    line.classList.add('receipt-line');
    line.innerHTML = `${item.qty} x ${item.name} <span>₱${total.toFixed(2)}</span>`;
    receiptBody.appendChild(line);
  });
  document.getElementById('subtotal').textContent = subtotal.toFixed(2);
  updateTotals();
}

function updateTotals() {
  const discountRate = parseFloat(document.getElementById('discountType').value);
  const subtotal = parseFloat(document.getElementById('subtotal').textContent);
  const discount = subtotal * discountRate;
  const grandTotal = subtotal - discount;

  document.getElementById('discount').textContent = discount.toFixed(2);
  document.getElementById('grandTotal').textContent = grandTotal.toFixed(2);

  computeChange();
}

function computeChange() {
  const payment = parseFloat(document.getElementById('payment').value) || 0;
  const total = parseFloat(document.getElementById('grandTotal').textContent);
  const change = payment - total;
  document.getElementById('change').value = change >= 0 ? change.toFixed(2) : '';
}

function alertReceipt() {
  let text = "============================\n";
  text += "      LATTE LIBRARY\n";
  text += "    'TARA KAPE'\n";
  text += "============================\n";
  cart.forEach(item => {
    text += `${item.qty} x ${item.name} = ₱${(item.price * item.qty).toFixed(2)}\n`;
  });
  text += "----------------------------\n";
  text += `Subtotal: ₱${document.getElementById('subtotal').textContent}\n`;
  text += `Discount: ₱${document.getElementById('discount').textContent}\n`;
  text += `Total: ₱${document.getElementById('grandTotal').textContent}\n`;
  text += `Payment: ₱${document.getElementById('payment').value}\n`;
  text += `Change: ₱${document.getElementById('change').value}\n`;
  text += "----------------------------\n";
  text += "SALAMAT PO! MARAMING SALAMAT!\n";
  alert(text);
}
</script>

</body>
</html>
