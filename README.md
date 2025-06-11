## Desafio de 7 dias

🚀 JavaScript e Comparação de Tipos

📌 Problema

Uma situação muito comum para quem utiliza JavaScript é lidar com problemas na comparação de valores devido aos diferentes tipos de variáveis. Em linguagens compiladas como Java e C#, esse erro é detectado durante a compilação, mas no JavaScript, os erros passam despercebidos até a execução do código.

A confusão acontece porque o JavaScript pode converter automaticamente os valores para um tipo booleano ao fazer comparações, o que pode causar resultados inesperados. Por exemplo, todos os testes abaixo retornam true:

console.log(false == '0');  // true


console.log(null == undefined);  // true


console.log(" \t\r\n" == 0);  // true


console.log(' ' == 0);  // true

Isso pode gerar bugs difíceis de identificar, especialmente para quem está começando a aprender lógica de programação com JavaScript.

🎯 Objetivo

Reescrever o código abaixo para que ele faça comparações corretas entre os valores, garantindo que a saída seja coerente e sem erros.

let numeroUm = 1;


let stringUm = '1';


let numeroTrinta = 30;


let stringTrinta = '30';


let numeroDez = 10;


let stringDez = '10';

### //Solução da reescrita do código começa aqui...




if (numeroUm === stringUm) {


  console.log('As variáveis numeroUm e stringUm têm o mesmo valor e mesmo tipo');
} 

else if (numeroUm == stringUm) {


  console.log('As variáveis numeroUm e stringUm têm o mesmo valor, mas tipos diferentes');
} 

else {


  console.log('As variáveis numeroUm e stringUm não têm o mesmo valor');
}

if (numeroTrinta === stringTrinta) {


  console.log('As variáveis numeroTrinta e stringTrinta têm o mesmo valor e mesmo tipo');
} 

else {


  console.log('As variáveis numeroTrinta e stringTrinta não têm o mesmo tipo');
}

if (numeroDez === stringDez) {


  console.log('As variáveis numeroDez e stringDez têm o mesmo valor e mesmo tipo');
} 

else if (numeroDez == stringDez) {


  console.log('As variáveis numeroDez e stringDez têm o mesmo valor, mas tipos diferentes');
} 
else {


  console.log('As variáveis numeroDez e stringDez não têm o mesmo valor');
}

🔥 Solução

Usando === (comparação estrita)

O operador === compara tanto o valor quanto o tipo das variáveis, evitando conversões automáticas indesejadas. Isso garante que o código funcione corretamente e evite comportamentos inesperados.

### Dicas para evitar problemas com comparação de tipos

✅ Sempre prefira === ao invés de == para comparações.

✅ Se precisar converter tipos, faça isso explicitamente (ex: Number(string) ou String(number)).

✅ Utilize typeof para verificar o tipo de uma variável antes da comparação.

🎯 Testando o Código

### Para testar o código, siga os passos:

1️⃣ Salve o código em um arquivo chamado script.js.

2️⃣ No terminal, execute:

node script.js

Se estiver rodando no navegador, abra o Console (F12 > Console no Chrome/Edge) e cole o código lá.

🛠️ Contribuindo

Se quiser sugerir melhorias ou reportar problemas, fique à vontade para abrir uma issue ou enviar um pull request! 🚀

📌 Autor: Luiz André (@brodyandre)
