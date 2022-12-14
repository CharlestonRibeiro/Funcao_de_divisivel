# desafio 1 - Seleção de Desenvolvedor de Software.

Teste Técnico 01.

- Para resolução desse desafio foi escolhido a linguagem Dart.    

Descrição:
- Implemente uma função que receba um número inteiro positivo e retorne o
somatório de todos os valores inteiros divisíveis por 3 ou 5 que sejam inferiores ao
número passado.

### Solução desenvolvida:

```
void main() {

  String error = '';
  List<int> result = [];
  int sum = 0;

  divisible(int num) {
    if (num < 0) {
      return error = 'Por favor insira um numero positivo';
    } else {
      for (var i = 0; i < num; i++) {
        if (i % 3 == 0 || i % 5 == 0) {
          result.add(i);
          sum = sum + i;
        }
      }
      return sum;
    }
  }

  print(divisible(11));
}
```

Exemplos:
- Caso sua função receba o inteiro 10, ela deve retornar 23, resultante do somatório
dos números 3, 5, 6 e 9 que são menores que 10.
- Caso sua função receba o inteiro 11, ela deve retornar 33, resultante do somatório
dos números 3, 5, 6, 9 e 10 que são menores que 11.

---------

# Como Testar:

Recomendo testar a solução copiando o código acima e colando no DartPad: [Link](https://dartpad.dev/?).  

- Tutorial em vídeo de como usar o DartPad: [Link](https://www.youtube.com/watch?v=dkJF_YLFMLs&ab_channel=KamusWarrior).

# Como rodar:
 
Baixe o projeto:

- Tutorial de como baixar arquivos no GitHub: [Link](https://pt.jugomobile.com/como-baixar-arquivos-do-github/).
- Caso opte por baixar pode ser necessário instalar o Flutter: [Link](https://docs.flutter.dev/get-started/install).



