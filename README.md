# Projeto Loteca
Este é um projeto de simulador de loteria, onde o usuário digita 6 números e realiza um sorteio de outros 6 números, logo é verificado quantos números ele acertou.

## Tecnologia utilizadas
- **HTML**: Estrutura do site
- __CSS__: Estilização do site
- *_JS_*: Funções o site
- ~~BootStrap~~: Não foi utilizado

### Melhorias Possíveis
1. [ ] Subir para o GitHubPages
2. [ ] Alterar os alerts
3. [ ] Utilizar o Bootstrap
4. [ ] Deixar responsivo 

### Disponibilizado em
[GitHubPages](https://fabioramos-02.github.io/loteca-mat/)

| ID | Primeira tela | Segunda Tela |
|----|---------------|--------------|
| 1 | Loteca Limpa   | loteca Preenchida |
| 2 | ![tela loteca não preenchida](https://user-images.githubusercontent.com/101193102/161781655-7cbd1142-cd83-44f6-8b9b-11f195b2d8c8.png) | ![loteca Preenchida](https://user-images.githubusercontent.com/101193102/161782575-3d053bdb-4f59-4b30-943d-11a9c1ca7dcb.png) |

#### Função Princiapl
```
function sorteio() {
  if(numEsco.length == 6){
  var cont = 0;
  numSort = [];

  while (cont < 6) {
    let num = Math.random() * 60;
    num = Math.ceil(num);
    if (!numSort.includes(num)) {
      numSort[cont] = num;
      console.log(numSort);
      cont++;
    }
  }
  
  document.getElementById("sorteados").innerHTML = numSort;
  contAcertos();
} else {
  alert("É necessario digitar seis numeros antes do sorteio")

}
}
```
