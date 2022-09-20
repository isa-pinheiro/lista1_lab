# lista1_lab
<p align="center">
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
 
  
  
  </p>
 
 ## QUESTÃO 02 - 
Faça um programa que leia um valor inteiro decimal X e escreva, na tela, este mesmo valor nas bases
hexadecimal e octal.

 ``` c
 #include <stdio.h>

int main(void) {
  int a;
  printf("Escreva o número em decimal: ");
  scanf("%d", &a);

  printf("Hexadecimal: %x \nOctal: %o", a, a);
}
 ```
 
 ## QUESTÃO 03 -
 Faça um programa capaz de ler um valor real e escrevê-lo com apenas uma casa decimal.
 
 ``` c
 #include <stdio.h>

int main(void) {
  float a;
  printf("Insira um número: ");
  scanf("%f", &a);

  printf("O número é: %.1f", a);
  return 0;
}
 ```
 
## QUESTÃO 04 -
Sabendo que os argumentos da função "printf" podem ser expressões (a+b, a/b, a*b...), e não somente
argumentos, faça um programa capaz de ler um valor inteiro X e escrever seu triplo, seu quadrado, e
seu meio.

 ``` c
 #include <stdio.h>

int main(void) {
  float x;
  printf("Escreva um número: ");
  scanf("%f", &x);

  printf("O triplo: %.2f \nO quadrado: %.2f \nO meio: %.2f", 3 * x, x * x, x / 2);
  return 0;
}
 ```
 
 ## QUESTÃO 05 -
 Escreva um programa que pegue o valor de uma conta de restaurante e imprima o valor total a ser
 pago, considerando que o restaurante cobra 10% de taxa para o garçom.
 
 ``` c
 #include <stdio.h>

int main(void) {
  float valor;
  printf("Qual o valor da conta: ");
  scanf("%f", &valor);

  printf("O valor com os 10%% é: %.2f", 1.1 * valor);
  return 0;
}
 ```
 
 ## QUESTÃO 06 -
 Fazer um programa para ler a altura (em metros) e o sexo de uma pessoa e calcular o seu peso ideal
 através da seguinte fórmula:
  - para homens: 72.7 * altura - 58
  - para mulheres: 62.1 * altura - 44.7

 ``` c
 #include <stdio.h>

int main(void) {
  float altura;
  char sexo;
  printf("Qual a sua altura: ");
  scanf("%f", &altura);
  printf("Digite seu sexo biológico: \nM - Masculino \nF - Feminino\n");
  scanf("%s", &sexo);

  if (sexo == 'M'){
    printf("Seu peso ideal é: %.2f", 72.7 * altura - 58);
  } else if (sexo == 'F'){
    printf("Seu peso ideal é: %.2f", 62.1 * altura - 44.7 );
  } else {
    printf("Algo deu errado, por favor refaça");
  } 
  return 0;
}
 ```
 
 ## QUESTÃO 07 -
 Faça um programa que leia uma quantidade de horas, minutos e segundos e imprima o total de segundos.

 ``` c
 #include <stdio.h>

int main(void) {
  int h, m, s;
  printf("Insira um tempo com o fomato: \n\nhoras:minutos:segundos \n\n(exemplo 25:10:20 = 25 horas, 10 minutos e 20 segundos)\n");
  scanf("%d:%d:%d", &h, &m, &s);
  
  int segundos = 3600 * h + 60 * m + s;
  printf("Em segundos esse tempo é igual a: %d segundos", segundos);
  
  return 0;
}
 ```
 
 ## QUESTÃO 08 -
 Escreva um programa que receba um valor inteiro e apresente o resultado do valor lido elevado ao
 quadrado.
 
 ``` c
 #include <stdio.h>

int main(void) {
  int x;
  printf("Insira um número inteiro: ");
  scanf("%d", &x);
  printf("O quadrado desse número é: %d", x*x);
  
  return 0;
}
 ```
 
 ## QUESTÃO 09 -
 Escreva um programa que leia um valor numérico inteiro e apresente como resultado os seus valores
 sucessor e antecessor.

 ``` c
 #include <stdio.h>

int main(void) {
  int a;
  printf("Insira um inteiro: ");
  scanf("%d", &a);

  printf("O antecessor é: %d \nO sucessor é: %d", a - 1, a + 1);
  return 0;
}
 ```
 
 ## QUESTÃO 10 -
 Escreva um programa que calcule e apresente o valor do volume de um caixa retangular utilizando a
 fórmula VOLUME = COMPRIMENTO * LARGURA * ALTURA.

 ``` c
 #include <stdio.h>

int main(void) {
  float c, l, a;
  printf("Insira o comprimento, a largura e a altura da sua caixa:\n");
  scanf("%f %f %f", &c, &l, &a);

  printf("O volume dessa caixa é: %.2f", c * l * a);
  return 0;
}
 ```
 
 ## QUESTÃO 11 -
 Elabore um programa que apresente o valor da conversão em dólar de um valor lido em real. O
 programa deve solicitar o valor da cotação do dólar e também a quantidade de reais que o usuário
 deseja converter.

 ``` c
 #include <stdio.h>

int main(void) {
  float d, r;
  printf("Insira a cotação atual do dólar: ");
  scanf("%f", &d);
  printf("Insira a quantidade de reais a converter: ");
  scanf("%f", &r);

  printf("Você tem o equivalente a %.2f dólares", r / d);
  
  return 0;
}
 ```
 
 ## QUESTÃO 12 -
 Escreva um programa que peça ao usuário para digitar dois números, obtenha-os do usuário e imprima 
 a soma, o produto, a diferençaa, o quociente e o resto da divisão dos dois números.

 ``` c
 #include <stdio.h>

int main(void) {
  int a, b;
  printf("Insira dois números inteiros: ");
  scanf("%d %d", &a, &b);
  
  printf("A soma: %d \nO produto: %d \nA diferença: %d \nO quociente: %d \nO resto da divisão: %d", a + b, a * b, a - b, a / b, a % b);

  
  return 0;
}
 ```
 
 ## QUESTÃO 13 -
 Escreva um programa que leia duas vari ́aveis A e B e efetue a troca dos valores. O objetivo é que a
 variável A passe a conter o valor de B e a variável B passe a possuir o valor de A. Apresente os valores
 após a efetivação do processamento da troca.

 ``` c
 #include <stdio.h>

int main(void) {
  int a, b, c;
  printf("Insira um valor de a: ");
  scanf("%d", &a);
    printf("Insira um valor de b: ");
  scanf("%d", &b);
  c = a;
  a = b;
  b = c;
  printf("a = %d e b = %d", a, b);
  return 0;
} 
 ```
 
 ## QUESTÃO 14 -
 Escreva um programa que leia uma temperatura em graus Celsius e apresente convertida em graus
 Fahrenheit. A fórmula de versão é F = (9 * C + 160) / 5, sendo F a temperatura Fahrenheit e C a
 temperatura em Celsius.

 ``` c
#include <stdio.h>

int main(void) {
  float c, f;
  printf("Insira a temperatura em Ceulsius: ");
  scanf("%f", &c);
  
  f = (9 * c + 160) / 5;

  printf("A temperatura equivalente em Fahrenheit é: %.2f", f);
  return 0;
}
 ```
 
 ## QUESTÃO 15 -
 Uma empresa contrata um vendedor a R$ 50,25 por dia. Crie um programa que solicite o número de
 dias trabalhados pelo vendedor e imprima o valor líquido a ser pago ao mesmo, sabendo que se ele
 trabalhou até 10 dias não tem direito à gratificação, se ele trabalhou acima de 10 dias e até 20 dias
 tem direito à gratificação de 20%, se ele trabalhou acima de 20 dias tem direito à gratificação de 30%.
 Sempre são descontados 10% de imposto de renda em cima do valor bruto.

 ``` c

 ```
 
 ## QUESTÃO 16 -
 Desenvolva um programa que calcule o salario liquido de um professor. Para elaborar o programa,  ́e
necess ́ario possuir alguns dados, tais como o valor da hora aula, n ́umero de horas trabalhadas no mˆes e
percentual de desconto do INSS. Em primeiro lugar, deve-se estabelecer o seu sal ́ario bruto para fazer
o desconto e ter o valor do salario liquido. Obs.: o programa deve informar o salario bruto e salario
liquido do professor.

 ``` c

 ```
 
 ## QUESTÃO 17 -
 Escrever um programa que receba um valor inteiro do usu ́ario e apresente o seu valor absoluto (m ́odulo).
N ̃ao utilize estrutura de decis ̃ao if.

 ``` c

 ```
 
 ## QUESTÃO 18 -
 Escreva um programa que leia o raio de um c ́ırculo e imprima seu diˆametro, o valor de sua circunferˆencia
 e sua  ́area. Use o valor de 3,14159 para ”pi”. Faça cada um destes c ́alculos dentro da instru ̧c ̃oes (ou
 instruções) printf e use o especificador de conversão %f.

 ``` c

 ```
 
 ## QUESTÃO 19 -
 Escreva um programa que imprima um retˆangulo, uma elipse, uma seta e um losango como se segue:

 ``` c

 ```
 
 ## QUESTÃO 20 -
 Escreva um programa que receba um n ́umero inteiro e ent ̃ao determine e imprima se ele  ́e par ou  ́ımpar.
Obs.: N ̃ao utilizar estrutura de decis ̃ao if.
 ``` c

 ```
 
 ## QUESTÃO 21 -
 Escreva um programa que leia dois inteiros e ent ̃ao determine e imprima se o primeiro  ́e m ́ultiplo do
segundo. Obs.: N ̃ao utilizar estrutura de decis ̃ao if.

 ``` c

 ```
 
 ## QUESTÃO 22 -
 A linguagem C pode representar letras mai ́usculas, letras min ́usculas e uma grande variedade de
s ́ımbolos especiais. O C usa internamente pequenos inteiros para representar cada caractere diferente.

O conjunto de caracteres que um computador utiliza e as representa ̧c ̃oes dos n ́umeros inteiros corres-
pondentes `aqueles caracteres  ́e chamado conjunto de caracteres do computador. Vocˆe pode imprimir

o n ́umero inteiro equivalente `a letra mai ́uscula A, por exemplo, executando a instru ̧c ̃ao

printf(”%d”, ’A’);

Escreva um programa em C que imprima os inteiros equivalentes a algumas letras mai ́usculas, letras
min ́usculas e s ́ımbolos especiais. No m ́ınimo, determine os n ́umeros inteiros equivalentes ao conjunto
seguinte: A BCabc 0 12 $ * + / e o caractere espa ̧co em branco.

 ``` c

 ```
 
 ## QUESTÃO 23 -
 Escreva um programa que receba a entrada de um n ́umero de trˆes d ́ıgitos, separe o n ́umero em seus
d ́ıgitos componentes e reconstrua um n ́umero com os componentes na ordem inversa. Exemplo: para
entrada de 123, a resposta do programa seria 321.

 ``` c

 ```
 
 ## QUESTÃO 24 -
 Escreva um programa que calcule o produto entre um valor dado x por 2 elevado a um valor dado n.
Obs.: Utilize operadores bin ́arios.

 ``` c

 ```
 
 ## QUESTÃO 25 -
 Escreva um programa que leia um tempo em segundos e imprima quantas horas, minutos e segundos
h ́a neste tempo.

 ``` c

 ```
 
 ## QUESTÃO 26 -
 26. Fazer um programa para ler as coordenadas x e y de dois pontos e calcular a distˆancia entre os dois
pontos no plano. (Utilize a fun ̧c ̃ao sqrt (numero), biblioteca math.h).

 ``` c

 ```
 
 ## QUESTÃO 27 -
 Escreva um programa que solicite 3 n ́umeros em ponto flutuante e imprima a m ́edia aritm ́etica e
geom ́etrica. (Utilize a fun ̧c ̃ao pow(base, expoente) da biblioteca math.h).

 ``` c

 ```
