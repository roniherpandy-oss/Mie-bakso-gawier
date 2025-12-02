# Mie-bakso-gawier
Restoran Bakso
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Seblak Enak & Berkualitas</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 0; padding: 0; background-color: #fff8f0; }
        header { background-color: #ff4500; color: white; text-align: center; padding: 25px; }
        header h1 { margin: 0; font-size: 2rem; }
        header p { margin-top: 5px; font-size: 1rem; }
        .container { max-width: 1200px; margin: 0 auto; padding: 20px; }
        .hero { text-align: center; margin-bottom: 40px; }
        .hero img { width: 100%; max-width: 600px; border-radius: 15px; }
        .menu { display: flex; flex-wrap: wrap; justify-content: space-around; }
        .item { background: #fff5f0; padding: 20px; margin: 10px; border-radius: 15px; box-shadow: 0 5px 15px rgba(0,0,0,0.1); width: 300px; transition: transform 0.3s; }
        .item:hover { transform: scale(1.05); }
        .item img { width: 100%; height: 200px; object-fit: cover; border-radius: 10px; }
        .item h3 { margin: 10px 0 5px; }
        .item p { margin: 5px 0 10px; }
        button { background-color: #ff4500; color: white; border: none; padding: 10px 20px; border-radius: 10px; cursor: pointer; transition: background 0.3s; }
        button:hover { background-color: #e03e00; }
        footer { background-color: #333; color: white; text-align: center; padding: 15px; margin-top: 20px; }
        a { color: #ffcb9a; text-decoration: none; }
        a:hover { text-decoration: underline; }
        @media (max-width: 768px) { .item { width: 100%; } }
    </style>
</head>
<body>
    <header>
        <h1>Seblak Enak & Berkualitas</h1>
        <p>Seblak pedas gurih, bahan segar, siap santap!</p>
    </header>
    
    <div class="container">
        <section class="hero">
            <h2>Selamat Datang di Toko Seblak Kami</h2>
            <img src="https://images.unsplash.com/photo-1600891965051-79d3f0a6c32c?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=600" alt="Seblak Lezat">
            <p>Kunjungi lokasi kami: <a href="https://maps.app.goo.gl/hLvB972NzGVcsqMg8" target="_blank">Lihat di Google Maps</a></p>
        </section>
        
        <section class="menu">
            <div class="item">
                <img src="https://images.unsplash.com/photo-1600891965051-79d3f0a6c32c?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=400" alt="Seblak Original">
                <h3>Seblak Original</h3>
                <p>Bahan: Kerupuk, sayur, bumbu pedas. Harga: Rp15.000</p>
                <button data-text="Saya mau pesan Seblak Original">Pesan via WhatsApp</button>
            </div>
            <div class="item">
                <img src="https://images.unsplash.com/photo-1582452528216-d65d4ef3b167?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=400" alt="Seblak Seafood">
                <h3>Seblak Seafood</h3>
                <p>Bahan: Udang, cumi, bumbu spesial. Harga: Rp25.000</p>
                <button data-text="Saya mau pesan Seblak Seafood">Pesan via WhatsApp</button>
            </div>
        </section>
    </div>
    
    <footer>
        <p>&copy; 2023 Toko Seblak. Hubungi: 081122334133</p>
    </footer>
    
    <script>
        document.querySelectorAll('button').forEach(btn => {
            btn.addEventListener('click', () => {
                const msg = encodeURIComponent(btn.getAttribute('data-text'));
                window.open(`https://wa.me/6281122334133?text=${msg}`, '_blank');
            });
        });
    </script>
</body>
</html>
