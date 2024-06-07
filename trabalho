#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main(void) {
  // atribuições
  int i, y, num, prov, vetor[6];
  srand(time(0));

  // sorteando os números
  for (i = 0; i < 6; i++) {
    num = rand() % 101;
    // verificando se o número já foi sorteado
    for (y = 0; y < 6; y++) {
      if (num != vetor[y]) {
        vetor[i] = num;
      }
    }
  }

  // ordenando o vetor
  for (i = 0; i < 6; i++) {
    for (y = 0; y < 6; y++) {
      if (vetor[i] < vetor[y]) {
        prov = vetor[i];
        vetor[i] = vetor[y];
        vetor[y] = prov;
      }
    }
  }

  // imprimindo o vetor
  for (i = 0; i < 6; i++) {
    printf("%d\n", vetor[i]);
  }
  return 0;
}
