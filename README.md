#include <stdio.h>
#include <stdlib.h>

int main()
{

    int nombre1,nombre2,nombre;
    char choix;
    while("choix"){
    printf("donner le premier nombre:");
    scanf("%d",&nombre1);
    getc(stdin);
    printf("donner l'operateur:");
    scanf("%c",&choix);
    printf("donner le deuxieme nombre:");
    scanf("%d",&nombre2);

    switch(choix)
    {
        case'+':
          printf("%d + %d = %d\n",nombre1,nombre2,nombre1 + nombre2);
        break;
        case'-':
          printf("%d - %d = %d\n",nombre1,nombre2,nombre1 - nombre2);

        break;
        case'*':
          printf("%d * %d = %d\n",nombre1,nombre2,nombre1 * nombre2);
        break;
        case'/':
             if(nombre2 !=0)
          printf("%d / %d = %d\n",nombre1,nombre2,nombre1 / nombre2);
            else
          printf("Math Error : Impossible de deviser par 0\n");

        break;
        default : printf("operateur inconnue\n");
    }

    }

    return 0;
}
