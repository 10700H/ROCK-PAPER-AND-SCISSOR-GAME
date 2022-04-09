#include <iostream>
#include <string>
#include <dos.h>
#include <conio.h>
#include <stdio.h>
using namespace std;
void main1();
void E()
{   system("cls");
   	cout<<"do you want to play again or exit\n";
	cout
	char n;
	n=getch();
	switch(n)
	{
		case '1':
			{
			 system("cls");	
			 main1();
			}break;
		case '2':
		   {
		   	 void exit();
		   }break;
		default:
		   {
		    system("cls");  
		    cout<<"enter again\n";
			E();	
		   }break;	
	}
}
void main1()
{ 
 cout<<"\t\t\t\t\t\t\t !!!! Rock, Paper and Scissor !!!! \t\t\t\t\t\t\t\n";	
 cout<<"1:Rock \n";
 cout<<"2:Scissor\n";
 cout<<"3:paper\n";
 char choice1,choice2;
 cout<<"Enter between the three choices\n";
 cout<<"Enter player 1\n";
 choice1=getch();
 system("cls");
 cout<<"Enter player 2\n";
 choice2=getch();
 system("cls");
 if(choice1=='1' && choice2=='1')
 {
 	cout<<"Draw \n";
 }
 if(choice1=='1' && choice2=='2')
 {
 	cout<<"Rock wins\n";
 }
 if(choice1=='1' && choice2=='3')
 {
 	cout<<"Paper wins\n";
 }
 if(choice1=='2' && choice2=='1')
 {
 	cout<<"Rock wins\n";
 }
 if(choice1=='2' && choice2=='2')
 {
 	cout<<"Draw\n";
 }
 if(choice1=='2' && choice2=='3')
 {
 	cout<<"Scissor wins\n";
 }
 if(choice1=='3' && choice2=='1')
 {
 	cout<<"Paper wins\n";
 }
 if(choice1=='3' && choice2=='2')
 {
 	cout<<"Scissor wins\n";
 }
 if(choice1=='3' && choice2=='3')
 {
 	cout<<"Draw\n";
 }
 E();
}
int main()
{
 main1();
}
