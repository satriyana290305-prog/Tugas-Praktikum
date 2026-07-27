<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Toko Elektronik Cepat</title>
    <style>
        * { box-sizing: border-box; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
        body { margin: 0; padding: 20px; background-color: #f4f6f9; color: #333; }
        header { background: linear-gradient(135deg, #1e3c72, #2a5298); color: white; padding: 20px; border-radius: 10px; margin-bottom: 20px; display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; }
        header h1 { margin: 0; font-size: 24px; }
        #jam-digital { font-size: 1.1em; background: rgba(255,255,255,0.2); padding: 8px 15px; border-radius: 5px; font-family: monospace; }
        
        .main-container { display: grid; grid-template-columns: 2fr 1fr; gap: 20px; }
        @media (max-width: 768px) { .main-container { grid-template-columns: 1fr; } }
        
        .card { background: white; padding: 20px; border-radius: 10px; box-shadow: 0 4px 6px rgba(0,0,0,0.05); margin-bottom: 20px; }
        .card h2 { margin-top: 0; color: #1e3c72; border-bottom: 2px solid #eee; padding-bottom: 10px; }
        
        /* Slideshow Layout */
        .slideshow-container { text-align: center; position: relative; background: #fafafa; padding: 15px; border-radius: 8px; }
        .slideshow-container img { width: 100%; max-height: 300px; object-fit: contain; border-radius: 5px; }
        .nav-btn { background: #1e3c72; color: white; border: none; padding: 10px 15px; cursor: pointer; border-radius: 5px; margin: 10px 5px; font-weight: bold; }
        .nav-btn:hover { background: #2a5298; }
        .prod-info { margin-top: 15px; }
        .prod-price { font-size: 20px; color: crimson; font-weight: bold; }

        /* Product List Layout */
        .product-list { list-style: none; padding: 0; margin: 0; }
        .product-list li { padding: 12px 15px; background: #f8f9fa; margin-bottom: 8px; border-left: 5px solid #ccc; cursor: pointer; border-radius: 0 5px 5px 0; transition: all 0.2s; font-weight: 500; }
        .product-list li:hover { background: #e9ecef; border-left-color: #2a5298; transform: translateX(3px); }
        .product-list li.active { background: #e2ecf7; border-left-color: #1e3c72; color: #1e3c72; }

        /* Form Layout */
        .form-group { margin-bottom: 15px; }
        .form-group label { display: block; margin-bottom: 5px; font-weight: 600; }
        .form-group input { width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 5px; font-size: 14px; }
        .form-group input:focus { border-color: #1e3c72; outline: none; }
        .btn-submit { width: 100%; background: #28a745; color: white; border: none; padding: 12px; font-size: 16px; font-weight: bold; border-radius: 5px; cursor: pointer; }
        .btn-submit:hover { background: #218838; }
        .error-msg { color: red; font-size: 0.85em; margin-top: 5px; display: block; }

        /* Invoice Output Layout */
        .invoice-box { background: #fffde7; border: 2px dashed #fbc02d; padding: 20px; border-radius: 8px; margin-top: 20px; display: none; }
        .invoice-box table { width: 100%; border-collapse: collapse; margin-top: 10px; }
        .invoice-box td { padding: 8px 0; font-size: 15px; }
        .invoice-box td:first-child { font-weight: bold; color: #555; width: 40%; }
        .invoice-total { font-size: 18px; color: #1e3c72; font-weight: bold; border-top: 2px solid #ccc; padding-top: 10px; }
    </style>
</head>
<body>

    <header>
        <h1>Toko Elektronik Cepat</h1>
        <div id="jam-digital">Memuat Waktu...</div>
    </header>

    <div class="main-container">
        <!-- Kolom Kiri: Display & Order Form -->
        <div>
            <div class="card">
                <h2>Display Produk Utama</h2>
                <div class="slideshow-container">
                    <img id="main-image" src="" alt="Produk">
                    <div>
                        <button class="nav-btn" onclick="ubahSlide(-1)">◀ Prev</button>
                        <button class="nav-btn" onclick="ubahSlide(1)">Next ▶</button>
                    </div>
                </div>
                <div class="prod-info">
                    <h3 id="main-prod-name">-</h3>
                    <div class="prod-price" id="main-prod-price">Rp 0</div>
                </div>
            </div>

            <div class="card">
                <h2>Formulir Pemesanan</h2>
                <div class="form-group">
                    <label for="nama-pemesan">Nama Pemesan *</label>
                    <input type="text" id="nama-pemesan" placeholder="Masukkan nama lengkap Anda">
                    <span id="err-nama" class="error-msg"></span>
                </div>
                <div class="form-group">
                    <label for="jumlah-pesan">Jumlah Pesan *</label>
                    <input type="number" id="jumlah-pesan" min="1" value="1">
                    <span id="err-jumlah" class="error-msg"></span>
                </div>
                <div class="form-group">
                    <label for="kode-promo">Kode Promo (Gunakan 'DISKON10')</label>
                    <input type="text" id="kode-promo" placeholder="Contoh: DISKON10">
                </div>
                <button class="btn-submit" onclick="prosesPemesanan()">Pesan Sekarang</button>
            </div>
        </div>

        <!-- Kolom Kanan: Daftar Produk & Output Struk -->
        <div>
            <div class="card">
                <h2>Daftar Produk</h2>
                <ul id="list-produk-dom" class="product-list"></ul>
            </div>

            <div id="invoice" class="invoice-box">
                <h3 style="margin-top:0; text-align:center; color:#fbc02d;">🧾 STRUK RINGKASAN PESANAN</h3>
                <table>
                    <tr><td>ID Pesanan</td><td id="inv-id"></td></tr>
                    <tr><td>Nama Pemesan</td><td id="inv-nama"></td></tr>
                    <tr><td>Nama Produk</td><td id="inv-produk"></td></tr>
                    <tr><td>Jumlah Barang</td><td id="inv-qty"></td></tr>
                    <tr><td>Subtotal</td><td id="inv-sub"></td></tr>
                    <tr><td>Potongan Diskon</td><td id="inv-potongan"></td></tr>
                    <tr class="invoice-total"><td>Total Akhir</td><td id="inv-total"></td></tr>
                </table>
            </div>
        </div>
    </div>

    <script>
        // 1. DATA ARRAY PRODUK (Minimal 3 produk beserta objek data lengkap)
        var databaseProduk = [
            {
                nama: "Smartphone Galaxy Prime v4",
                harga: 3500000,
                gambar: [
                    "https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?w=400",
                    "https://images.unsplash.com/photo-1598327105666-5b89351aff97?w=400"
                ]
            },
            {
                nama: "Laptop UltraBook Pro Slim",
                harga: 8500000,
                gambar: [
                    "https://images.unsplash.com/photo-1496181130204-755241524eab?w=400",
                    "https://images.unsplash.com/photo-1588872657578-7efd1f1555ed?w=400"
                ]
            },
            {
                nama: "Wireless Headphone Noise Cancel",
                harga: 1200000,
                gambar: [
                    "https://images.unsplash.com/photo-1505740420928-5e560c06d30e?w=400",
                    "https://images.unsplash.com/photo-1484704849700-f032a568e944?w=400"
                ]
            }
        ];

        var produkAktifIndex = 0;
        var slideGambarIndex = 0;

        // 2. JAM DIGITAL REAL-TIME (Date & setInterval)
        function mulaiJamDigital() {
            setInterval(function() {
                var d = new Date();
                var tgl = d.getDate() + "-" + (d.getMonth()+1) + "-" + d.getFullYear();
                var jam = (d.getHours()<10?"0":"")+d.getHours() + ":" + 
                          (d.getMinutes()<10?"0":"")+d.getMinutes() + ":" + 
                          (d.getSeconds()<10?"0":"")+d.getSeconds();
                document.getElementById("jam-digital").innerText = tgl + " || " + jam;
            }, 1000);
        }

        // 3. GENERATE LIST PRODUK (Looping & DOM)
        function renderDaftarProduk() {
            var listContainer = document.getElementById("list-produk-dom");
            listContainer.innerHTML = "";
            for (let i = 0; i < databaseProduk.length; i++) {
                var kelasAktif = (i === produkAktifIndex) ? "class='active'" : "";
                listContainer.innerHTML += "<li " + kelasAktif + " onclick='gantiProdukAktif(" + i + ")'>" + databaseProduk[i].nama + "</li>";
            }
        }

        // 4. DISPLAY UPDATE UTAMA 
        function updateDisplayProduk() {
            var prod = databaseProduk[produkAktifIndex];
            document.getElementById("main-prod-name").innerText = prod.nama;
            document.getElementById("main-prod-price").innerText = "Rp " + prod.harga.toLocaleString('id-ID');
            document.getElementById("main-image").src = prod.gambar[slideGambarIndex];
        }

        function gantiProdukAktif(index) {
            produkAktifIndex = index;
            slideGambarIndex = 0; // reset ke gambar pertama produk baru
            renderDaftarProduk(); // Re-render highlight list samping
            updateDisplayProduk();
        }

        // 5. CAROUSEL SLIDESHOW UTAMA
        function ubahSlide(arah) {
            var listGambar = databaseProduk[produkAktifIndex].gambar;
            slideGambarIndex += arah;
            if (slideGambarIndex >= listGambar.length) slideGambarIndex = 0;
            if (slideGambarIndex < 0) slideGambarIndex = listGambar.length - 1;
            document.getElementById("main-image").src = listGambar[slideGambarIndex];
        }

        // 6. LOGIKA PROSES PEMESANAN (Validasi, Perhitungan, String, & Math Objek)
        function prosesPemesanan() {
            var nama = document.getElementById("nama-pemesan").value.trim();
            var qty = parseInt(document.getElementById("jumlah-pesan").value);
            var promo = document.getElementById("kode-promo").value.trim();
            
            var errNama = document.getElementById("err-nama");
            var errQty = document.getElementById("err-jumlah");
            
            // Reset state error & invoice
            errNama.innerHTML = ""; errQty.innerHTML = "";
            document.getElementById("invoice").style.display = "none";

            var valid = true;

            // Validasi input form
            if (nama === "") {
                errNama.innerHTML = "Nama pemesan wajib diisi!";
                valid = false;
            }
            if (isNaN(qty) || qty <= 0) {
                errQty.innerHTML = "Jumlah pesan harus berupa angka lebih besar dari 0!";
                valid = false;
            }

            if (!valid) return; // Hentikan fungsi jika form tidak valid

            // Kalkulasi matematika harga dasar
            var produkTerpilih = databaseProduk[produkAktifIndex];
            var subtotal = produkTerpilih.harga * qty;
            var potongan = 0;

            // Manipulasi String & Percabangan Diskon 10%
            if (promo.toUpperCase() === "DISKON10") {
                potongan = subtotal * 0.10;
            }

            var totalAkhir = subtotal - potongan;

            // Pembuatan acak Nomor Order ID unik (Objek Math)
            var angkaAcakUnique = Math.floor(Math.random() * 90000) + 10000; // Menghasilkan 5 digit (10000 - 99999)
            var orderID = "INV-" + angkaAcakUnique;

            // Menampilkan data olahan ke Struk Output Invoice
            document.getElementById("inv-id").innerText = orderID;
            document.getElementById("inv-nama").innerText = nama;
            document.getElementById("inv-produk").innerText = produkTerpilih.nama;
            document.getElementById("inv-qty").innerText = qty + " unit";
            document.getElementById("inv-sub").innerText = "Rp " + subtotal.toLocaleString('id-ID');
            document.getElementById("inv-potongan").innerText = "Rp " + potongan.toLocaleString('id-ID');
            document.getElementById("inv-total").innerText = "Rp " + totalAkhir.toLocaleString('id-ID');

            // Munculkan container invoice ke user
            document.getElementById("invoice").style.display = "block";
        }

        // Inisialisasi program saat jendela pertama dimuat browser
        window.onload = function() {
            mulaiJamDigital();
            renderDaftarProduk();
            updateDisplayProduk();
        };
    </script>
</body>   
</html>
