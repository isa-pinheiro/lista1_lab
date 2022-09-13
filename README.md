# lista1_lab
<p align="center">
  <a href="#questão-02">2</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
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
