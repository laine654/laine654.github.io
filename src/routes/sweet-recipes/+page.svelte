
<script>
    let sweetRecipes = [
      { 
        title: "Bolo de Cenoura", 
        description: "Este bolo de cenoura é uma deliciosa opção para quem ama um doce caseiro. Com uma textura macia e uma cobertura de chocolate cremoso, é perfeito para acompanhar um café ou chá. Rende 12 porções.", 
        image: "/download (4).jfif",
        link: "https://receitadaboa.com.br/receitas/bolo-de-cenoura-fofinho-com-cobertura-de-chocolate-cremoso/" 
      },
      { 
        title: "Torta de Limão", 
        description: "Torta de limão é uma torta cozida no forno e recheada com um creme a base de limão. Sua origem é incerta, embora existam alguns relatos que indicam que tem origem no sul dos Estados Unidos ou na França.", 
        image: "/img-8977.jpg",
        link: "https://catracalivre.com.br/receitas/torta-de-limao-facil/" 
      },
      { 
        title: "Brigadeiro", 
        description: "O brigadeiro é um doce típico da culinária brasileira, de origem paulista, que rapidamente se difundiu pelo resto do país, tornando-se comum em todo o país a sua presença em festas de aniversário, junto com doces como o cajuzinho e o beijinho. É conhecido também no Rio Grande do Sul pelo nome de negrinho.", 
        image: "/65PAZKHVUFAXDDB4COUHCL3ZSQ.avif",
        link: "https://www.estadao.com.br/paladar/receita/brigadeiro-ao-leite/" 
      },
      { 
        title: "Pudim de Leite", 
        description: "Os pudins antigos são apresentados em forma de massa sólida, constituída pela mistura de vários ingredientes unidos por uma liga que pode incluir farinha de trigo (como no Pudim de Yorkshire), sangue (pudim preto), ovos (pudim de pão), ou uma mistura de gordura e farinha ou algum outro cereal (pudim de ameixa). Esses tipos de pudim podem ser assados, cozidos ou fervidos. Esse tipo ainda é comum em vários lugares, especialmente na Grã-Bretanha, e pode ser o prato principal de uma refeição ou a sobremesa.", 
        image: "/pudim-de-leite-receita.webp",
        link: "https://receitas.globo.com/tipos-de-prato/doces-e-sobremesas/pudim-de-leite-condensado-5641fa104d388508c300004d.ghtml" 
      },
      { 
        title: "Cookies de Chocolate", 
        description: "A palavra cookie vem do alemão, koekje, que significa “pequeno bolo”. Ganhou esse nome porque era, naquele tempo, feita a partir da massa de um bolo e usada para testar a temperatura do forno antes de colocar o bolo inteiro para assar, minimizando os erros. Foram os britânicos que descobriram a bolachinha e acharam que combinaria com seu tradicional chá. Até o século XVIII, as receitas ainda eram publicadas nos livros de culinária como pequenos bolos, apesar de já serem muito populares na Europa há, pelo menos, quatro séculos.", 
        image: "/download (5).jfif",
        link: "https://www.receitasnestle.com.br/receitas/cookies-de-chocolate-com-gotas-de-chocolate-branco-nestle" 
      },
    ];
  </script>
  
  <main>
    <h1>Receitas Doces</h1>
    <div class="grid">
      {#each sweetRecipes as recipe}
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
    .tamanho-padrao {
        width: 400px;
    }
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
  background-color: rgb(219, 52, 60);
  padding: 12px 20px;
  border-radius: 5px;
  color: white;
  text-decoration: none;
  font-weight: bold;
}

.back:hover {
  background-color: #bb2121;
}

  </style>

  
  