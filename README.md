# LBYEC72-EB1-Cruz-Pamittan

LBYEC72 EB1
Members:
Danielle Cruz
Bea Pamittan

Brief description of the project:


#include <stdio.h>
#include <string.h>
#include <math.h>
#include <iostream>

using namespace std;

typedef struct{
	string Username;
	string Firstname;
	string Lastname;
	string Password;
	string Password2;
	int Idno;
}m;

main(){
	int i=0, c, quantity=1, loggedin=0, temp, a, f, r;
	m student[100];
	string s;
	
	do{
	system("cls");
	cout<<"~~~~~~~~~~ANIMOO SIS~~~~~~~~~~"<<endl;
	cout<<"\n\n";
	
	cout<<"1. Log In\n";
	cout<<"2. Sign up\n";
	cin>>c;
	
	loggedin=0;
	
	if(c==1){
		cout<<"~~~~~~~~~~Log In~~~~~~~~~~"<<endl;
		cout<<"username:";
		cin>>s;
	f=0;
	for(int i=0; i<quantity; i++){
		if(s.find(student[i].Username) <= 1){
			cout<<endl;
			temp=i;
	}}
		cout<<"Password:";
		cin>>s;
		if(student[temp].Password==s){
			i=temp;
			f++;
			loggedin++;
		}
	
	if(f==0){
		cout<<endl<<"INCORRECT PASSWORD OR USERNAME"<<endl;
	}
	
	}else if(c==2){
			system("cls");
			do{
			cout<<"~~~~~~~~~~SIGN UP~~~~~~~~~~"<<endl;
				if(student[quantity].Password2!=student[quantity].Password)
				cout<<"Please Make sure your password is retyped correcly\n";
			cout<<"New student's Username: ";
			cin>>student[quantity].Username;
			cout<<"New student's Last Name: ";
			cin>>student[quantity].Lastname;
			cout<<"New student's First Name: ";
			cin>>student[quantity].Firstname;
			cout<<"New student's ID number: ";
			cin>>student[quantity].Idno;
			cout<<"New student's Password: ";
			cin>>student[quantity].Password;
			cout<<"Retype New student's Password: ";
			cin>>student[quantity].Password2;
		}while(student[quantity].Password2!=student[quantity].Password);
			i=quantity;
			quantity++;
			loggedin++;
	}
	
	if(loggedin>0){
		do{
	system("cls");
	cout<<"~~~~~~~~~~ANIMOO SIS~~~~~~~~~~"<<endl;
	cout<<"\n\n";
	
	cout<<"1. Enrol in a class\n";
	cout<<"2. Drop a Class\n";
	cout<<"3. View class\es\n";
	cout<<"4. Drop out of school\n";
	cout<<"5. Log out\n";
	cin>>a;
		if(a==1){
			system("cls");
			cout<<"~~~~~~~~~~Enrol in a class~~~~~~~~~~"<<endl<<endl;
			cin>>c;
			
		}else if(a==2){
			system("cls");
			cout<<"~~~~~~~~~~Drop a Class~~~~~~~~~~"<<endl<<endl;
			cin>>c;
			
		}else if(a==3){
			system("cls");
			cout<<"~~~~~~~~~~View class/es~~~~~~~~~~"<<endl<<endl;
			cin>>c;
			
		}else if(a==4){
			system("cls");
			cout<<"~~~~~~~~~~Dropping out of school~~~~~~~~~~"<<endl<<endl;
			cout<<"Would you, "<<student[i].Firstname<<" "<<student[i].Lastname<<" would like to drop out of school?"<<endl;
			cout<<"	1. YES"<<endl;
			cin>>c;
			if(c==1){
				for(; i<=quantity; i++){
				student[i].Username=student[i+1].Username;
				student[i].Lastname=student[i+1].Lastname;
				student[i].Firstname=student[i+1].Firstname;
				student[i].Password=student[i+1].Password;
				student[i].Password2=student[i+1].Password2;
				student[i].Idno=student[i+1].Idno;
			}quantity--;
			a=5;
			}
		}else if(a==5){
			loggedin--;
		}
	}while(a!=5);}
	cout<<endl<<"RETURN TO LOG IN(1 for yes)"<<endl;
	cin>>r;
	}while(r==1);}	
