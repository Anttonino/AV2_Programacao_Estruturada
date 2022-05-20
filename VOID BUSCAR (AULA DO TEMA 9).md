# Cadastros-em-C-
Trabalho Acadêmico de programação estruturada do Centro Universitário Unicarioca.



07:46 19/05/2022
// TEMA 9 - Pré-compilação e compilação [Registros com Matriz e Vetores]

#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include <iostream>
using namespace std;

typedef struct{
	
	char nome [20], end[20], tel[15];
	int idade;
	
}Funcionario;

Funcionario func[10];
int total=0;


void Cadastrar(){
	system ("cls");
		cout<<"PROGRAMA"<<endl;
		cout<<"[1] CADASTRAR FUNCIONARIO"<<endl;	
		
		if (total<10){
		
		cout<<"Nome: ";      cin>>func[total].nome;
		cout<<"Idade: ";  	 cin>>func[total].idade;
		cout<<"Endereco: ";  cin>>func[total].end;
		cout<<"Telefone: ";  cin>>func[total].tel;
		total++;	
		}
		else{
		
		cout<<"SISTEMA LOTADO"<<endl;	
		}
	system ("pause");
		
}

void Buscar (){
	
	system ("cls");
		cout<<"PROGRAMA"<<endl;
		cout<<"[2] BUSCAR FUNCIONARIO"<<endl;
		
		if (total== 0){
			
		cout<<"SISTEMA VAZIO"<<endl;
							
		} 
		
		else {
			char nome[20];
			cout<<"Nome para busca: "; cin>>nome;
		
		for (int i=0; i<total; i++)	{
			
			if (strcmp(func[i].nome,nome)==0){
				
				cout<<"Idade: "<<func[i].idade<<endl;
				cout<<"Endereco: "<<func[i].end<<endl;
				cout<<"Telefone: "<<func[i].tel<<endl<<endl;
			}
		}
			
		}
	
	system ("pause");	
	
	
}

main (){
	int op;
	do {
		
		cout<<"PROGRAMA"<<endl;
		cout<<"[1] CADASTRAR FUNCIONARIO"<<endl;
		cout<<"[2] BUSCAR FUNCIONARIO"<<endl;
		cout<<"[0] SAIR" <<endl;
		cout<<"OPCAO: ";  cin>>op;
		
		switch (op){
			
			case 1: Cadastrar();
			break;
			case 2: Buscar();
			break;
		}
		}

	while(op!=0);	
	
}
=================================================================================================================================================================
