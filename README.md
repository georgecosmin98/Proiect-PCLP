// Ver 1.0.cpp : Defines the entry point for the console application.
//

#include "stdafx.h"
#include <iostream>
#include <fstream>
#include <string>
#include <climits> //Necesar pentru a putea testa daca un caracter e cifra (int_max)
using namespace std;

int an,aux;
void testCifra(int &cif)
{// input validation
while (cin.fail())
{
	cin.clear(); // clear input buffer to restore cin to a usable state
	cin.ignore(INT_MAX, '\n'); // ignore last input
	cout << "Introdu o valoare valida:";
	cin >> cif;
	cout << endl;
}
}

int main()
{
	aux = 0;
	int x = -1;
	while (x!=0)
	{  
		cout << "1.Stoc substante" << endl;
		cout << "2.Bilant" << endl;
		cout << "3.Depozit" << endl;
		cout << "4.Suprafete agricole" << endl;
		cout << "5.Tratamente" << endl;
		cout << "6.Stare" << endl;
		cout << "7.Fonduri Europene" << endl;
		cout << "8.Personal" << endl;
		cout << "9.Utilaje" << endl;
		cout << "0.Iesire" << endl;
		cout << "Introduceti cifra corespunzatoare submeniului pe care doriti sa-l accesati: ";
		cin >> aux;
		cout << endl;
		testCifra(aux);
		x = aux;
		
		system("cls");
		if (x==1)
		{
			int x1 = -1;
			while (x1 != 0)
			{
				cout << "1.Afisare stoc substante" << endl;
				cout << "2.Adaugare substanta in stoc" << endl;
				cout << "3.Stergere substanta din stoc" << endl;
				cout << "0.Inapoi la meniul principal" << endl;
				cout << "Introduceti cifra corespunzatoare submeniului pe care doriti sa-l accesati: ";
				cin >> aux;
				cout << endl;
				testCifra(aux);
				x1 = aux;
				
				system("cls");
			}
		}

		if(x==2)
		{
			int x2 = -1;
			while (x2 != 0)
			{
				cout << "1.Bilant venituri" << endl;
				cout << "2.Bilant cheltuieli" << endl;
				cout << "3.Bilant total" << endl;
				cout << "0.Inapoi la meniul principal" << endl;
				cout << "Introduceti cifra corespunzatoare submeniului pe care doriti sa-l accesati: ";
				cin >> aux;
				cout << endl;
				testCifra(aux);
				x2 = aux;
				
				system("cls");
			}
		}


		if (x == 3)
		{
			int x3 = -1;
			while (x3 != 0)
			{
				cout << "1.Afisarea produselor din depozit" << endl;
				cout << "2.Adaugarea produselor in depozit" << endl;
				cout << "3.Stergerea produselor din depozit" << endl;
				cout << "0.Inapoi la meniul principal" << endl;
				cout << "Introduceti cifra corespunzatoare submeniului pe care doriti sa-l accesati: ";
				cin >> aux;
				cout << endl;
				testCifra(aux);
				x3 = aux;
				
				system("cls");
			}
		}


		if (x == 4)
		{
			int x4 = -1;
			while (x4 != 0)
			{
				cout << "1.Afisarea suprafetelor agricole detinute" << endl;
				cout << "2.Cumpararea unei suprafete agricole" << endl;
				cout << "3.Vanzarea unei suprafete agricole" << endl;
				cout << "0.Inapoi la meniul principal" << endl;
				cout << "Introduceti cifra corespunzatoare submeniului pe care doriti sa-l accesati: ";
				cin >> aux;
				cout << endl;
				testCifra(aux);
				x4 = aux;
				
				system("cls");
			}
		}


		if (x == 5)
		{
			int x5 = -1;
			while (x5 != 0)
			{
				cout << "1.Afisarea tratamentelor efectuate" << endl;
				cout << "2.Adaugarea unui tratament" << endl;
				cout << "0.Inapoi la meniul principal" << endl;
				cout << "Introduceti cifra corespunzatoare submeniului pe care doriti sa-l accesati: ";
				cin >> aux;
				cout << endl;
				testCifra(aux);
				x5 = aux;
				
				system("cls");
			}
		}
	
	

		if (x == 6)
		{
			int x6 = -1;
			while (x6 != 0)
			{
				cout << "1.Afisarea starii suprafetelor agricole" << endl;
				cout << "2.Schimbarea starii suprafetelor agricole" << endl;
				cout << "0.Inapoi la meniul principal" << endl;
				cout << "Introduceti cifra corespunzatoare submeniului pe care doriti sa-l accesati: ";
				cin >> aux;
				cout << endl;
				testCifra(aux);
				x6 = aux;

				system("cls");
			}
		}



		if (x == 7)
		{
			int x7 = -1;
			while (x7 != 0)
			{
				cout << "1.Afisarea fondurilor accesate" << endl;
				cout << "2.Adaugarea fondului accesat" << endl;
				cout << "0.Inapoi la meniul principal" << endl;
				cout << "Introduceti cifra corespunzatoare submeniului pe care doriti sa-l accesati: ";
				cin >> aux;
				cout << endl;
				testCifra(aux);
				x7 = aux;
				
				system("cls");
			}
		}


		if (x == 8)
		{
			int x8 = -1;
			while (x8 != 0)
			{
				cout << "1.Afisarea personalului" << endl;
				cout << "2.Adaugarea unui angajat" << endl;
				cout << "3.Stergerea unui angajat" << endl;
				cout << "0.Inapoi la meniul principal" << endl;
				cout << "Introduceti cifra corespunzatoare submeniului pe care doriti sa-l accesati: ";
				cin >> aux;
				cout << endl;
				testCifra(aux);
				x8 = aux;

				system("cls");
			}
		}

	

		if (x == 9)
		{
			int x9 = -1;
			while (x9 != 0)
			{
				cout << "1.Afisarea utilajelor" << endl;
				cout << "2.Adaugarea cheltuielilor cu utilaje" << endl;
				cout << "3.Adauga utilaje" << endl;
				cout << "4.Sterge utilaj" << endl;
				cout << "0.Inapoi la meniul principal" << endl;
				cout << "Introduceti cifra corespunzatoare submeniului pe care doriti sa-l accesati: ";
				cin >> aux;
				cout << endl;
				testCifra(aux);
				x9 = aux;

				system("cls");
			}
		}

     }
 


    return 0;
}

