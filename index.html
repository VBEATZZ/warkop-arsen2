<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Warkop Arsen - Kasir & Order</title>
    <!-- Tailwind CSS untuk Tampilan Modern & Simpel -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body { background-color: #0f172a; color: #f8fafc; font-family: sans-serif; }
    </style>
</head>
<body class="min-h-screen pb-20">

    <!-- Navbar -->
    <nav class="bg-slate-900 border-b border-slate-800 p-4 sticky top-0 z-40 shadow-lg">
        <div class="max-w-6xl mx-auto flex justify-between items-center">
            <div class="flex items-center space-x-3">
                <i class="fa-solid fa-mug-hot text-amber-500 text-2xl"></i>
                <h1 class="text-xl font-bold text-amber-500 tracking-wide">Warkop Arsen</h1>
            </div>
            <div>
                <button id="authBtn" onclick="openLoginModal()" class="bg-amber-500 hover:bg-amber-600 text-slate-950 px-4 py-2 rounded-lg font-bold text-sm transition">
                    <i class="fa-solid fa-user-gear mr-2"></i>Login Owner
                </button>
            </div>
        </div>
    </nav>

    <!-- Main Content -->
    <div class="max-w-6xl mx-auto p-4 md:p-6 grid grid-cols-1 lg:grid-cols-3 gap-6">

        <!-- Menu Section (2 Cols) -->
        <div class="lg:col-span-2">
            <div class="mb-6 flex justify-between items-center">
                <h2 class="text-2xl font-bold text-slate-100">Daftar Menu</h2>
                <span id="roleBadge" class="bg-slate-800 text-amber-400 border border-amber-500/30 text-xs px-3 py-1 rounded-full">Mode: Customer</span>
            </div>

            <!-- Grid Menu -->
            <div id="menuContainer" class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                <!-- Menu Items injected by JavaScript -->
            </div>
        </div>

        <!-- Order / Cart Section (1 Col) -->
        <div class="lg:col-span-1">
            <div class="bg-slate-900 border border-slate-800 rounded-2xl p-5 sticky top-24 shadow-xl">
                <h3 class="text-lg font-bold border-b border-slate-800 pb-3 mb-4 flex items-center justify-between">
                    <span><i class="fa-solid fa-cart-shopping text-amber-500 mr-2"></i>Pesanan</span>
                    <button onclick="clearCart()" class="text-xs text-rose-400 hover:underline">Reset</button>
                </h3>

                <div id="cartItems" class="space-y-3 max-h-60 overflow-y-auto pr-1 mb-4">
                    <p class="text-slate-500 text-sm text-center py-4">Belum ada menu yang dipilih.</p>
                </div>

                <div class="border-t border-slate-800 pt-3 space-y-2 text-sm">
                    <div class="flex justify-between text-slate-400">
                        <span>Total Item:</span>
                        <span id="totalItems">0</span>
                    </div>
                    <div class="flex justify-between font-bold text-lg text-amber-400 pt-1 border-t border-slate-800">
                        <span>Total Bayar:</span>
                        <span id="totalPrice">Rp 0</span>
                    </div>
                </div>

                <!-- Fitur Pembayaran / Checkout -->
                <button onclick="processOrder()" class="w-full mt-5 bg-emerald-600 hover:bg-emerald-500 text-white font-bold py-3 rounded-xl shadow-lg transition">
                    <i class="fa-solid fa-paper-plane mr-2"></i>Proses Pesanan
                </button>
            </div>
        </div>
    </div>

    <!-- Owner Dashboard Modal (Khusus Owner) -->
    <div id="ownerPanel" class="hidden fixed inset-0 bg-black/80 backdrop-blur-sm z-50 flex items-center justify-center p-4">
        <div class="bg-slate-900 border border-slate-800 rounded-2xl w-full max-w-2xl p-6 relative max-h-[90vh] overflow-y-auto">
            <button onclick="closeOwnerPanel()" class="absolute top-4 right-4 text-slate-400 hover:text-white">
                <i class="fa-solid fa-xmark text-xl"></i>
            </button>
            <h2 class="text-xl font-bold text-amber-500 mb-4 flex items-center">
                <i class="fa-solid fa-chart-line mr-2"></i>Panel Ringkasan Penjualan (Owner)
            </h2>
            
            <div class="grid grid-cols-2 gap-4 mb-6">
                <div class="bg-slate-800 p-4 rounded-xl border border-slate-700">
                    <span class="text-xs text-slate-400">Total Transaksi</span>
                    <p id="ownerTotalOrders" class="text-2xl font-bold text-amber-400">0</p>
                </div>
                <div class="bg-slate-800 p-4 rounded-xl border border-slate-700">
                    <span class="text-xs text-slate-400">Total Pemasukan</span>
                    <p id="ownerTotalRevenue" class="text-2xl font-bold text-emerald-400">Rp 0</p>
                </div>
            </div>

            <h3 class="font-bold text-slate-200 mb-2">Riwayat Transaksi</h3>
            <div id="historyList" class="space-y-2 max-h-48 overflow-y-auto">
                <p class="text-xs text-slate-500">Belum ada riwayat transaksi.</p>
            </div>

            <button onclick="logoutOwner()" class="w-full mt-6 bg-rose-600 hover:bg-rose-500 text-white font-bold py-2 rounded-xl transition">
                Logout Owner
            </button>
        </div>
    </div>

    <!-- Login Modal -->
    <div id="loginModal" class="hidden fixed inset-0 bg-black/80 backdrop-blur-sm z-50 flex items-center justify-center p-4">
        <div class="bg-slate-900 border border-slate-800 rounded-2xl w-full max-w-md p-6 relative">
            <button onclick="closeLoginModal()" class="absolute top-4 right-4 text-slate-400 hover:text-white">
                <i class="fa-solid fa-xmark text-xl"></i>
            </button>
            <h2 class="text-xl font-bold text-amber-500 mb-4 text-center">Login Khusus Owner</h2>
            
            <form onsubmit="handleLogin(event)" class="space-y-4">
                <div>
                    <label class="text-xs text-slate-400 block mb-1">Username</label>
                    <input type="text" id="username" required class="w-full bg-slate-800 border border-slate-700 rounded-lg px-3 py-2 text-white focus:outline-none focus:border-amber-500">
                </div>
                <div>
                    <label class="text-xs text-slate-400 block mb-1">Password</label>
                    <input type="password" id="password" required class="w-full bg-slate-800 border border-slate-700 rounded-lg px-3 py-2 text-white focus:outline-none focus:border-amber-500">
                </div>
                <p id="loginError" class="text-rose-500 text-xs hidden">Username atau Password salah!</p>
                <button type="submit" class="w-full bg-amber-500 hover:bg-amber-600 text-slate-950 font-bold py-2 rounded-lg transition">
                    Masuk
                </button>
            </form>
        </div>
    </div>

    <!-- JavaScript Logic -->
    <script>
        // Data Menu Lengkap Warkop Arsen
        const menus = [
            { id: 1, name: 'Pop Ice', price: 5000, desc: 'Es blender segar manis khas nongkrong', flavor: 'Cokelat, Taro, Strawberry, Mangga, Alpukat, Permen Karet' },
            { id: 2, name: 'Kopi Hitam / Tubruk', price: 5000, desc: 'Kopi racikan khas warkop mantap dan pekat', flavor: 'Pahit Mantap / Manis Sedang' },
            { id: 3, name: 'Es Teh Manis', price: 5000, desc: 'Teh seduh segar dingin pelepas dahaga', flavor: 'Manis Dingin' },
            { id: 4, name: 'Teh Hangat', price: 3000, desc: 'Teh manis hangat cocok untuk santai', flavor: 'Hangat Manis' },
            { id: 5, name: 'Nutrisari', price: 5000, desc: 'Minuman sari buah kaya vitamin C', flavor: 'Jeruk Peras, Mangga, Florida Orange, Sweet Guava' },
            { id: 6, name: 'Good Day', price: 6000, desc: 'Kopi instan kekinian dingin / hangat', flavor: 'Mocacinno, Coolin, Vanilla Latte, Freeze' },
            { id: 7, name: 'Beng Beng Drink', price: 6000, desc: 'Minuman cokelat kaya rasa dengan kelezatan khas Beng-Beng', flavor: 'Cokelat Creamy' },
            { id: 8, name: 'Milo', price: 6000, desc: 'Minuman cokelat malt bernutrisi tinggi', flavor: 'Cokelat Malt' },
            { id: 9, name: 'Tora Moka', price: 5000, desc: 'Kopi moka paduan cokelat dan kopi', flavor: 'Moka Creamy' },
            { id: 10, name: 'ABC Susu', price: 5000, desc: 'Perpaduan kopi hitam dan susu manis gurih', flavor: 'Kopi Susu' },
            { id: 11, name: 'Kopi Hitam ABC / Item', price: 5000, desc: 'Kopi hitam instan aroma khas', flavor: 'Pahit Sedang' },
            { id: 12, name: 'White Koffie', price: 5000, desc: 'Kopi putih nikmat, aman di lambung', flavor: 'Krimy Lembut' },
            { id: 13, name: 'Wedang Jahe', price: 5000, desc: 'Minuman jahe hangat penambah stamina tubuh', flavor: 'Pedas Hangat Alami' },
            { id: 14, name: 'Air Putih', price: 3000, desc: 'Air mineral kemasan dingin/biasa', flavor: 'Netral' },
            { id: 15, name: 'Es Batu (Extra)', price: 2000, desc: 'Tambahan es batu segar', flavor: 'Dingin' },
            { id: 16, name: 'Indomie Single', price: 5000, desc: 'Mie instan goreng/kuah hangat mantap', flavor: 'Goreng, Kuah Soto, Ayam Bawang' }
        ];

        let cart = [];
        let isOwner = false;
        let totalSales = 0;
        let totalOrdersCount = 0;
        let orderHistory = [];

        // Render Menu ke UI
        function renderMenu() {
            const container = document.getElementById('menuContainer');
            container.innerHTML = '';

            menus.forEach(item => {
                container.innerHTML += `
                    <div class="bg-slate-900 border border-slate-800 rounded-xl p-4 flex flex-col justify-between hover:border-amber-500/50 transition shadow-md">
                        <div>
                            <div class="flex justify-between items-start mb-2">
                                <h3 class="font-bold text-amber-400 text-lg">${item.name}</h3>
                                <span class="text-sm font-semibold bg-slate-800 text-slate-200 px-2.5 py-1 rounded-md">Rp ${item.price.toLocaleString()}</span>
                            </div>
                            <p class="text-xs text-slate-400 mb-1">${item.desc}</p>
                            <span class="inline-block text-[10px] bg-slate-800 text-amber-500/80 px-2 py-0.5 rounded border border-amber-500/20 mb-3">
                                <i class="fa-solid fa-tag mr-1"></i>Varian/Rasa: ${item.flavor}
                            </span>
                        </div>
                        <button onclick="addToCart(${item.id})" class="w-full bg-slate-800 hover:bg-amber-500 hover:text-slate-950 text-slate-200 text-xs font-bold py-2 rounded-lg transition">
                            + Tambah ke Pesanan
                        </button>
                    </div>
                `;
            });
        }

        // Tambah ke Keranjang
        function addToCart(id) {
            const item = menus.find(m => m.id === id);
            const existing = cart.find(c => c.id === id);

            if (existing) {
                existing.qty += 1;
            } else {
                cart.push({ ...item, qty: 1 });
            }
            updateCart();
        }

        // Update Tampilan Keranjang
        function updateCart() {
            const cartItems = document.getElementById('cartItems');
            const totalPrice = document.getElementById('totalPrice');
            const totalItems = document.getElementById('totalItems');

            if (cart.length === 0) {
                cartItems.innerHTML = `<p class="text-slate-500 text-sm text-center py-4">Belum ada menu yang dipilih.</p>`;
                totalPrice.innerText = 'Rp 0';
                totalItems.innerText = '0';
                return;
            }

            cartItems.innerHTML = '';
            let total = 0;
            let count = 0;

            cart.forEach(item => {
                total += item.price * item.qty;
                count += item.qty;
                cartItems.innerHTML += `
                    <div class="flex justify-between items-center bg-slate-800/60 p-2.5 rounded-lg border border-slate-700/50 text-sm">
                        <div class="truncate max-w-[120px]">
                            <p class="font-semibold text-slate-200">${item.name}</p>
                            <p class="text-xs text-slate-400">Rp ${item.price.toLocaleString()}</p>
                        </div>
                        <div class="flex items-center space-x-2">
                            <button onclick="changeQty(${item.id}, -1)" class="w-6 h-6 bg-slate-700 hover:bg-slate-600 rounded text-xs font-bold">-</button>
                            <span class="text-xs font-bold w-4 text-center">${item.qty}</span>
                            <button onclick="changeQty(${item.id}, 1)" class="w-6 h-6 bg-slate-700 hover:bg-slate-600 rounded text-xs font-bold">+</button>
                        </div>
                    </div>
                `;
            });

            totalPrice.innerText = `Rp ${total.toLocaleString()}`;
            totalItems.innerText = count;
        }

        // Ubah Jumlah Item
        function changeQty(id, change) {
            const item = cart.find(c => c.id === id);
            if (item) {
                item.qty += change;
                if (item.qty <= 0) {
                    cart = cart.filter(c => c.id !== id);
                }
            }
            updateCart();
        }

        // Reset Keranjang
        function clearCart() {
            cart = [];
            updateCart();
        }

        // Proses Transaksi
        function processOrder() {
            if (cart.length === 0) {
                alert('Pilih menu terlebih dahulu!');
                return;
            }

            const total = cart.reduce((sum, item) => sum + (item.price * item.qty), 0);
            totalSales += total;
            totalOrdersCount += 1;

            orderHistory.push({
                id: totalOrdersCount,
                time: new Date().toLocaleTimeString(),
                total: total,
                items: [...cart]
            });

            alert(`Pesanan Berhasil Diproses!\nTotal Bayar: Rp ${total.toLocaleString()}`);
            clearCart();
            updateOwnerStats();
        }

        // Update Statistik Owner
        function updateOwnerStats() {
            document.getElementById('ownerTotalOrders').innerText = totalOrdersCount;
            document.getElementById('ownerTotalRevenue').innerText = `Rp ${totalSales.toLocaleString()}`;
            
            const historyList = document.getElementById('historyList');
            if (orderHistory.length > 0) {
                historyList.innerHTML = '';
                orderHistory.slice().reverse().forEach(ord => {
                    historyList.innerHTML += `
                        <div class="bg-slate-800 p-2.5 rounded-lg border border-slate-700 text-xs flex justify-between items-center">
                            <div>
                                <span class="font-bold text-amber-400">#${ord.id}</span> - <span class="text-slate-400">${ord.time}</span>
                            </div>
                            <span class="font-bold text-emerald-400">Rp ${ord.total.toLocaleString()}</span>
                        </div>
                    `;
                });
            }
        }

        // Auth & Modal Functions
        function openLoginModal() {
            if (isOwner) {
                document.getElementById('ownerPanel').classList.remove('hidden');
            } else {
                document.getElementById('loginModal').classList.remove('hidden');
            }
        }

        function closeLoginModal() {
            document.getElementById('loginModal').classList.add('hidden');
            document.getElementById('loginError').classList.add('hidden');
        }

        function closeOwnerPanel() {
            document.getElementById('ownerPanel').classList.add('hidden');
        }

        function handleLogin(e) {
            e.preventDefault();
            const usn = document.getElementById('username').value;
            const pw = document.getElementById('password').value;

            // Kredensial khusus Owner
            if (usn === 'warkop arsen' && pw === 'warkoparsen') {
                isOwner = true;
                closeLoginModal();
                document.getElementById('roleBadge').innerText = 'Mode: Owner';
                document.getElementById('roleBadge').className = 'bg-amber-500/20 text-amber-400 border border-amber-500 text-xs px-3 py-1 rounded-full font-bold';
                document.getElementById('authBtn').innerHTML = `<i class="fa-solid fa-chart-line mr-2"></i>Panel Owner`;
                alert('Login Berhasil sebagai Owner!');
                openLoginModal(); // Buka panel owner langsung
            } else {
                document.getElementById('loginError').classList.remove('hidden');
            }
        }

        function logoutOwner() {
            isOwner = false;
            closeOwnerPanel();
            document.getElementById('roleBadge').innerText = 'Mode: Customer';
            document.getElementById('roleBadge').className = 'bg-slate-800 text-amber-400 border border-amber-500/30 text-xs px-3 py-1 rounded-full';
            document.getElementById('authBtn').innerHTML = `<i class="fa-solid fa-user-gear mr-2"></i>Login Owner`;
            alert('Berhasil Logout.');
        }

        // Inisialisasi Aplikasi
        renderMenu();
    </script>
</body>
</html>
