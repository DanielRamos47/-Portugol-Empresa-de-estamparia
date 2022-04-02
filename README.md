# Empresa-de-estamparia PORTUGOL
Esse trabalho consiste em pegar o projeto de outra equipe e fazer alterações que o professor pedir.


programa
{
	
	funcao inicio()//p, m, g, xl
	{
		inteiro linha=0, coluna=0 
		inteiro n=1, n1=0
		real quantidade[2][4], NCamisetas=0.0
		cadeia tamanho, cor, tamanhos[]={"P","M","G","XG"}, cores[]={"Amarela","Verde","Vermelha","Azul"}
		escreva("Tamanhos: 'P', 'M', 'G', 'XG'\nCores: 'Amarela', 'Verde', 'Vermelha', 'Azul'\n")
		

		enquanto(n!=0){
			escreva("\nDigite a quantidade de camisetas que foram produzidas: ")
			leia(n)
			NCamisetas=n+NCamisetas
			se(n!=0){
				escreva("Digite o tamanho da(s) camiseta(s) produzida(s): ")
				leia(tamanho)
				enquanto (tamanho!="P" e tamanho!="M" e tamanho!="G" e tamanho!="XG" e tamanho!="p" e tamanho!="m" e tamanho!="g" e tamanho!="xg"){
					escreva("Digite o tamanho da(s) camiseta(s) produzida(s) corretamente: ")
					leia(tamanho)
					}
				se(tamanho=="P" ou tamanho=="p"){
					quantidade[0][0]=quantidade[0][0]+n
				}
				senao{
					se(tamanho=="M" ou tamanho=="m"){
						quantidade[0][1]=quantidade[0][1]+n
					}
					senao{
						se(tamanho=="G" ou tamanho=="g"){						
							quantidade[0][2]=quantidade[0][2]+n
						}
						senao{
							se(tamanho=="XG" ou tamanho=="xg"){							
								quantidade[0][3]=quantidade[0][3]+n
							}							
						}
					}
				}
				escreva("Insira a cor(es) da(s) camiseta(s): ")
				leia(cor)
				enquanto (cor!="Amarela" e cor!="Verde" e cor!="Vermelha" e cor!="Azul" e cor!="amarela" e cor!="verde" e cor!="vermelha" e cor!="azul"){
					escreva("Insira a cor(es) da(s) camiseta(s) corretamente: ")
					leia(cor)
					}
				se(cor=="amarela" ou cor=="Amarela"){
					quantidade[1][0]=quantidade[1][0]+n
				}
				senao{
					se(cor=="Verde" ou cor=="verde"){
						quantidade[1][1]=quantidade[1][1]+n
					}
					senao{
						se(cor=="Vermelha" ou cor=="vermelha"){
							quantidade[1][2]=quantidade[1][2]+n
						}
						senao{
							se(cor=="Azul" ou cor=="azul"){
								quantidade[1][3]=quantidade[1][3]+n
							}
						}
					}
				}
			}
		}
		
		escreva("\nOrdem crescente de quantidade por cor: ")
		escreva("\n")

			se(quantidade[1][0]<quantidade[1][1] e quantidade[1][1]<quantidade[1][2] e quantidade[1][2]<quantidade[1][3]){
			escreva(quantidade[1][0], " , ",quantidade[1][1], " , ",quantidade[1][2], " , ",quantidade[1][3])
			}senao{
			se(quantidade[1][0]<quantidade[1][1] e quantidade[1][1]<quantidade[1][3] e quantidade[1][3]<quantidade[1][2]){
			escreva(quantidade[1][0], " , ",quantidade[1][1], " , ",quantidade[1][3], " , ",quantidade[1][2])
			}senao{
			se(quantidade[1][0]<quantidade[1][2] e quantidade[1][2]<quantidade[1][1] e quantidade[1][1]<quantidade[1][3]){
			escreva(quantidade[1][0], " , ",quantidade[1][2], " , ",quantidade[1][1], " , ",quantidade[1][3])
			}senao{
			se(quantidade[1][0]<quantidade[1][2] e quantidade[1][2]<quantidade[1][3] e quantidade[1][3]<quantidade[1][1]){
			escreva(quantidade[1][0], " , ",quantidade[1][2], " , ",quantidade[1][3], " , ",quantidade[1][1])
			}senao{
			se(quantidade[1][0]<quantidade[1][3] e quantidade[1][3]<quantidade[1][1] e quantidade[1][1]<quantidade[1][2]){
			escreva(quantidade[1][0], " , ",quantidade[1][3], " , ",quantidade[1][1], " , ",quantidade[1][2])
			}senao{
			se(quantidade[1][0]<quantidade[1][3] e quantidade[1][3]<quantidade[1][2] e quantidade[1][2]<quantidade[1][1]){
			escreva(quantidade[1][0], " , ",quantidade[1][3], " , ",quantidade[1][2], " , ",quantidade[1][1])
			
			
			// Com 1|1
			}senao{
			se(quantidade[1][1]<quantidade[1][0] e quantidade[1][0]<quantidade[1][2] e quantidade[1][2]<quantidade[1][3]){
			escreva(quantidade[1][1], " , ",quantidade[1][0], " , ",quantidade[1][2], " , ",quantidade[1][3])
			}senao{
			se(quantidade[1][1]<quantidade[1][0] e quantidade[1][0]<quantidade[1][3] e quantidade[1][3]<quantidade[1][2]){
			escreva(quantidade[1][1], " , ",quantidade[1][0], " , ",quantidade[1][3], " , ",quantidade[1][2])
			}senao{
			se(quantidade[1][1]<quantidade[1][2] e quantidade[1][2]<quantidade[1][0] e quantidade[1][0]<quantidade[1][3]){
			escreva(quantidade[1][1], " , ",quantidade[1][2], " , ",quantidade[1][0], " , ",quantidade[1][3])
			}senao{
			se(quantidade[1][1]<quantidade[1][2] e quantidade[1][2]<quantidade[1][3] e quantidade[1][3]<quantidade[1][0]){
			escreva(quantidade[1][1], " , ",quantidade[1][2], " , ",quantidade[1][3], " , ",quantidade[1][0])
			}senao{
			se(quantidade[1][1]<quantidade[1][3] e quantidade[1][3]<quantidade[1][0] e quantidade[1][0]<quantidade[1][2]){
			escreva(quantidade[1][1], " , ",quantidade[1][3], " , ",quantidade[1][0], " , ",quantidade[1][2])
			}senao{
			se(quantidade[1][1]<quantidade[1][3] e quantidade[1][3]<quantidade[1][2] e quantidade[1][2]<quantidade[1][0]){
			escreva(quantidade[1][1], " , ",quantidade[1][3], " , ",quantidade[1][2], " , ",quantidade[1][0])
			
			
			// Com 1|2
			}senao{
			se(quantidade[1][2]<quantidade[1][1] e quantidade[1][1]<quantidade[1][2] e quantidade[1][2]<quantidade[1][0]){
			escreva(quantidade[1][2], " , ",quantidade[1][1], " , ",quantidade[1][0], " , ",quantidade[1][3])
			}senao{
			se(quantidade[1][2]<quantidade[1][1] e quantidade[1][1]<quantidade[1][3] e quantidade[1][3]<quantidade[1][0]){
			escreva(quantidade[1][2], " , ",quantidade[1][1], " , ",quantidade[1][3], " , ",quantidade[1][0])
			}senao{
			se(quantidade[1][2]<quantidade[1][0] e quantidade[1][0]<quantidade[1][1] e quantidade[1][1]<quantidade[1][3]){
			escreva(quantidade[1][2], " , ",quantidade[1][0], " , ",quantidade[1][1], " , ",quantidade[1][3])
			}senao{
			se(quantidade[1][2]<quantidade[1][0] e quantidade[1][0]<quantidade[1][3] e quantidade[1][3]<quantidade[1][1]){
			escreva(quantidade[1][2], " , ",quantidade[1][0], " , ",quantidade[1][3], " , ",quantidade[1][1])
			}senao{
			se(quantidade[1][2]<quantidade[1][3] e quantidade[1][3]<quantidade[1][1] e quantidade[1][1]<quantidade[1][0]){
			escreva(quantidade[1][2], " , ",quantidade[1][3], " , ",quantidade[1][1], " , ",quantidade[1][0])
			}senao{
			se(quantidade[1][2]<quantidade[1][3] e quantidade[1][3]<quantidade[1][0] e quantidade[1][0]<quantidade[1][1]){
			escreva(quantidade[1][2], " , ",quantidade[1][3], " , ",quantidade[1][0], " , ",quantidade[1][1])
			
			
			// Com 1|3
			}senao{
			se(quantidade[1][3]<quantidade[1][1] e quantidade[1][1]<quantidade[1][2] e quantidade[1][2]<quantidade[1][0]){
			escreva(quantidade[1][3], " , ",quantidade[1][1], " , ",quantidade[1][2], " , ",quantidade[1][0])
			}senao{
			se(quantidade[1][3]<quantidade[1][1] e quantidade[1][1]<quantidade[1][0] e quantidade[1][0]<quantidade[1][2]){
			escreva(quantidade[1][3], " , ",quantidade[1][1], " , ",quantidade[1][0], " , ",quantidade[1][2])
			}senao{
			se(quantidade[1][3]<quantidade[1][2] e quantidade[1][2]<quantidade[1][1] e quantidade[1][1]<quantidade[1][0]){
			escreva(quantidade[1][3], " , ",quantidade[1][2], " , ",quantidade[1][1], " , ",quantidade[1][0])
			}senao{
			se(quantidade[1][3]<quantidade[1][2] e quantidade[1][2]<quantidade[1][0] e quantidade[1][0]<quantidade[1][1]){
			escreva(quantidade[1][3], " , ",quantidade[1][2], " , ",quantidade[1][0], " , ",quantidade[1][1])
			}senao{
			se(quantidade[1][3]<quantidade[1][0] e quantidade[1][0]<quantidade[1][1] e quantidade[1][1]<quantidade[1][2]){
			escreva(quantidade[1][3], " , ",quantidade[1][0], " , ",quantidade[1][1], " , ",quantidade[1][2])
			}senao{
			se(quantidade[1][3]<quantidade[1][0] e quantidade[1][0]<quantidade[1][2] e quantidade[1][2]<quantidade[1][1]){
			escreva(quantidade[1][3], " , ",quantidade[1][0], " , ",quantidade[1][2], " , ",quantidade[1][1])
			
			
			}}}}}}}}}}}}}}}}}}}}}}}
		escreva("\n")
		escreva("\nOrdem decrescente por tamanho: ")
		escreva("\n")
			
			// Com 1|0
			se(quantidade[0][0]>quantidade[0][1] e quantidade[0][1]>quantidade[0][2] e quantidade[0][2]>quantidade[0][3]){
			escreva(quantidade[0][0], " , ",quantidade[0][1], " , ",quantidade[0][2], " , ",quantidade[0][3])
			}senao{
			se(quantidade[0][0]>quantidade[0][1] e quantidade[0][1]>quantidade[0][3] e quantidade[0][3]>quantidade[0][2]){
			escreva(quantidade[0][0], " , ",quantidade[0][1], " , ",quantidade[0][3], " , ",quantidade[0][2])
			}senao{
			se(quantidade[0][0]>quantidade[0][2] e quantidade[0][2]>quantidade[0][1] e quantidade[0][1]>quantidade[1][3]){
			escreva(quantidade[0][0], " , ",quantidade[0][2], " , ",quantidade[0][1], " , ",quantidade[0][3])
			}senao{
			se(quantidade[0][0]>quantidade[0][2] e quantidade[0][2]>quantidade[0][3] e quantidade[0][3]>quantidade[0][1]){
			escreva(quantidade[0][0], " , ",quantidade[0][2], " , ",quantidade[0][3], " , ",quantidade[0][1])
			}senao{
			se(quantidade[0][0]>quantidade[0][3] e quantidade[0][3]>quantidade[0][1] e quantidade[0][1]>quantidade[0][2]){
			escreva(quantidade[0][0], " , ",quantidade[0][3], " , ",quantidade[0][1], " , ",quantidade[0][2])
			}senao{
			se(quantidade[0][0]>quantidade[0][3] e quantidade[0][3]>quantidade[0][2] e quantidade[0][2]>quantidade[0][1]){
			escreva(quantidade[0][0], " , ",quantidade[0][3], " , ",quantidade[0][2], " , ",quantidade[0][1])
			
			
			// Com 1|1
			}senao{
			se(quantidade[0][1]>quantidade[0][0] e quantidade[0][0]>quantidade[0][2] e quantidade[0][2]>quantidade[0][3]){
			escreva(quantidade[0][1], " , ",quantidade[0][0], " , ",quantidade[0][2], " , ",quantidade[0][3])
			}senao{
			se(quantidade[0][1]>quantidade[0][0] e quantidade[0][0]>quantidade[0][3] e quantidade[0][3]>quantidade[0][2]){
			escreva(quantidade[0][1], " , ",quantidade[0][0], " , ",quantidade[0][3], " , ",quantidade[0][2])
			}senao{
			se(quantidade[0][1]>quantidade[0][2] e quantidade[0][2]>quantidade[0][0] e quantidade[0][0]>quantidade[0][3]){
			escreva(quantidade[0][1], " , ",quantidade[0][2], " , ",quantidade[0][0], " , ",quantidade[0][3])
			}senao{
			se(quantidade[0][1]>quantidade[0][2] e quantidade[0][2]>quantidade[0][3] e quantidade[0][3]>quantidade[0][0]){
			escreva(quantidade[0][1], " , ",quantidade[0][2], " , ",quantidade[0][3], " , ",quantidade[0][0])
			}senao{
			se(quantidade[0][1]>quantidade[0][3] e quantidade[0][3]>quantidade[0][0] e quantidade[0][0]>quantidade[0][2]){
			escreva(quantidade[0][1], " , ",quantidade[0][3], " , ",quantidade[0][0], " , ",quantidade[0][2])
			}senao{
			se(quantidade[0][1]>quantidade[0][3] e quantidade[0][3]>quantidade[0][2] e quantidade[0][2]>quantidade[0][0]){
			escreva(quantidade[0][1], " , ",quantidade[0][3], " , ",quantidade[0][2], " , ",quantidade[0][0])
			
			
			// Com 1|2
			}senao{
			se(quantidade[0][2]>quantidade[0][1] e quantidade[0][1]>quantidade[0][2] e quantidade[0][2]>quantidade[0][0]){
			escreva(quantidade[0][2], " , ",quantidade[0][1], " , ",quantidade[0][0], " , ",quantidade[0][3])
			}senao{
			se(quantidade[0][2]>quantidade[0][1] e quantidade[0][1]>quantidade[0][3] e quantidade[0][3]>quantidade[0][0]){
			escreva(quantidade[0][2], " , ",quantidade[0][1], " , ",quantidade[0][3], " , ",quantidade[0][0])
			}senao{
			se(quantidade[0][2]>quantidade[0][0] e quantidade[0][0]>quantidade[0][1] e quantidade[0][1]>quantidade[0][3]){
			escreva(quantidade[0][2], " , ",quantidade[0][0], " , ",quantidade[0][1], " , ",quantidade[0][3])
			}senao{
			se(quantidade[0][2]>quantidade[0][0] e quantidade[0][0]>quantidade[0][3] e quantidade[0][3]>quantidade[0][1]){
			escreva(quantidade[0][2], " , ",quantidade[0][0], " , ",quantidade[0][3], " , ",quantidade[0][1])
			}senao{
			se(quantidade[0][2]>quantidade[0][3] e quantidade[0][3]>quantidade[0][1] e quantidade[0][1]>quantidade[0][0]){
			escreva(quantidade[0][2], " , ",quantidade[0][3], " , ",quantidade[0][1], " , ",quantidade[0][0])
			}senao{
			se(quantidade[0][2]>quantidade[0][3] e quantidade[0][3]>quantidade[0][0] e quantidade[0][0]>quantidade[0][1]){
			escreva(quantidade[0][2], " , ",quantidade[0][3], " , ",quantidade[0][0], " , ",quantidade[0][1])
			
			// Com 1|3
			}senao{
			se(quantidade[0][3]>quantidade[0][1] e quantidade[0][1]>quantidade[0][2] e quantidade[0][2]>quantidade[0][0]){
			escreva(quantidade[0][3], " , ",quantidade[0][1], " , ",quantidade[0][2], " , ",quantidade[0][0])
			}senao{
			se(quantidade[0][3]>quantidade[0][1] e quantidade[0][1]>quantidade[0][0] e quantidade[0][0]>quantidade[0][2]){
			escreva(quantidade[0][3], " , ",quantidade[0][1], " , ",quantidade[0][0], " , ",quantidade[0][2])
			}senao{
			se(quantidade[0][3]>quantidade[0][2] e quantidade[0][2]>quantidade[0][1] e quantidade[0][1]>quantidade[0][0]){
			escreva(quantidade[0][3], " , ",quantidade[0][2], " , ",quantidade[0][1], " , ",quantidade[0][0])
			}senao{
			se(quantidade[0][3]>quantidade[0][2] e quantidade[0][2]>quantidade[0][0] e quantidade[0][0]>quantidade[0][1]){
			escreva(quantidade[0][3], " , ",quantidade[0][2], " , ",quantidade[0][0], " , ",quantidade[0][1])
			}senao{
			se(quantidade[0][3]>quantidade[0][0] e quantidade[0][0]>quantidade[0][1] e quantidade[0][1]>quantidade[0][2]){
			escreva(quantidade[0][3], " , ",quantidade[0][0], " , ",quantidade[0][1], " , ",quantidade[0][2])
			}senao{
			se(quantidade[0][3]>quantidade[0][0] e quantidade[0][0]>quantidade[0][2] e quantidade[0][2]>quantidade[0][1]){
			escreva(quantidade[0][3], " , ",quantidade[0][0], " , ",quantidade[0][2], " , ",quantidade[0][1])
			
			}}}}}}}}}}}}}}}}}}}}}}}}}
		escreva("\n")
		escreva("\nA quantidade total de camisetas produzidas: ",NCamisetas)
		escreva("\n")
		//a) A quantidade total de camisetas produzidas
		
		//b) A quantidade total de camisetas produzidas agrupadas por cor
		//c) A quantidade total de camisetas produzidas agrupadas por tamanho
		para(linha=0;linha<2;linha++){
			se(linha==0){
				escreva("\nA quantidade de camisetas produzidas por cor:\n")
			}
			senao{
				escreva("\nA quantidade de camisetas produzidas por tamanho:\n")
			}
			para(coluna=0;coluna<4;coluna++){
				se(linha==0){
					escreva(tamanhos[coluna],": ",quantidade[linha][coluna],"\n")
				}
				senao{
					escreva(cores[coluna],": ",quantidade[linha][coluna],"\n")
				}
			}
		}
		//d) A porcentagem de camisetas produzidas agrupadas por cor
		//e) A porcentagem de camisetas produzidas agrupadas por tamanho
		para(linha=0;linha<2;linha++){
			se(linha==0){
				escreva("\nA porcentagem de camisetas produzidas agrupadas por cor:\n")
			}
			senao{
				escreva("\nA porcentagem de camisetas produzidas agrupadas por tamanho:\n")
			}
			para(coluna=0;coluna<4;coluna++){
				se(linha==0){
					escreva(tamanhos[coluna],": ",quantidade[linha][coluna]/NCamisetas*100,"%\n")
				}
				senao{
					escreva(cores[coluna],": ",quantidade[linha][coluna]/NCamisetas*100,"%\n")
}
}
}
}
}
