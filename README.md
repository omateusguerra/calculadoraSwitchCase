# calculadoraSwitchCase
Aprendendo a utilizar o "switch case", desenvolvi uma calculadora com as seguintes operações: soma, subtração, divisão e multiplicação.

#include <stdio.h>
#include <locale.h>

int main()
{
    int placarTimeUm = 0;
    int placarTimeDois = 0;

    setlocale(LC_ALL,"Portuguese");    

    printf("SOFTWARE DE RESULTADO DE PARTIDA DE FUTEBOL! \n");
   
    printf("Digite o placar do primeiro time: \n");
    scanf("%d", &placarTimeUm);
   
    printf("Digite o placar do segundo time: \n");
    scanf("%d", &placarTimeDois);
   
    if (placarTimeUm > placarTimeDois) {
        printf("Time 1 venceu por: %d à %d!", placarTimeUm, placarTimeDois);
    }else if(placarTimeDois > placarTimeUm){
        printf("Time 2 venceu por: %d à %d!", placarTimeDois, placarTimeUm);
    }else {
        printf("A partida terminou empatada em: %d à %d!", placarTimeDois, placarTimeUm);
    };
   
    return 0;
};
