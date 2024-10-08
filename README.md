<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eros Music - Fatos Musicais</title>
    <style>
        /* Importa a fonte Chakra Petch do Google Fonts */
@import url('https://fonts.googleapis.com/css2?family=Chakra+Petch:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500;1,600;1,700&display=swap');

/* Estiliza o corpo da página */
body {
    font-family: "Chakra Petch", sans-serif; /* Define a fonte padrão */
    background-color: #020520; /* Cor de fundo da página */
    display: flex; /* Usa Flexbox para layout */
    flex-direction: column; /* Alinha os itens na vertical */
    align-items: center; /* Centraliza os itens horizontalmente */
    justify-content: center; /* Centraliza os itens verticalmente */
    height: 100vh; /* Preenche a altura total da viewport */
    margin: 0; /* Remove a margem padrão */
    padding: 0; /* Remove o padding padrão */
}

/* Estiliza os títulos h1 */
h1 {
    font-size: 50px; /* Tamanho da fonte */
    color: #033073; /* Cor do texto */
    text-align: center; /* Alinha o texto ao centro */
    letter-spacing: 3px; /* Espaçamento entre letras */
}

h2 {
    font-size: 20px; /* Tamanho da fonte */
    color: #0723a0; /* Cor do texto */
    text-align: center; /* Alinha o texto ao centro */
    letter-spacing: 3px; /* Espaçamento entre letras */
}

p {
    color: #FFFFFF;
}

/* Estiliza as seções da página */
section {
    display: flex; /* Usa Flexbox para layout */
    flex-direction: column; /* Alinha os itens na vertical */
    align-items: center; /* Centraliza os itens horizontalmente */
    margin-bottom: 3rem; /* Espaçamento abaixo de cada seção */
}

/* Estiliza os inputs dentro das seções */
section input {
    width: 30rem; /* Largura dos inputs */
    border: none; /* Remove a borda padrão */
    padding: 1rem; /* Espaçamento interno */
    border-radius: 1.5rem; /* Borda arredondada */
    margin-bottom: 1rem; /* Espaçamento abaixo dos inputs */
    color: #09368f; /* Cor do texto */
    font-size: 1rem; /* Tamanho da fonte */
    box-sizing: border-box; /* Inclui padding e border na largura total */
}

/* Estiliza os botões dentro das seções */
button {
    padding: 0.8rem 1.2rem; /* Espaçamento interno do botão */
    border: none; /* Remove a borda padrão */
    border-radius: 1.5rem; /* Borda arredondada */
    background-color: #033073; /* Cor de fundo do botão */
    color: #ffffff; /* Cor do texto do botão */
    font-size: 1rem; /* Tamanho da fonte */
    cursor: pointer; /* Muda o cursor para indicar que é clicável */
}

/* Adiciona efeito hover ao botão de pesquisa */
button:hover {
    background-color: #30475E; /* Muda a cor de fundo ao passar o mouse */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Adiciona uma sombra mais intensa */
}

/* Estiliza a caixa de resultados da pesquisa */
.resultados-pesquisa {
    width: 60rem; /* Largura máxima da caixa de resultados */
    height: 46vh; /* Altura máxima da caixa de resultados */
    overflow-y: auto; /* Adiciona rolagem vertical se necessário */
    margin-top: 1rem; /* Espaçamento acima da caixa de resultados */
    padding: 1rem; /* Espaçamento interno */
    border-radius: 0.6rem; /* Borda arredondada */
}

/* Estiliza cada item de resultado */
.item-resultado {
    background: #020520; /* Cor de fundo dos itens */
    border-radius: 0.6rem; /* Borda arredondada */
    padding: 1rem; /* Espaçamento interno */
    margin-bottom: 1rem; /* Espaçamento abaixo dos itens */
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* Sombra leve */
}

/* Estiliza os títulos dentro dos itens de resultado */
.item-resultado h2 {
    font-size: 1.5rem; /* Tamanho da fonte */
    color: #ffffff; /* Cor do texto */
}

/* Estiliza os links dentro dos itens de resultado */
.item-resultado a {
    text-decoration: none; /* Remove o sublinhado padrão dos links */
    color: #033073; /* Cor do texto dos links */
}

/* Estiliza os links quando são passados o mouse sobre */
.item-resultado a:hover {
    text-decoration: underline; /* Adiciona sublinhado ao passar o mouse */
}

/* Estiliza a descrição meta dentro dos itens de resultado */
.descricao-meta {
    color: #45474B; /* Cor do texto */
    margin: 0.5rem 0; /* Margem acima e abaixo */
}

/* Estiliza o rodapé da página */
footer {
    background-color: #030c35; /* Cor de fundo do rodapé */
    color: #45474B; /* Cor do texto */
    text-align: center; /* Alinha o texto ao centro */
    padding: 0; /* Espaçamento interno */
    width: 100%; /* Largura total da página */
    position: absolute; /* Posiciona o rodapé */
    bottom: 0; /* Alinha ao fundo da página */
    font-size: 1rem; /* Tamanho da fonte */
}

@media (max-width: 768px) {
    h1 {
        font-size: 2rem; /* Tamanho da fonte em telas menores */
        letter-spacing: 0.2rem; /* Espaçamento entre letras em telas menores */
    }

    section input {
        width: 25rem; /* Largura dos inputs em telas menores */
        padding: 0.8rem; /* Espaçamento interno em telas menores */
    }

    .resultados-pesquisa {
        width: 40rem; /* Largura da caixa de resultados em telas menores */
        height: 40vh; /* Altura da caixa de resultados em telas menores */
    }

    .item-resultado h2 {
        font-size: 1.3rem; /* Tamanho da fonte dos títulos em telas menores */
    }
}

/* Responsividade para celulares */
@media (max-width: 480px) {

    h1 {
        font-size: 1.8rem; /* Tamanho da fonte em telas pequenas */
        letter-spacing: 0.1rem; /* Espaçamento entre letras em telas pequenas */
    }

    section input {
        width: 17rem; /* Largura total dos inputs em telas pequenas */
        color: #033073;
    }

    button {
        padding: 0.6rem 1rem; /* Espaçamento interno do botão em telas pequenas */
        font-size: 0.9rem; /* Tamanho da fonte do botão em telas pequenas */
    }

    .resultados-pesquisa {
        width: 90%; /* Largura da caixa de resultados em telas pequenas */
        height: 50vh; /* Altura da caixa de resultados em telas pequenas */
    }

    .item-resultado h2 {
        font-size: 1.1rem; /* Tamanho da fonte dos títulos em telas pequenas */
    }

    footer {
        font-size: 1px; /* Tamanho da fonte do rodapé em telas pequenas */
    }
}
    </style>
</head>
<body>
    <header>
        <h1>Fatos Sobre a Música</h1>
        
    </header>
    <main>
        <section>
        <input type="text" placeholder="Digite sua busca musical" id="campo-pesquisa">
        </section>
        <section>
        <button onclick="pesquisar()">Pesquisar</button>
        </section>
        <section class="resultados-pesquisa" id="resultados-pesquisa">
        </section>
        <h2>Trítono</h2>
    </main>
    <footer>
        <p>2024 - Fatos Musicais. Todos os Direitos Reservados.</p>
        <p>Entre em contato pelo email: leandro.luiz.junior2006@gmail.com</p>
    </footer>
</body>
<script>
    let dados = [
        {
        titulo : "Trítono",
        descricao : "É um intervalo de 3 tons, entre duas notas musicais. Houve crenças de que o Trítono tinha alguma relação com o diabo.",
        link : "https://pt.wikipedia.org/wiki/Tr%C3%ADtono#:~:text=Chamamos%20de%20Tr%C3%ADtono",
        tags : "diabo diabolos"
        },
        {
            titulo : "Círculo das Quintas",
            descricao : "É um mapa circular que explica as relações das 12 notas da escala cromática. A distância de cada uma das notas, tanto no sentido horário, quanto no anti-horário, é distanciada de quintas.",
            link : "https://pt.wikipedia.org/wiki/C%C3%ADrculo_de_quintas",
            tags: "círculo quinta quintas"
        },
        {    
            titulo : "Inversão de Intervalos",
            descricao : "É um evento musical, pela qual o leitor inverte a posição de uma das duas notas, colocando uma delas uma oitava acima ou abaixo.",
            link: "https://pt.wikipedia.org/wiki/Invers%C3%A3o_(m%C3%BAsica)#:~:text=Em%20harmonia%2C%20o%20termo%20indica,%C3%A9%20a%20s%C3%A9tima%2C%20terceira%20invers%C3%A3o.",
            tags: "inversão intervalos"
        }
    ]

    function pesquisar() {
  const section = document.getElementById("resultados-pesquisa");
  const campoPesquisa = document.getElementById("campo-pesquisa").value.toLowerCase();

  if (!campoPesquisa) {
    section.innerHTML = "<p>Não há resultados</p>";
    return;
  }

  let resultados = "";

  for (let dado of dados) {
    const titulo = dado.titulo.toLowerCase();
    const descricao = dado.descricao.toLowerCase();
    const tags = dado.tags.toLowerCase();

    if (titulo.includes(campoPesquisa) || descricao.includes(campoPesquisa) || tags.includes(campoPesquisa)) {
      resultados += `
        <div class="item-resultado">
          <h2>
            <a href="${dado.link}">${dado.titulo}</a>
          </h2>
          <p class="descricao-meta">${dado.descricao}</p>
        </div>
      `;
    }
  }

  section.innerHTML = resultados || "<p>Não temos este resultado de pesquisa</p>";
}
</script>
</html>
