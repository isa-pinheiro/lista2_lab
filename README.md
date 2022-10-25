# lista2_lab

  ## QUESTÃO 01 -
  Implemente um programa que tenha como entrada um número (1-7) que corresponde a um dos dias 
  da semana e imprima na tela o nome do dia correspondente (domingo, segunda, terça, quarta, quinta,
  sexta, sábado). Se o número lido não estiver no intervalo 1-7, imprima: “Número de dia não válido”. O
  programa deve permanecer executando até que o usuário tecle o numero 0. (Utilize obrigatoriamente
  teste no início).
  
  ``` c
  #include <stdio.h>
  
int main(void) {
  int n;
  while(n != 0){
    printf("Insira um número de 1-7 para saber o dia da semana correspondente: \nPara parar o programa, digite 0.\n");
  scanf("%d", &n);
    if(n == 1){
      printf("Domingo\n\n");
    } else if(n == 2){
      printf("Segunda\n\n");
    } else if(n == 3){
      printf("Terça\n\n");
    } else if(n == 4){
      printf("Quarta\n\n");
    } else if(n == 5){
      printf("Quinta\n\n");
    } else if(n == 6){
      printf("Sexta\n\n");
    } else if(n == 7){
      printf("Sábado\n\n");
    } else if(n != 0){
      printf("Dia da semana inválido\n\n");
    }
  }
}
  ```
  
  ## QUESTÃO 02 -
  Refaça o programa da Questão 1, utilizando a estrutura de repetição com teste no final.
  
   ``` c
   #include <stdio.h>

int main(void) {
  int n;
  printf("Insira um número de 1-7 para saber o dia da semana correspondente: \nPara parar o programa, digite 0.\n");
  scanf("%d", &n);
  
  do {
      if(n == 0){
        break;
      } else if(n == 1){
        printf("Domingo");
      } else if(n == 2){
        printf("Segunda");
      } else if(n == 3){
        printf("Terça");
      } else if(n == 4){
        printf("Quarta");
      } else if(n == 5){
        printf("Quinta");
      } else if(n == 6){
        printf("Sexta");
      } else if(n == 7){
        printf("Sábado");
      } else if(n != 0){
        printf("Dia da seman inválido");
      }
    printf("\n\nInsira um número de 1-7 para saber o dia da semana correspondente: \nPara parar o programa, digite 0.\n");
    scanf("%d", &n);
    } while (n != 0);
  return 0;
}
   ```
   
  ## QUESTÃO 03 -
  Escreva um programa que leia um número inteiro e positivo F e calcule o fatorial deste número.
  
   ``` c
   #include <stdio.h>
#include<stdlib.h>

int main(void) {
  int n, f = 1;
  puts("Insira um número natural: ");
  scanf("%d", &n);
  n = abs(n);
  for(int i = 1; i <= n; i++){
    f *= i;
  }
  
  printf("O fatorial desse número é: %d", f);
  
  return 0;
}
   ```
   
  ## QUESTÃO 04 -
  Implementar um programa para resolver o seguinte problema: José tem 150 centímetros e cresce 2
  centímetros por ano. O Pedro tem 110 centímetros e cresce 3 centímetros por ano. Em quantos anos
  Pedro será maior que José?

   ``` c
   #include <stdio.h>

int main(void) {
  int aj = 150, ap = 110, a;
  
  for(a = 1; aj > ap; a++){
  aj = 150 + 2 * a;
  ap = 110 + 3 * a;
  }
  
  printf("Pedro vai ser maior que josé em %d anos.", a);
  return 0;
}
   ```
   
  ## QUESTÃO 05 -
  Fazer um programa que receba um valor n no teclado e determine o maior e o menor termo fornecido.
  A condi ̧cão de termino do programa é quando o usuário digitar zero.
  
   ``` c
   #include <stdio.h>

int main(void) {
  int n = 1, menor, maior;

  
  for(int i = 0; ;i++){
    puts("Digite o termo: ");
    scanf("%d", &n);
    
    if(n == 0){
      break;
    }
    
    if(i == 0){
    menor = n;
    maior = n;
    } else {
      if(n < menor){
        menor = n;
      } 
      if(n > maior){
        maior = n;
      }
    }
    printf("Maior = %d \nMenor = %d\n", maior, menor);
   ```
   
  ## QUESTÃO 06 -
  Escreva um programa que transforme o computador numa urna eletrônica para eleição para presidente
  de um certo país, às quais concorrem os candidatos 5-Paulo e 7-Renata. Cada voto deve ser dado pelo
  número do candidato, permitindo-se ainda o voto 0 para voto em branco. Qualquer voto diferente dos
  já citados é considerado nulo; em qualquer situação, o eleitor deve ser consultado quanto à confirmação
  do seu voto. No final da eleição o programa deve emitir um relatório contendo as porcentagens de
  votação de cada candidato, votos em branco, votos nulos e o candidato eleito. 
  Obs: O código para finalizar a urna (votação) é o usuário digitar algum número negativo.
  
   ``` c
   #include <stdio.h>

int main(void) {
  int voto, paulo = 0, renata = 0, nulo = 0, branco = 0;
  char confirma = 0;

  for(;;){
    printf("Insira o número do canditado: ");
    scanf("%d", &voto);

    if(voto < 0){
      break;
    }
    
    switch (voto) {
      case 5:
      printf("Seu voto é para renata? Digite S para sim e N para não\n");
      scanf("%s", &confirma);
      if(confirma == 'S'){
        renata++;
      }
      if(confirma == 'N'){
        continue;
      }
      break;
      case 7:
      printf("Seu voto é para Paulo? Digite S para sim e N para não\n");
      scanf("%s", &confirma);
      if(confirma == 'S'){
        paulo++;
      }
      if(confirma == 'N'){
        continue;
      }
      break;
      case 0:
      printf("Você quer votar branco? Digite S para sim e N para não\n");
      scanf("%s", &confirma);
      if(confirma == 'S'){
        branco++;
      }
      if(confirma == 'N'){
        continue;
      }
      break;
      default:
       printf("Você quer votar nulo? Digite S para sim e N para não\n");
      scanf("%s", &confirma);
      if(confirma == 'S'){
        nulo++;
      }
      if(confirma == 'N'){
        continue;
      }
      break;
    }
  }
  float total;
  total = renata + paulo + branco + nulo;
  
  
  paulo == renata ? printf("A eleição foi um empate") : paulo > renata ? puts("Paulo foi eleito") : puts("Renata foi eleita");

  printf("%.2f%% dos votos foram de Paulo \n%.2f%% dos votos foram de Renata \n%.2f%% dos votos foram 
  em branco \n%.2f%% dos votos foram nulos", paulo/total*100, renata/total*100, branco/total*100, nulo/total*100);
  return 0;
}
   ```
   
  ## QUESTÃO 07 -
  Para que a divis ̃ao entre 2 n ́umeros possa ser realizada, o divisor n ̃ao pode ser nulo (zero). Escreva
um programa para ler 2 valores e imprimir o resultado da divis ̃ao do primeiro pelo segundo. OBS: O
programa deve validar a leitura do segundo valor (que n ̃ao deve ser nulo). Enquanto for fornecido um
valor nulo a leitura deve ser repetida.
   ``` c
   ```
   
  ## QUESTÃO 08 -
  Uma loja vende seus produtos no sistema entrada mais duas presta ̧c ̃oes, sendo a entrada maior do que
ou igual `as duas presta ̧c ̃oes; estas devem ser iguais, inteiras e as maiores poss ́ıveis. Por exemplo, se o
valor da mercadoria for R$ 270,00, a entrada e as duas presta ̧c ̃oes s ̃ao iguais a R$ 90,00; se o valor da
mercadoria for R$ 302,75, a entrada  ́e de R$ 102,75 e as duas presta ̧c ̃oes s ̃ao iguais a R$ 100,00. Escreva
um programa que receba o valor da mercadoria e forne ̧ca o valor da entrada e das duas presta ̧c ̃oes, de
acordo com as regras acima.
   ``` c
   ```
   
  ## QUESTÃO 09 -
  A série de Fibonacci é formada pela seguinte sequência: 1, 1, 2, 3, 5, 8, 13, 21, 34, 55... etc. Escreva
  um algoritmo que gere a série de Fibonacci até o vigésimo termo.
   ``` c
   ```
   
  ## QUESTÃO 10 -
   ``` c
   ```
   
  ## QUESTÃO 11 -
   ``` c
   ```
   
  ## QUESTÃO 12 -
   ``` c
   ```
   
  ## QUESTÃO 13 -
   ``` c
   ```
   
  ## QUESTÃO 14 -
   ``` c
   ```
   
  ## QUESTÃO 15 -
   ``` c
   ```
   
  ## QUESTÃO 16 -
   ``` c
   ```
   
  ## QUESTÃO 17 -
   ``` c
   ```
   
  ## QUESTÃO 18 -
   ``` c
   ```
   
  ## QUESTÃO 19 -
   ``` c
   ```
   
  ## QUESTÃO 20 -
   ``` c
   ```
   
  ## QUESTÃO 21 -
   ``` c
   ```
   
  ## QUESTÃO 22 -
   ``` c
   ```
   
  ## QUESTÃO 23 -
   ``` c
   ```
   
  ## QUESTÃO 24 -
   ``` c
   ```
   
  ## QUESTÃO 25 -
   ``` c
   ```
   
  ## QUESTÃO 26 -
   ``` c
   ```
   
  ## QUESTÃO 27 -
   ``` c
   ```
   
  ## QUESTÃO 28 -
   ``` c
   ```
