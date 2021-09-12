# Genius Game!
Simples jogo de memória, cujo objetivo é desafiar os participantes a acertarem as diversas sequências musicais propostas no jogo. São quatro cores, verde, amarelo, azul e vermelho, que formam sequências aleatórias, que vão aumentando de dificuldade conforme o andamento do jogo.

## Como jogar:
* Clique nas cores conforme as sequências apresentadas.

## Linguagens utilizadas
* HTML;
* Javascript; e
* CSS

## Projeto
Projeto realizado para o curso de **JavaScript Game Developer** da **Digital Innovation One**.


{% hint style="info" %}
É necessário adicionar o tempo do setTimeout da função lightColor. Faltou colocar _number_ no final. Tem um Pull Request no [github da Gabriela](https://github.com/SpruceGabriela/genesis-dio) que identificou isso e corrigiu isso.
{% endhint %}

```javascript
// acende a próxima cor
let lightColor = (element, number) => {
    number = number * 500;
    setTimeout(() => {
        element.classList.add('selected');
    }, number - 250);
    setTimeout(() => {
        element.classList.remove('selected');
    }, number);
}
```