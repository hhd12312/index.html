<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>超人小家电</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>超人小家电</h1>
        <input type="text" id="search" placeholder="搜索产品...">
    </header>
    <div class="container">
        <div class="sidebar">
            <h3>分类</h3>
            <ul class="category-list" id="category-list">
                <!-- 动态生成 -->
            </ul>
        </div>
        <div class="main-content">
            <div class="image-grid" id="image-grid">
                <!-- 动态生成 -->
            </div>
            <div class="pagination" id="pagination">
                <!-- 动态生成 -->
            </div>
        </div>

        <!-- 购物车侧边详情面板（合并按钮与详情） -->
        <div id="cart-panel" class="cart-panel collapsed">
            <div class="cart-header">
                <h2>购物车详情 (<span id="cart-count">0</span>)</h2>
                <button class="close-cart" onclick="toggleCartPanel()">×</button>
            </div>
            <table class="cart-table">
                <thead>
                    <tr>
                        <th>产品</th>
                        <th>单价</th>
                        <th>盒数</th>
                        <th>总价</th>
                        <th>操作</th>
                    </tr>
                </thead>
                <tbody id="cart-table-body">
                </tbody>
            </table>
            <div class="cart-footer">
                <div class="total" id="cart-total">总计: ¥0</div>
                <button class="checkout-btn" onclick="checkout()">确认下单</button>
            </div>
        </div>
    </div>

    <script>
        // 产品数据（示例，替换为真实数据）
        const products = [
            // 在这里继续增加电池产品
            { id: 1, category: '电池', name: '南孚2粒装五号电池', price: 120, img: '图片/fPsod5ZvH.jpeg' },
            { id: 2, category: '电池', name: '南孚5粒装五号电池', price: 12, img: '图片/微信图片_20260403175257_98_65.jpg' },
            { id: 3, category: '电池', name: '南孚2粒装七号电池', price: 89, img: '' },
            { id: 4, category: '电池', name: '南孚5粒装七号电池', price: 8, img: 'https://via.placeholder.com/250x200?text=CR2032' },
            { id: 5, category: '电池', name: '南孚大号碱性电池', price: 40, img: 'https://via.placeholder.com/250x200?text=AA10' },
            { id: 6, category: '电池', name: '丰蓝大号1粒装电池', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 7, category: '电池', name: '丰蓝大号2粒装电池', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 8, category: '电池', name: '双鹿5号电池', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 9, category: '电池', name: '双鹿七号电池', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 10, category: '电池', name: '双鹿普通大号电池', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 11, category: '电池', name: '双鹿挂卡大号电池', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 12, category: '电池', name: '双鹿9v电池', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 13, category: '电池', name: '南孚传应电池2032', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 14, category: '电池', name: '南孚传应电池2450', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 15, category: '电池', name: '南孚传应电池1632', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 16, category: '电池', name: '南孚传应电池2016', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 17, category: '电池', name: '南孚传应电池27A', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 18, category: '电池', name: '南孚传应电池23A', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 19, category: '电池', name: '南孚纽扣电池CR1220', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 20, category: '电池', name: '南孚纽扣电池AG13', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 21, category: '电池', name: '奇劲5号电池', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 22, category: '电池', name: '奇劲7号电池', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
             { id: 23, category: '电池', name: '夜平安锂电池', price: 35, img: 'https://via.placeholder.com/250x200?text=AAA10' },
            // 在这里继续增加电池产品
        ];

        const categories = ['电池', '水杯', '水壶', '插座', '剃须刀', '吹风机', '灯泡', '小百货', '购物车'];

        // 自动补充其他类别示例产品
        categories.forEach(cat => {
            if (cat !== '电池') {
                for (let i = 1; i <= 30; i++) {
                    products.push({
                        id: products.length + 1,
                        category: cat,
                        name: `${cat}产品${i}`,
                        price: Math.floor(Math.random() * 400) + 30,
                        img: `https://via.placeholder.com/250x200?text=${encodeURIComponent(cat + i)}`
                    });
                }
            }
        });

        let currentCategory = 'all';
        let currentPage = 1;
        const itemsPerPage = 20;
        let filteredProducts = products;
        let cart = JSON.parse(localStorage.getItem('cart')) || [];

        // 渲染类别列表
        function renderCategories() {
            const categoryList = document.getElementById('category-list');
            categoryList.innerHTML = '<li data-category="all" class="active">全部</li>';
            categories.forEach(cat => {
                if (cat === '购物车') {
                    categoryList.innerHTML += `<li id="cart-category" data-category="${cat}" style="border-top: 2px solid #ddd; margin-top: 10px;" onclick="toggleCartPanel()">${cat}(<span id='cart-count-badge'>0</span>)</li>`;
                } else {
                    categoryList.innerHTML += `<li data-category="${cat}">${cat}</li>`;
                }
            });

            // 添加事件监听
            document.querySelectorAll('.category-list li').forEach(li => {
                if (li.dataset.category !== '购物车') {
                    li.addEventListener('click', () => {
                        document.querySelectorAll('.category-list li').forEach(l => l.classList.remove('active'));
                        li.classList.add('active');
                        currentCategory = li.dataset.category;
                        currentPage = 1;
                        filterAndRender();
                    });
                }
            });

            updateCartIndicator();
        }

        // 过滤产品
        function filterProducts() {
            if (currentCategory === 'all') {
                filteredProducts = products;
            } else {
                filteredProducts = products.filter(p => p.category === currentCategory);
            }

            const searchTerm = document.getElementById('search').value.toLowerCase();
            if (searchTerm) {
                filteredProducts = filteredProducts.filter(p => p.name.toLowerCase().includes(searchTerm));
            }
        }

        // 渲染产品
        function renderProducts() {
            const start = (currentPage - 1) * itemsPerPage;
            const end = start + itemsPerPage;
            const pageProducts = filteredProducts.slice(start, end);

            const imageGrid = document.getElementById('image-grid');
            imageGrid.innerHTML = '';
            pageProducts.forEach(product => {
                imageGrid.innerHTML += `
                    <div class="image-item">
                        <img src="${product.img}" alt="${product.name}">
                        <div class="info">
                            <div class="name">${product.name}</div>
                            <div class="amount">¥${product.price}</div>
                            <div class="quantity-container">
                                <label>盒数:</label>
                                <input type="number" min="1" value="1" id="qty-${product.id}">
                            </div>
                            <button class="add-to-cart" onclick="addToCart(${product.id})">加入购物车</button>
                        </div>
                    </div>
                `;
            });
        }

        // 渲染分页
        function renderPagination() {
            const totalPages = Math.ceil(filteredProducts.length / itemsPerPage);
            const pagination = document.getElementById('pagination');
            pagination.innerHTML = '';

            if (totalPages <= 1) return;

            for (let i = 1; i <= totalPages; i++) {
                pagination.innerHTML += `<button class="${i === currentPage ? 'active' : ''}" data-page="${i}">${i}</button>`;
            }

            // 添加事件监听
            document.querySelectorAll('.pagination button').forEach(btn => {
                btn.addEventListener('click', () => {
                    currentPage = parseInt(btn.dataset.page);
                    renderProducts();
                    renderPagination();
                });
            });
        }

        // 过滤并渲染
        function filterAndRender() {
            filterProducts();
            renderProducts();
            renderPagination();
        }

        // 加入购物车
        function addToCart(productId) {
            const qty = parseInt(document.getElementById(`qty-${productId}`).value);
            const product = products.find(p => p.id === productId);
            const existing = cart.find(item => item.id === productId);
            if (existing) {
                existing.quantity += qty;
            } else {
                cart.push({ ...product, quantity: qty });
            }
            localStorage.setItem('cart', JSON.stringify(cart));
            alert('已加入购物车！');
            updateCartIndicator();
            renderCart();
        }

        // 渲染购物车面板内容
        function renderCart() {
            const tableBody = document.getElementById('cart-table-body');
            const totalDiv = document.getElementById('cart-total');
            const cartCount = document.getElementById('cart-count');
            const cartBadge = document.getElementById('cart-count-badge');

            tableBody.innerHTML = cart.map((item, index) => `
                <tr>
                    <td>${item.name}</td>
                    <td>¥${item.price}</td>
                    <td><input type="number" class="qty-input" value="${item.quantity}" min="1" onchange="updateQuantity(${index}, this.value)"></td>
                    <td>¥${item.price * item.quantity}</td>
                    <td><button class="remove-btn" onclick="removeFromCart(${index})">删除</button></td>
                </tr>
            `).join('');

            const total = cart.reduce((sum, item) => sum + item.price * item.quantity, 0);
            totalDiv.innerText = `总计: ¥${total}`;
            cartCount.innerText = cart.reduce((sum, item) => sum + item.quantity, 0);
            if (cartBadge) cartBadge.innerText = cartCount.innerText;

            updateCartIndicator();
        }

        // 展开/收起购物车面板
        function toggleCartPanel(forceShow) {
            const panel = document.getElementById('cart-panel');
            const isHidden = panel.classList.contains('collapsed');
            if (forceShow === true || (forceShow === undefined && isHidden)) {
                panel.classList.remove('collapsed');
            } else {
                panel.classList.add('collapsed');
            }
            renderCart();
        }

        // 更新购物车数量提示
        function updateCartIndicator() {
            const totalItems = cart.reduce((sum, item) => sum + item.quantity, 0);
            const badge = document.getElementById('cart-count-badge');
            const headerCount = document.getElementById('cart-count');
            if (badge) badge.innerText = totalItems;
            if (headerCount) headerCount.innerText = totalItems;
            const cartCat = document.getElementById('cart-category');
            if (cartCat) cartCat.innerText = `购物车(${totalItems})`;
        }

        // 更新数量
        function updateQuantity(index, newQty) {
            newQty = parseInt(newQty);
            if (newQty < 1) newQty = 1;
            cart[index].quantity = newQty;
            localStorage.setItem('cart', JSON.stringify(cart));
            renderCart();
        }

        // 删除商品
        function removeFromCart(index) {
            cart.splice(index, 1);
            localStorage.setItem('cart', JSON.stringify(cart));
            renderCart();
        }

        // 下单
        function checkout() {
            if (cart.length === 0) {
                alert('购物车为空！');
                return;
            }
            const total = cart.reduce((sum, item) => sum + item.price * item.quantity, 0);
            alert(`总价: ¥${total}\n模拟下单成功！`);
            cart = [];
            localStorage.removeItem('cart');
            renderCart();
        }

        // 搜索事件
        document.getElementById('search').addEventListener('input', () => {
            currentPage = 1;
            filterAndRender();
        });

        // 初始化
        renderCategories();
        filterAndRender();
        renderCart();
        updateCartIndicator();
    </script>
</body>
</html>
