<!DOCTYPE html>
<html lang="pt-br">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Curitiba</title>
         <style>
                header{
                    background-color: #D0F9AE;
                    color: #000000;
                    text-align: center; 
                    max-width: 800px;
                    margin: 0 auto;
                    padding: 16px;
                    border: 5px solid #417208;
                }
                main{
                    background-color: #ffffff;
                    color:#2c4907;
                    text-align: center; 
                    max-width: 800px;
                    margin: 0 auto;
                    padding: 16px;
                }
                article{
                    display: flex;
                }

                img{
                    width: 120px;
                    height: 80px;
                }
                .artigo-autor {
                    font-weight: bold;
                }
            </style>
    </head>
    <body>
        <header>
            <h1>Curitiba</h1>
            <p>vou compartilhar curiosidades/conhecimentos sobre Curitiba</p>
        </header>
        <main>
            <article>
                <img src="imagem-de curitiba.png" alt="Ilustração em pixel art dos pontos turísticos de Curitiba, com o Jardim Botânico, Catedral e uma estátua sábia contando a história da cidade ao fundo.">
                <div>
                    <h2>Primeiras curiosidades</h2>
                    <p class="artigo-autor">por: Luiz Matheus Martins</p>
                    <p>Seja bem vindo a minha pagina de web, irei conpartilhar algumas curiosidades sobre Curitiba</p>
                    <button>❤️ <SPan>0</SPan></button>
                    <button>👍 <SPan>0</SPan></button>
                </div> 
            </article>
            <article>
                <img src="imagem-de curitiba.png" alt="Ilustração em pixel art dos pontos turísticos de Curitiba, com o Jardim Botânico, Catedral e uma estátua sábia contando a história da cidade ao fundo.">
               <div>
                   <h2>Segundas curiosidades</h2>
                   <p class="artigo-autor">por: Luiz Matheus Martins</p>
                   <p>Seja bem vindo a minha pagina de web, irei conpartilhar algumas curiosidades sobre Curitiba</p>
                   <button>❤️ <SPan>0</SPan></button>
                   <button>👍 <SPan>0</SPan></button>
               </div>
            </article>
        </main>
    </body>
    <Script>
        const botoes = document.querySelectorAll("button");
        
        botoes.forEach( function(botao){
            let curtiu = false;
            botao.addEventListener("click", botaoClicado);         
            function botaoClicado(){
                console.log("fui clicado");
                let texto = botao.querySelector("span");
                if (curtiu === false){
                    texto.textContent++;
                    curtiu = true;
                } else{
                    texto.textContent--;
                    curtiu = false;
                }
            }
        } )


    </Script>
</html>
