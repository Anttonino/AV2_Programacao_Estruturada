# Cadastros-em-C-
Trabalho Acadêmico de programação estruturada do Centro Universitário Unicarioca.

Codigo para o calculo da média

#include <stdio.h>
#include <stdlib.h>
#include <iostream>
#include <string.h>

using namespace std;


void media (){
	
	// Declaração de variavies internas
	
	float av1,av2,av3,media;
	
	// Solicitação de dados 
	
	cout<<"AV1: "; cin>>av1;
	cout<<"AV2: "; cin>>av2;
	cout<<"AV3: "; cin>>av3;

	cout<< " " <<endl;
	
	// Operação de Media 
	

	
	/*
	condição sendo satisfeita para AV2 e AV3.
	*/
	
	
	if (av1<=av3 && av2>=av1) 
	{
	media = (av2+av3)/2;
	}
	
		/*
	condição sendo satisfeita para AV1 e AV3.
	*/
	
	else if (av2<=av3 && av1>=av2)
	{
	media = (av1+av3)/2;	
		
	}
	
		/*
	condição sendo satisfeita para AV1 e AV2.
	*/
	else if (av1>=av3 && av2>=av3)
	{
		media = (av1+av2)/2;
		
	}
	
	
	//Exibição do Resultado da media.

	cout<<"Media Final do Aluno:  " <<media<<endl<<endl;


}


// Execução do programa principal 

main (){
	
	media ();
	
			
		return (0);
		system ("pause");

}
