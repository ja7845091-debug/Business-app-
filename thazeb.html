<!DOCTYPE html>
<html lang="ur">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tehzeeb Bakers - Official Menu</title>
    <style>
        /* --- DESIGN SETTINGS --- */
        body { font-family: 'Segoe UI', sans-serif; margin: 0; padding: 0; background-color: #f8f9fa; padding-bottom: 100px; }
        
        /* Header */
        .header { background: #b30000; color: white; padding: 20px; text-align: center; position: sticky; top: 0; z-index: 100; box-shadow: 0 2px 10px rgba(0,0,0,0.2); }
        .header h1 { margin: 0; font-size: 24px; }
        .header p { margin: 5px 0 0; font-size: 13px; opacity: 0.9; }

        /* Search Bar */
        .search-container { padding: 15px; background: white; border-bottom: 1px solid #ddd; }
        .search-box { width: 100%; padding: 12px; border: 1px solid #ccc; border-radius: 8px; font-size: 16px; box-sizing: border-box; }

        /* Categories */
        .categories { display: flex; overflow-x: auto; padding: 10px; background: white; gap: 10px; white-space: nowrap; -webkit-overflow-scrolling: touch; }
        .cat-btn { padding: 8px 15px; border: 1px solid #b30000; border-radius: 20px; background: white; color: #b30000; font-weight: bold; cursor: pointer; }
        .cat-btn.active { background: #b30000; color: white; }

        /* Grid Layout */
        .container { padding: 15px; display: grid; grid-template-columns: 1fr 1fr; gap: 15px; }
        @media (min-width: 600px) { .container { grid-template-columns: 1fr 1fr 1fr; } }

        /* Item Card */
        .item-card { background: white; border-radius: 12px; overflow: hidden; box-shadow: 0 4px 10px rgba(0,0,0,0.05); display: flex; flex-direction: column; border: 1px solid #eee; }
        .item-image { width: 100%; height: 120px; object-fit: cover; background: #eee; }
        .card-content { padding: 10px; flex-grow: 1; display: flex; flex-direction: column; justify-content: space-between; }
        .item-name { font-weight: bold; font-size: 15px; color: #333; margin-bottom: 5px; height: 40px; overflow: hidden; }
        .item-price { color: #b30000; font-weight: bold; font-size: 16px; margin-bottom: 8px; }
        
        .add-btn { background: #f0f0f0; color: #333; border: none; padding: 10px; border-radius: 5px; font-weight: bold; width: 100%; cursor: pointer; transition: 0.2s; }
        .add-btn.added { background: #b30000; color: white; }

        /* Floating Cart */
        .cart-bar { position: fixed; bottom: 0; left: 0; right: 0; background: white; padding: 15px; box-shadow: 0 -5px 20px rgba(0,0,0,0.1); display: flex; justify-content: space-between; align-items: center; z-index: 1000; border-top: 1px solid #eee; display: none; }
        .total-text { font-size: 16px; font-weight: bold; }
        .order-now-btn { background-color: #25D366; color: white; border: none; padding: 12px 20px; border-radius: 25px; font-weight: bold; cursor: pointer; font-size: 16px; }

        /* Checkout Modal */
        .modal-overlay { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.6); z-index: 2000; }
        .modal-content { position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); background: white; padding: 20px; border-radius: 15px; width: 90%; max-width: 400px; box-shadow: 0 10px 30px rgba(0,0,0,0.2); }
        .modal-title { font-size: 20px; font-weight: bold; margin-bottom: 15px; color: #b30000; border-bottom: 1px solid #eee; padding-bottom: 10px; }
        .form-group { margin-bottom: 15px; }
        .form-group label { display: block; font-weight: bold; margin-bottom: 5px; font-size: 14px; color: #333; }
        .form-control { width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 5px; box-sizing: border-box; font-size: 15px; }
        
        .submit-btn { background: #25D366; color: white; width: 100%; padding: 12px; border: none; border-radius: 5px; font-weight: bold; font-size: 16px; cursor: pointer; margin-top: 10px; }
        .close-btn { background: #ccc; color: #333; width: 100%; padding: 10px; border: none; border-radius: 5px; font-weight: bold; font-size: 15px; cursor: pointer; margin-top: 10px; }
    </style>
</head>
<body>

    <div class="header">
        <h1>Tehzeeb Bakers</h1>
        <p>A Culinary Legacy of 113 Years</p>
    </div>

    <div class="search-container">
        <input type="text" id="search-box" class="search-box" placeholder="Search Pizza, Cake, Sweets..." onkeyup="filterItems()">
    </div>

    <div class="categories">
        <button class="cat-btn active" onclick="filterCategory('all', this)">All</button>
        <button class="cat-btn" onclick="filterCategory('pizza', this)">Pizzas</button>
        <button class="cat-btn" onclick="filterCategory('cake', this)">Cakes</button>
        <button class="cat-btn" onclick="filterCategory('sweets', this)">Sweets</button>
        <button class="cat-btn" onclick="filterCategory('fastfood', this)">Fast Food</button>
        <button class="cat-btn" onclick="filterCategory('bakery', this)">Bakery</button>
        <button class="cat-btn" onclick="filterCategory('nimco', this)">Nimco</button>
    </div>

    <div class="container" id="menu-container">
    </div>

    <div class="cart-bar" id="cart-bar">
        <div class="total-text">
            Total: Rs. <span id="total-price">0</span>
            <div style="font-size: 12px; color: #666;">(<span id="item-count">0</span> items)</div>
        </div>
        <button onclick="openCheckout()" class="order-now-btn">Order Now </button>
    </div>

    <div class="modal-overlay" id="checkout-modal">
        <div class="modal-content">
            <div class="modal-title">Complete Your Order</div>
            
            <div class="form-group">
                <label>Your Name</label>
                <input type="text" id="cust-name" class="form-control" placeholder="Enter your name">
            </div>

            <div class="form-group">
                <label>Select Branch</label>
                <select id="cust-branch" class="form-control">
                    <option value="Rawalpindi Saddar">Rawalpindi Saddar</option>
                    <option value="Chaklala Scheme 3">Chaklala Scheme 3</option>
                    <option value="Bahria Town RWP">Bahria Town RWP</option>
                    <option value="Blue Area Islamabad">Blue Area Islamabad</option>
                    <option value="G-9 Markaz Islamabad">G-9 Markaz Islamabad</option>
                    <option value="F-11 Markaz Islamabad">F-11 Markaz Islamabad</option>
                    <option value="M.M. Alam Road Lahore">M.M. Alam Road Lahore</option>
                </select>
            </div>

            <div class="form-group">
                <label>Payment Method</label>
                <select id="cust-payment" class="form-control">
                    <option value="Easypaisa">Easypaisa</option>
                    <option value="JazzCash">JazzCash</option>
                    <option value="Bank Account">Bank Account Transfer</option>
                    <option value="Cash on Delivery">Cash on Delivery</option>
                </select>
            </div>

            <button class="submit-btn" onclick="sendToWhatsapp()">Confirm & Send Order</button>
            <button class="close-btn" onclick="closeCheckout()">Cancel</button>
        </div>
    </div>

    <script>
        // === OFFICIAL BAKERY NUMBER ===
        const bakeryNumber = "923000507425"; // Tehzeeb Bakers official number 

        // === ALL ITEMS DATABASE ===
        const allItems = [
            // PIZZAS
            { id: 1, name: "Chicken Tikka Pizza (L)", category: "pizza", price: 1850, img: "https://images.unsplash.com/photo-1565299624946-b28f40a0ae38?w=400" },
            { id: 2, name: "Chicken Fajita Pizza (L)", category: "pizza", price: 1850, img: "https://images.unsplash.com/photo-1513104890138-7c749659a591?w=400" },
            { id: 3, name: "Tehzeeb Special Pizza", category: "pizza", price: 2100, img: "https://images.unsplash.com/photo-1604382354936-07c5d9983bd3?w=400" },

            // CAKES
            { id: 5, name: "Black Forest Cake (2lbs)", category: "cake", price: 2200, img: "https://images.unsplash.com/photo-1578985545062-69928b1d9587?w=400" },
            { id: 6, name: "Pineapple Cake (2lbs)", category: "cake", price: 2000, img: "https://images.unsplash.com/photo-1535141192574-5d4897c12636?w=400" },
            { id: 7, name: "Chocolate Fudge Cake", category: "cake", price: 2500, img: "https://images.unsplash.com/photo-1571115177098-24ec42ed204d?w=400" },

            // SWEETS (Mitai)
            { id: 20, name: "Mix Sweets (1kg)", category: "sweets", price: 1500, img: "https://images.unsplash.com/photo-1589115794711-6670868eb370?w=400" },
            { id: 21, name: "Gulab Jamun (1kg)", category: "sweets", price: 1400, img: "https://images.unsplash.com/photo-1558961363-fa8fdf82db35?w=400" },
            { id: 22, name: "Baklava (Special Box)", category: "sweets", price: 2800, img: "https://images.unsplash.com/photo-1595928642581-f50f4f3453a5?w=400" },

            // FAST FOOD
            { id: 10, name: "Zinger Burger", category: "fastfood", price: 450, img: "https://images.unsplash.com/photo-1568901346375-23c9450c58cd?w=400" },
            { id: 11, name: "Chicken Sandwich", category: "fastfood", price: 350, img: "https://images.unsplash.com/photo-1521305916504-4a1121188589?w=400" },
            { id: 13, name: "Chicken Patties (Doz)", category: "fastfood", price: 600, img: "https://images.unsplash.com/photo-1619250907534-1188613149ba?w=400" },

            // BAKERY
            { id: 14, name: "Special Biscuits (1kg)", category: "bakery", price: 1200, img: "https://images.unsplash.com/photo-1558961363-fa8fdf82db35?w=400" },
            { id: 15, name: "Plain Bread (Large)", category: "bakery", price: 220, img: "https://images.unsplash.com/photo-1598373182133-52452f7691ef?w=400" },
            { id: 18, name: "Cake Rusk (Packet)", category: "bakery", price: 350, img: "https://images.unsplash.com/photo-1589115794711-6670868eb370?w=400" },

            // NIMCO
            { id: 30, name: "Mix Nimco (500g)", category: "nimco", price: 400, img: "https://images.unsplash.com/photo-1604382354936-07c5d9983bd3?w=400" },
            { id: 31, name: "Spicy Daal Sev", category: "nimco", price: 350, img: "https://images.unsplash.com/photo-1558961363-fa8fdf82db35?w=400" }
        ];

        let cart = {}; 
        let currentTotal = 0;

        // --- RENDER MENU ---
        function renderMenu(itemsToRender) {
            const container = document.getElementById('menu-container');
            container.innerHTML = '';
            
            itemsToRender.forEach(item => {
                const qty = cart[item.name] ? cart[item.name].qty : 0;
                const btnClass = qty > 0 ? 'add-btn added' : 'add-btn';
                const btnText = qty > 0 ? `Order Now (${qty})` : 'Order Now';

                container.innerHTML += `
                    <div class="item-card">
                        <img src="${item.img}" class="item-image" alt="${item.name}">
                        <div class="card-content">
                            <div class="item-name">${item.name}</div>
                            <div class="item-price">Rs. ${item.price}</div>
                            <button id="btn-${item.id}" class="${btnClass}" onclick="addToCart(${item.id})">${btnText}</button>
                        </div>
                    </div>
                `;
            });
        }

        // --- FILTER CATEGORIES ---
        function filterCategory(cat, btn) {
            document.querySelectorAll('.cat-btn').forEach(b => b.classList.remove('active'));
            btn.classList.add('active');

            if (cat === 'all') {
                renderMenu(allItems);
            } else {
                const filtered = allItems.filter(item => item.category === cat);
                renderMenu(filtered);
            }
        }

        // --- SEARCH ---
        function filterItems() {
            const query = document.getElementById('search-box').value.toLowerCase();
            const filtered = allItems.filter(item => item.name.toLowerCase().includes(query));
            renderMenu(filtered);
        }

        // --- CART LOGIC ---
        function addToCart(id) {
            const item = allItems.find(i => i.id === id);
            
            if (cart[item.name]) {
                cart[item.name].qty += 1;
            } else {
                cart[item.name] = { price: item.price, qty: 1 };
            }

            updateCartUI();
            
            const btn = document.getElementById(`btn-${id}`);
            if(btn) {
                btn.innerHTML = `Order Now (${cart[item.name].qty})`;
                btn.classList.add('added');
            }
        }

        function updateCartUI() {
            let total = 0;
            let count = 0;
            for (let key in cart) {
                total += cart[key].price * cart[key].qty;
                count += cart[key].qty;
            }
            currentTotal = total;

            document.getElementById('total-price').innerText = total;
            document.getElementById('item-count').innerText = count;

            const bar = document.getElementById('cart-bar');
            if (count > 0) bar.style.display = 'flex';
        }

        // --- MODAL CONTROLS ---
        function openCheckout() {
            document.getElementById('checkout-modal').style.display = 'block';
        }

        function closeCheckout() {
            document.getElementById('checkout-modal').style.display = 'none';
        }

        // --- SEND TO WHATSAPP FINAL ---
        function sendToWhatsapp() {
            if (Object.keys(cart).length === 0) return;

            const name = document.getElementById('cust-name').value;
            const branch = document.getElementById('cust-branch').value;
            const payment = document.getElementById('cust-payment').value;

            if (name.trim() === "") {
                alert("Please enter your name!");
                return;
            }

            let message = `*NEW ORDER - Tehzeeb Bakers*%0A%0A`;
            message += `👤 *Customer Name:* ${name}%0A`;
            message += `🏪 *Branch Selected:* ${branch}%0A`;
            message += `💳 *Payment Method:* ${payment}%0A%0A`;
            message += `*--- Order Details ---*%0A`;

            for (const [itemName, details] of Object.entries(cart)) {
                let itemTotal = details.price * details.qty;
                message += `▪️ ${itemName} (x${details.qty}) - Rs. ${itemTotal}%0A`;
            }

            message += `%0A💰 *Total Bill: Rs. ${currentTotal}*%0A`;
            message += `%0A📍 Please reply with payment details or confirmation.`;

            const url = `https://wa.me/${bakeryNumber}?text=${message}`;
            window.open(url, '_blank');
            closeCheckout();
        }

        // Initialize App
        renderMenu(allItems);
    </script>
</body>
</html>
