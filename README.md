# lista2_lab

<p align="center">
  <a href="#questão-01--">01</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-02--">02</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-03--">03</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-04--">04</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-05--">05</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-06--">06</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-07--">07</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-08--">08</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-09--">09</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-10--">10</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-11--">11</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-12--">12</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-13--">13</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-14--">14</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-15--">15</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-16--">16</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-17--">17</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-18--">18</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-19--">19</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-20--">20</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-21--">21</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-22--">22</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-23--">23</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-24--">24</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-25--">25</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-26--">26</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-27--">27</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#questão-28--">28</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  
  </p>
  
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
  
   ## QUESTÃO 03 -
   ``` c
   ```
   
   ## QUESTÃO 04 -
   ``` c
   ```
   
   ## QUESTÃO 05 -
   ``` c
   ```
   
   ## QUESTÃO 06 -
   ``` c
   ```
