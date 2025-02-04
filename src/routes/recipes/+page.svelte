<script>
    let recipes = [
      { 
        title: "Lasanha de Carne", 
        description: "Uma receita italiana clássica com molho bechamel e queijo derretido.", 
        description: "A lasanha tem origem profundamente enraizada na tradição italiana e pode ter sido inspirada em pratos similares na Roma Antiga. A versão mais próxima da lasanha que conhecemos hoje começou a se formar durante a Idade Média, na região de Nápoles, com finas tiras de massa preparadas al dente e recheio de queijo e legumes", 
        image: "/download (7).jfif",
        link: "https://www.tudogostoso.com.br/receita/11217-lasanha-de-frango-com-queijo.html" 
      },
      { 
        
        title: "Risoto de Frango", 
        description: "O risoto de frango tem origem italiana e é um prato típico da culinária italiana. Ele chegou no Brasil trazido pelos imigrantes da Itália e foi transformado com ingredientes locais como carnes, crustáceos, frango, pato e queijos. Inicialmente chamado de arroz de forno, o risoto é feito com arroz, caldo de carne e outros ingredientes, seguindo influências da França e Espanha.", 
        image: "/download.jfif",
        link: "https://irga.rs.gov.br/risoto-de-frango-com-legumes" 
      },
      { 
        title: "Escondidinho de Carne Seca", 
        description: "O escondidinho de carne seca é um prato com raízes profundas na culinária nordestina do Brasil. Acredita-se que tenha surgido no interior do Nordeste, possivelmente em Pernambuco ou na Paraíba, no início do século XX. O nome “escondidinho” vem do fato de a carne ficar “escondida” entre as camadas de purê de mandioca.", 
        image: "/download (1).jfif",
        link: "https://anamariareceitas.com.br/receitas/escondidinho-de-carne-seca/" 
      },
      { 
        title: "Quiche de Espinafre", 
        description: "Quiche é um tipo de tarte/torta feita com recheio à base de ovos e creme de leite ou natas, ao qual se adicionam pedacinhos de toucinho defumado, e que não leva cobertura. Embora atualmente a quiche seja considerada um prato tradicional da culinária francesa, sua origem é alemã, do reino medieval da Lorena", 
        image: "/download (2).jfif",
        link: "https://www.google.com/imgres?q=Quiche%20de%20Espinafre&imgurl=https%3A%2F%2Fstatic.itdg.com.br%2Fimages%2F1200-675%2Ffe8fca6a94850609b40599f7b9b34fa0%2F327153-original.jpg&imgrefurl=https%3A%2F%2Fwww.tudogostoso.com.br%2Freceita%2F23813-quiche-de-ricota-e-espinafre.html&docid=sbcBKLxC-RD0zM&tbnid=yC9xfnOqeDuzwM&vet=12ahUKEwjv1M_PjpmLAxXorZUCHdvbBtEQM3oECDMQAA..i&w=1000&h=667&hcb=2&ved=2ahUKEwjv1M_PjpmLAxXorZUCHdvbBtEQM3oECDMQAA" 
      },
      { 
        title: "Macarrão Carbonara", 
        description: "Carbonara, spaghetti alla carbonara ou pasta alla carbonara, é uma receita tradicional italiana de massa. Acredita-se que tenha sido uma receita apreciada pelos preparadores de carvão vegetal dos montes apeninos, na região italiana da Úmbria. Outras teorias apontam, por outro lado, que o nome se deve apenas à cor escura da pimenta preta recém moída, que é usada na sua preparação.", 
        image: "/download (3).jfif",
        link: "https://todeschinialimentos.com.br/receita/macarrao-a-carbonara" 
      },
    ];
  </script>
  
  <main>
    <h1>Receitas Salgadas</h1>
    <div class="grid">
      {#each recipes as recipe}
        <div class="card">
          <img src={recipe.image} alt={recipe.title} />
          <h2>{recipe.title}</h2>
          <p>{recipe.description}</p>
          <a href={recipe.link} class="btn">Ver Receita</a>
        </div>
      {/each}
    </div>

  <div class="back-button">
    <a href="/" class="btn back">Voltar para a Página Inicial</a>
  </div>

  </main>  
  
  <style>

    main {
      margin: 2rem;
      text-align: center;
    }
    ul {
      list-style: none;
      padding: 0;
    }
    li {
      margin-bottom: 2rem;
      text-align: center;
    }
    img {
      max-width: 80%;
      height: auto;
      border-radius: 10px;
      margin: 0 auto 1rem;
      display: block;
    }
    .btn {
      display: inline-block;
      padding: 10px 20px;
      background-color: #ff6b6b;
      color: white;
      text-decoration: none;
      border-radius: 5px;
    }

  
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  padding: 20px;
}

.card {
  background: #fff;
  border-radius: 10px;
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
  padding: 15px;
  text-align: center;
  transition: transform 0.2s;
}

.card:hover {
  transform: scale(1.05);
}

img {
  max-width: 100%;
  height: auto;
  border-radius: 10px;
}

.btn {
  display: inline-block;
  padding: 10px 20px;
  background-color: #ff6b6b;
  color: white;
  text-decoration: none;
  border-radius: 5px;
  margin-top: 10px;
}

.back-button {
  text-align: center;
  margin-top: 30px;
}

.back {
  background-color: #3498db;
  padding: 12px 20px;
  border-radius: 5px;
  color: white;
  text-decoration: none;
  font-weight: bold;
}

.back:hover {
  background-color: #217dbb;
}


  </style>
  