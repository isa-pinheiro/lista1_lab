# lista1_lab

 
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
Sabendo que os argumentos da função "printf" podem ser expressões (a+b, a/b, a*b...) e não somente
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
 #include <stdio.h>

int main(void) {
  int d;
  printf("Insira a quantidade de dias trabalhados: ");
  scanf("%d", &d);

  if(d <= 10){
    printf("Seu salário líquido final é: %.2f", 0.9 * 50.25 * d);
  } else if(d <= 20){
    printf("Seu salário líquido final é: %.2f", 0.9 * (1.2 * 50.25 * d));
  } else if(d <= 30){
    printf("Seu salário líquido final é %.2f", 0.9 * (1.3 * 50.25 * d));
  } else{
    printf("Quantidade de dias inválida");
  }
  return 0;
}
 ```
 
 ## QUESTÃO 16 -
 Desenvolva um programa que calcule o salário líquido de um professor. Para elaborar o programa, é
 necessário possuir alguns dados, tais como o valor da hora aula, número de horas trabalhadas no mês e
 percentual de desconto do INSS. Em primeiro lugar, deve-se estabelecer o seu salário bruto para fazer
 o desconto e ter o valor do salário líquido. 
 Obs: o programa deve informar o salário bruto e salário líquido do professor.

 ``` c
 #include <stdio.h>

int main(void) {
  float ha, inss, ht;
  printf("Insira o valor de hora aula: ");
  scanf("%f ", &ha);
  printf("Insira a quantidade de horas trabalhadas: ");
  scanf("%f", &ht);
  printf("Insira o percentual de desconto do issec sem o %%: ");
  scanf("%f", &inss);

  printf("O salário desse professor nesse mês foi: \nSálario bruto: %.2f \nSalário líquido: %.2f", ha * ht, ha * ht * (1 - inss/100));
  return 0;
}
 ```
 
 ## QUESTÃO 17 -
 Escrever um programa que receba um valor inteiro do usuário e apresente o seu valor absoluto (módulo).
 Não utilize estrutura de decisão if.

 ``` c
 #include <stdio.h>
 #include <stdlib.h>

int main(void) {
  int n;
  printf("Insira um número inteiro: ");
  scanf("%d", &n);

  printf("O valor em módulo desse número é: %d", abs(n));
  return 0;
}
 ```
 
 ## QUESTÃO 18 -
 Escreva um programa que leia o raio de um círculo e imprima seu diâmetro, o valor de sua circunferência
 e sua área. Use o valor de 3,14159 para ”pi”. Faça cada um destes cálculos dentro da instruçãos (ou
 instruções) printf e use o especificador de conversão %f.

 ``` c
 #include <stdio.h>

int main(void) {
  float pi = 3.14159, r;
  printf("Insira o raio do círculo: ");
  scanf("%f", &r);

  printf("\nA circunferência desse círculo é: %.2f \nA área desse círculo é: %.2f", 2 * pi * r, pi * r * r);

  
  return 0;
}
 ```
 
 ## QUESTÃO 19 -
 Escreva um programa que imprima um retângulo, uma elipse, uma seta e um losango.

 ``` c
 #include <stdio.h>

int main(void) {
  printf("******** \t\t   ***   \t\t   *   \t\t     *     \n");
  printf("*      * \t\t  *   *  \t\t  ***  \t\t    * *    \n");
  printf("*      * \t\t *     * \t\t ***** \t\t   *   *   \n");
  printf("*      * \t\t *     * \t\t   *   \t\t  *     *  \n");
  printf("*      * \t\t *     * \t\t   *   \t\t *       * \n");
  printf("*      * \t\t *     * \t\t   *   \t\t  *     *  \n");
  printf("*      * \t\t *     * \t\t   *   \t\t   *   *   \n");
  printf("*      * \t\t *     * \t\t   *   \t\t    * *    \n");
  printf("******** \t\t   ***   \t\t   *   \t\t     *     \n");
  return 0;
}
 ```
 
 ## QUESTÃO 20 -
 Escreva um programa que receba um número inteiro e então determine e imprima se ele é par ou ímpar.
 Obs.: Não utilizar estrutura de decisão if.
 
 ``` c
 #include <stdio.h>

int main(void) {
  int n;
  printf("Insira um número inteiro: ");
  scanf("%d", &n);

  (n % 2) ? printf("Esse número é ímpar.") : printf("Esse número é par.");
  return 0;
}
 ```
 
 ## QUESTÃO 21 -
 Escreva um programa que leia dois inteiros e então determine e imprima se o primeiro é múltiplo do segundo. 
 Obs.: Não utilizar estrutura de decisão if.

 ``` c
 #include <stdio.h>

int main(void) {
  int x, y;
  printf("Insira dois inteiros: ");
  scanf("%d %d", &x, &y);

  (x % y) ? printf("Não é múltiplo") : printf("É múltiplo");
  return 0;
}
 ```
 
 ## QUESTÃO 22 -
 A linguagem C pode representar letras maiúsculas, letras minúsculas e uma grande variedade de
 símbolos especiais. O C usa internamente pequenos inteiros para representar cada caractere diferente.
 O conjunto de caracteres que um computador utiliza e as representações dos números inteiros correspondentes
 àqueles caracteres é chamado conjunto de caracteres do computador. 
 Você pode imprimir o número inteiro equivalente à letra maiúscula A, por exemplo, executando a instrução:

                                         printf(”%d”, ’A’);
 
 Escreva um programa em C que imprima os inteiros equivalentes a algumas letras mai ́usculas, letras
 minúsculas e s ́ımbolos especiais. No m ́ınimo, determine os n ́umeros inteiros equivalentes ao conjunto
 seguinte: ABCabc012$*+/ e o caractere espaço em branco.

 ``` c
 #include <stdio.h>

int main(void) {
  printf("%d \n", 'A');
  printf("%d \n", 'a');
  printf("%d \n", 'B');
  printf("%d \n", 'b');
  printf("%d \n", 'C');
  printf("%d \n", 'c');
  printf("%d \n", ' ');
  printf("%d \n", '0');
  printf("%d \n", '1');
  printf("%d \n", '2');
  printf("%d \n", '$');
  printf("%d \n", '*');
  printf("%d \n", '+');
  printf("%d \n", '/');
  
  return 0;
}
 ```
 
 ## QUESTÃO 23 -
 Escreva um programa que receba a entrada de um número de três dígitos, separe o número em seus
 dígitos componentes e reconstrua um número com os componentes na ordem inversa. 
 Exemplo: para entrada de 123, a resposta do programa seria 321.

 ``` c
 #include <stdio.h>

int main(void) {
  int n;
  printf("Insira um número de 3 dígitos: ");
  scanf("%d", &n);
  int i1, i2, i3;
  i1 = n % 10;
  i2 = (n % 100)/10;
  i3 = n/100;
  printf("%d%d%d", i1, i2, i3);
  return 0;
}
 ```
 
 ## QUESTÃO 24 -
 Escreva um programa que calcule o produto entre um valor dado x por 2 elevado a um valor dado n.
 Obs: Utilize operadores binários.

 ``` c
 #include <stdio.h>

int main(void) {
  int x = 1, n;
  printf("Insira o valor de n: ");
  scanf("%d", &n);

  for(int i = 1; i <= n; i++){
    x = x * 2;
  }
  
  printf("O valor de x é: %d", x);
  return 0;
} 
 ```
 
 ## QUESTÃO 25 -
 Escreva um programa que leia um tempo em segundos e imprima quantas horas, minutos e segundos
 há neste tempo.

 ``` c
 #include <stdio.h>

int main(void) {
  int s;
  printf("Insira os segundos: ");
  scanf("%d", &s);
  int h, min, seg;
  h = s / 3600;
  min = (s % 3600)/60;
  seg = s % 60;
  printf("%d horas %d minutos e %d segundos", h, min, seg);
  return 0;
}
 ```
 
 ## QUESTÃO 26 -
 Fazer um programa para ler as coordenadas x e y de dois pontos e calcular a distância entre os dois
 pontos no plano. 
 (Utilize a função sqrt (numero), biblioteca math.h).

 ``` c
#include <stdio.h>
#include <math.h>

int main(void) {
  float x1, x2, y1, y2;
  printf("Insira a primeira coordenada no formato x,y: ");
  scanf("%f,%f", &x1, &y1);
  printf("Insira a segunda coordenada no formato x,y: ");
  scanf("%f,%f", &x2, &y2);

  float d;
  d = sqrt(pow(x2 - x1, 2) + pow(y2 - y1, 2));

  printf("A distância entre os pontos é: %f", d);
  return 0;
}
 ```
 
 ## QUESTÃO 27 -
 Escreva um programa que solicite 3 números em ponto flutuante e imprima a média aritmética e
 geométrica. 
 (Utilize a função pow(base, expoente) da biblioteca math.h).

 ``` c
 #include <stdio.h>
#include <math.h>

int main(void) {
  float a, b, c;
  printf("Insira três números reais: ");
  scanf("%f %f %f", &a, &b, &c);

  float ma, mg;
  ma = (a + b + c)/3;
  mg = pow(a*b*c, 1.0/3.0);
  printf("A média aritmética é: %f \nA média geométrica é: %f", ma, mg);
  return 0;
}
 ```
