
Link do video:
youtube.com/watch?v=gXLjWRteuWI

Link projeto Figma:
https://www.figma.com/file/ReJbOWDc0WR1uizrsgfyfQ/project?node-id=26%3A2

Processo de construção a partir dos ensinamentos do vídeo:

Primeiro analizar o layout no Figma, entendo os elementos e suas disposições.

Em seguida estruturar o HTML, criando seções, divs e todos elementos necessários que serão estilizados.
Utiliza-se de arquivos SVG para maior responsidavidade dos icones, importando-os diretamente do Figma.

No CSS o curso começa trabalhando com o menor dimensionamento (celular) para depois adaptar a responsividade para outros tamanhos. É utilizado o SASS juntamente com a extensão SASS server para renderizar e gerar os arquivos css normais.
Para maior responsividade, utilizamos Media Query (@media) fazendo o processo do menor para o maior, já que começamos a partir de telas menores. 
@media only screen and (min-width: 680px)
@media only screen and (min-width: 1200px)
Utilizamos animações para gerar uma sensação mais agradavél perante a página, usando a propriedade animation no elemento que queremos modificar, dando um nome para animação (Ex: animation: moveArrow 1s alternate-reverse infinite;). Então utilizamos @keyframes para modular as mudanças da animação, puxando-a através do nome que demos previamente. (Ex: @keyframes moveDown {
    from {
        transform: translateY(-100px);
    }
    to {
        transform: translateY(0);
        opacity: 1;
    }
})
Para gerar animações um site útil é: https://bennettfeely.com/clippy/

Para gerar interação com o menu sanduiche, utiliza-se um código JavaScript dentro do próprio HTML com a tag <script>, neste caso foi utilizado um script para ao click abrir e fechar a barra dos menus (em telas menores)

