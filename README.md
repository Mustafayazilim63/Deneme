<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Geçiş Butonu Örneği</title>
<style>
       body {
      font-family: Arial, sans-serif;
      background-color: #FFFFCC; /* Sarı */
      color: #000080; /* Mavi */
      margin: 0;
      padding: 0;
      text-align: center;
    }
    header {
      background-color: #000080; /* Mavi */
      color: #FFFFCC; /* Sarı */
      padding: 10%;
      text-align: center;
    }
    main {
      padding: 0%;
      font-size: 110%;
    }
    
    h2{
      padding: 4%;
    }
    
    footer {
      background-color: #000080; /* Mavi */
      color: #FFFFCC; /* Sarı */
      padding: 0px;
      text-align: center;
      position: fixed;
      bottom: 0;
      width: 100%;
    }
    button {
      background-color: #000080; /* Mavi */
      color: #FFFFCC; /* Sarı */
      padding: 5% 10%;
      border: none;
      border-radius: 5%;
      font-size: 100%;
      text-decoration: none;
      display: inline-block;
    }
    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .hidden {
        display: none;
    }
    
</style>
</head>
<body>
<div class="container">
    <div id="ilkSayfa">
         <header>
    <h1>Bilge Dede - Bebe Technology Group</h1>
  </header>
  <main>
    
    <h2 >Uygulamayı İndir</h2>
    <button onclick="gecis()">BilgeDede | indir</button>
    
    <h2>Uygulama Hakkında Bilgi</h2>
    <p>Bilge Dede, Bebe Technology Group tarafından geliştirilen bir okuma ve yazma uygulamasıdır </p>
    
    <h2>İletisim</h2>
    <p>Gmail:bebetechnlogygroup@gmail.com</p>
    
  </main>
  <footer>
    <p>© 2024 Bebe Technology Group | Tüm hakları saklıdır.</p>
  </footer>
        
    </div>
    <div id="ikinciSayfa" class="hidden">
        <h1>Çok yakında...</h1>
        <p>Bizi takipte kalın.</p>
    </div>
</div>

<script>
    function gecis() {
        document.getElementById('ilkSayfa').classList.add('hidden');
        document.getElementById('ikinciSayfa').classList.remove('hidden');
        window.scrollTo(0, 0); // Sayfanın en üstüne gitmek için
    }
</script>
</body>
</html>
