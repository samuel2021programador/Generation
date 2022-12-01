# Generation
atividades generation

Exercícios com Vetores[ ] e Matrizes [ ][ ] 

ATIVIDADE 1 

programa
{
	
	funcao inicio()
	{
				/*1. Faça um programa que crie um vetor por leitura com 5 valores de pontuação de uma
		atividade e o escreva em seguida. Encontre após a maior pontuação e a apresente.*/
		
		inteiro pontuacao[5],x, maior = 0 
		para (x=0;x<5;x++){
			escreva("coloque uma pontuação:  ")
			leia(pontuacao[x])
			}

		para (x=0;x<5;x++){
			se (maior<pontuacao[x]){
				
				maior = pontuacao[x]
				}
		}
		escreva("\n A maior pontuação é:  ", maior )
	}
}

ATIVIDADE 2 
programa
{
	
	funcao inicio()
	{
		/*2. Um dado é lançado 10 vezes e o valor correspondente é anotado. Faça um programa
		que gere um vetor com os lançamentos, escreva esse vetor. A seguir determine e
		imprima a média aritmética dos lançamentos, contabilize e apresente também
		quantas foram as ocorrências da maior pontuação.*/

		inteiro pontuacao[10],x,Maior = 0, repeticao = 0
		real MEDIA = 0.0, somaTotal = 0.0
		para (x=0;x<10;x++){
			escreva("coloque uma pontuação:  ")
			leia(pontuacao[x])
			somaTotal += pontuacao[x]
				se (Maior<pontuacao[x]){			
				Maior = pontuacao[x]
				}
		}
			para (x=0;x<10;x++){
				se (Maior==pontuacao[x]){			
				repeticao++
				}
			}
			MEDIA = somaTotal/10
			escreva("\n a média é :  ",MEDIA)
			escreva("\n A quantidade de vezes que o maior numero foi repetido é :  ", repeticao)
			escreva("\n A maior pontuação é:  ", Maior )
	}
}

ATIVIDADE 3 
programa
{
	
	funcao inicio()
	{
		/*3. Escreve um programa que lê duas matrizes N1 (4,6) e N2(4,6) e cria:
		a) Uma matriz M1 cujos elementos serão as somas dos elementos de mesma posição
		das matrizes N1 e N2;
		b) Uma matriz M2 cujos elementos serão as diferenças dos elementos de mesma
		posição das matrizes N1 e N2.*/

		inteiro N1[2][3],N2[2][3],M1[2][3],M2[2][3],C,L,cont1 = 0,cont2 = 0 
		
		para(L=0;L<2;L++){
			para(C=0;C<3;C++){

			escreva("Digite os valores da N1: ")
			leia(N1[L][C])
			}
		}

		
		para(L=0;L<2;L++){
			para(C=0;C<3;C++){

			escreva("Digite os valores da N2: ")
			leia(N2[L][C])
			}
		}
		
		
		para(L=0;L<2;L++){
			para(C=0;C<3;C++){
				cont1++
				M1[L][C] = N1[L][C] + N2[L][C]
				escreva("\n a soma da matriz N1 com N2 é:",cont1, "2 = ", M1[L][C])
			}
		}

			
		para(L=0;L<2;L++){
			para(C=0;C<3;C++){
				cont2++
				M2[L][C] = N1[L][C] - N2[L][C]
				escreva("\n a diferença da matriz N1 com N2 é:",cont2, " = ", M2[L][C])
			}
		}
			
	}
}

ATIVIDADE 4 
programa
{
	
	funcao inicio()
	{
		/*4. Crie um programa que receba valores do usuário para preencher uma matriz 3X3, e
		em seguida, exiba a soma dos valores dela e a soma dos valores da primeira
		diagonal, ou seja, diagonal principal.*/

		inteiro M1 [3][3],C,L,cont = 0 ,somaTotal = 0 ,diagonal 

		para (L=0;L<3;L++){
			para(C=0;C<3;C++){
			cont++
			escreva("\n DIGITE UM NUMERO : ")
			leia(M1[L][C])
			somaTotal += M1[L][C] 
		}
			}

			diagonal = M1[0][0] + M1[1][1] + M1[2][2] 
			escreva("\n a SOMA da matriz M1 com M2 é:",somaTotal)
			escreva("\n O valor da diagonal  é :",diagonal)




	}
}

