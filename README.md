#include<iostream>
#include<cstdlib>

using namespace std;

int main(){
	int opcion;
	float valor;
	
	do{
		cout<<"\t\t\t****CONVERTOR DE DIVISAS**** \n"<<endl;
		cout<<"\t\t\t1.Libras\n \t\t\t2.Dolares americanos \n \t\t\t3.Euros \n "<<endl;
		cout<<"Ingresa una opcion: ";
		cin>>opcion;
		
		switch(opcion){
			case 1: cout<<"\tIngrese la cantidad en pesos mexicanos a convertir: ";  // precio compra $27.56
					cin>>valor; valor=valor/27.56;
					cout<<"\tLa cantidad en libras es: "<<valor<<endl<<endl;
					system("pause");
					break;
			case 2: cout<<"\tIngrese la cantidad en pesos mexicanos a convertir: ";  //precio compra $19.82
					cin>>valor; valor=valor/19.82;
					cout<<"\tLa cantidad en dolares es: "<<valor<<endl<<endl;    
					system("pause");
					break;
			case 3: cout<<"\tIngrese la cantidad en pesos mexicanos a convertir: ";  //precio compra $23.98
					cin>>valor; valor=valor/23.98;
					cout<<"\tLa cantidad en euros es: "<<valor<<endl<<endl;
					system("pause");
					break;		
			default: cout<<"Opcion invalida";
					break;
		}
		system("cls");	
		
	}while(opcion<=3);
	return 0;
}
