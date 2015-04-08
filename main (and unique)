	

     
    #include<stdio.h>
    #define MAX_STRLEN 256
    #define SIN_TIPO float
     
     
    /*Source code from the web and Uriel Cambrón Hernández*/
     
    int main() {
            SIN_TIPO afd[20][20];
            char a_1[MAX_STRLEN];
            char b[MAX_STRLEN];
            int con;
            int i;
            int j;
            int k;
            float l;
            int opc;
            char x[MAX_STRLEN][10][10];
            for (i=1;i<=10;i+=1) {
                    for (j=1;j<=10;j+=1) {
                            x[i][j]="0";
                    }
            }
            do {
                    printf("Menu\n");
                    printf("1.-Input nodes\n");
                    printf("2.-Input tags\n");
                    printf("3.-Input unions\n");
                    printf("4.-Show AFN Lenguaje\n");
                    printf("5.-Get AFD\n");
                    printf("6.-Get Regular Expresion\n");
                    printf("7.-Exit\n");
                    do {
                            scanf("%i",&opc);
                    } while (!(opc==1 || opc==2 || opc==3 || opc==4 || opc==6 || opc==5 || opc==7));
                    switch (opc) {
                    case 1:
                            printf("¿How many nodos? (1-10)?:  ");
                            scanf("%i",&k);
                            k=k+1;
                            for (i=2;i<=k;i+=1) {
                                    j=1;
                                    printf("Write nodos: %f",i-1);
                                    scanf("%s",x[i][j]);
                            }
                            break;
                    case 2:
                            printf("¿How many tags?(1-10)?:  ");
                            scanf("%f",&l);
                            l=l+1;
                            for (i=2;i<=l;i+=1) {
                                    j=1;
                                    printf("Write tags:  %f",i-1);
                                    scanf("%s",x[j][i]);
                            }
                            break;
                    case 3:
                            con=1;
                            for (i=2;i<=k;i+=1) {
                                    for (j=2;j<=l;j+=1) {
                                            printf("¿What nodo(s) points %s in the tag %s?:  ",x[i][j-con],x[1][j]);
                                            scanf("%s",x[i][j]);
                                            con=con+1;
                                    }
                                    con=1;
                            }
                            for (i=1;i<=k;i+=1) {
                                    for (j=1;j<=l;j+=1) {
                                            printf("%s  ",x[i][j]);
                                    }
                                    printf(" \n");
                            }
                            break;
                    case 4:
                            a_1=x[2][1];
                            b=x[k][1];
                            printf("¿Where is the inicial node?  ");
                            scanf("%s",a_1);
                            printf("¿What is the final node?
                            printf("L(A)=(");
                            printf("{");
                            for (i=2;i<=k;i+=1) {
                                    printf("[%s],",x[i][1]);
                            }
                            printf("},E,{");
                            for (j=2;j<=l;j+=1) {
                                    printf("%s,",x[1][j]);
                            }
                            printf("},%s,%s)\n",a_1,b);
                            break;
                    case 5:
                            printf("%s\n",a_1);
                            break;
                    case 6:
                            printf("%s\n",a_1);
                            break;
                    }
            } while (opc!=7);
            return 0;
    }

