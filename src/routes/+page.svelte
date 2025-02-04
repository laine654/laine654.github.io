<script>
    export let title = "Bem-vindo ao My Food Blog!🍰";
  </script>
  
  <main>
    <h1>{title}</h1>
    <img src="/channels4_profile.jpg" alt="Imagem de destaque do blog" />
    <p>DESCUBRA RECEITAS INCRIVEIS, QUE TE DEIXARA COM AGUA NA BOCA!!.</p>
    <div class="buttons">
      <a href="/recipes" class="btn">Receitas Salgadas</a>
      <a href="/sweet-recipes" class="btn">Receitas Doces</a>
    </div>
  </main>
  
  <style>
    main {
      text-align: center;
      margin: 2rem;
    }
    img {
      max-width: 100%;
      height: auto;
      border-radius: 10px;
      margin: 1rem 0;
    }
    .buttons {
      display: flex;
      justify-content: center;
      gap: 10px;
    }
    .btn {
      display: inline-block;
      padding: 10px 20px;
      background-color: #ff6b6b;
      color: white;
      text-decoration: none;
      border-radius: 5px;
    }

   
 body {
  background: linear-gradient(to right, #9ad7ffde, #fad0c4);
  min-height: 100vh; 
  margin: 0;
  font-family: Arial, sans-serif;
}

main {
  background: rgba(255, 255, 255, 0.247);
  padding: 20px;
  border-radius: 10px;
  max-width: 900px;
  margin: 40px auto;
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
}

  </style>
  