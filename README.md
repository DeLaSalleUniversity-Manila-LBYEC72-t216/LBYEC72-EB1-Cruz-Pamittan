# LBYEC72-EB1-Cruz-Pamittan

LBYEC72 EB1
Members:
Danielle Cruz
Bea Pamittan

Brief description of the project:
#include<iostream>
#include<string>
#include<cstdlib>
#include<string.h>
using namespace std;


typedef struct{
    char name[17];
    int id;
    int ep;
    char bc[6][30];
    int num;
}m;

int main(){
    m data[40];
    char r[8]="HI";
    int pop=5, c, f=0, til, k, temp, pay, days;
    //char c[10];
    char *end;
    char *p;
    char *y[30];
    char *x[3];
    char s[17];
    char v[7];
    
    strcpy(data[0].name, "Bea Pamittan");
    data[0].id=11515473;
    data[0].ep=25000;
    data[0].num=0;
    
    strcpy(data[1].name, "Danielle Cruz");
    data[1].id=11513225;
    data[1].ep=25000;
    data[1].num=0;
    
    strcpy(data[2].name, "Mark Llido");
    data[2].id=11515260;
    data[2].ep=25000;
    data[2].num=0;
    
    strcpy(data[3].name, "Marton Viva");
    data[3].id=11538597;
    data[3].ep=25000;
    data[3].num=0;
    
    strcpy(data[4].name, "Kendrick Lin");
    data[4].id=11535229;
    data[4].ep=25000;
    data[4].num=0;
    
    
    do{
        cout << "~~~~~~~~~~Library~~~~~~~~~~\n" << endl;
        cout << "	1. Create Student Profile\n" << endl;
        cout << "	2. Borrow Books\n" << endl;
        cout << "	3. Check Overdue Books\n" << endl;
        cout << "	4. Search Student Profile\n" << endl;
        cout << "	5. Exit\n" << endl;
        
        cin >> c;
        if (c==1){
            cout << "~~~~~~~~~~Creation Of Profile~~~~~~~~~~\n" << endl;
            cout << "New Student's Nickname: \n" << endl;
            cin >> data[pop].name;
            cout << "New Student's Card Number: \n" << endl;
            cin >> data[pop].id;
            cout << "New Student's E-Purse Balance: \n" << endl;
            cin >> data[pop].ep;
            data[pop].num=0;
            
            do{
                cout << "\nLoaned books: \n" << endl;
                cout << "	1. Add\n" << endl;
                cout << "	2. Any key to stop adding\n" << endl;
                cin >> c;
                
                if (c==1){
                    
                    cout << "\n\n	*Book Titles*\n\n" << endl;
                    cout << "\n\nAA111	AA222	AA333	AA444	AA555	AA666\n" << endl;
                    cout << "BB111	BB222	BB333	BB444	BB555	BB666\n" << endl;
                    cout << "CC111	CC222	CC333	CC444	CC555	CC666\n" << endl;
                    cout << "DD111	DD222	DD333	DD444	DD555	DD666\n" << endl;
                    cout << "EE111	EE222	EE333	EE444	EE555	EE666\n" << endl;
                    cout << "\nLoaned Book: \n" << endl;
                    cin >> data[pop].bc[data[pop].num] ;
                    
                    y[0] = strstr(data[pop].bc[data[pop].num], "AA111");
                    y[1] = strstr(data[pop].bc[data[pop].num], "AA222");
                    y[2] = strstr(data[pop].bc[data[pop].num], "AA333");
                    y[3] = strstr(data[pop].bc[data[pop].num], "AA444");
                    y[4] = strstr(data[pop].bc[data[pop].num], "AA555");
                    y[5] = strstr(data[pop].bc[data[pop].num], "AA666");
                    
                    y[6] = strstr(data[pop].bc[data[pop].num], "BB111");
                    y[7] = strstr(data[pop].bc[data[pop].num], "BB222");
                    y[8] = strstr(data[pop].bc[data[pop].num], "BB333");
                    y[9] = strstr(data[pop].bc[data[pop].num], "BB444");
                    y[10] = strstr(data[pop].bc[data[pop].num], "BB555");
                    y[11] = strstr(data[pop].bc[data[pop].num], "BB666");
                    
                    y[12] = strstr(data[pop].bc[data[pop].num], "CC111");
                    y[13] = strstr(data[pop].bc[data[pop].num], "CC222");
                    y[14] = strstr(data[pop].bc[data[pop].num], "CC333");
                    y[15] = strstr(data[pop].bc[data[pop].num], "CC444");
                    y[16] = strstr(data[pop].bc[data[pop].num], "CC555");
                    y[17] = strstr(data[pop].bc[data[pop].num], "CC666");
                    
                    y[18] = strstr(data[pop].bc[data[pop].num], "DD111");
                    y[19] = strstr(data[pop].bc[data[pop].num], "DD222");
                    y[20] = strstr(data[pop].bc[data[pop].num], "DD333");
                    y[21] = strstr(data[pop].bc[data[pop].num], "DD444");
                    y[22] = strstr(data[pop].bc[data[pop].num], "DD555");
                    y[23] = strstr(data[pop].bc[data[pop].num], "DD666");
                    
                    y[24] = strstr(data[pop].bc[data[pop].num], "EE111");
                    y[25] = strstr(data[pop].bc[data[pop].num], "EE222");
                    y[26] = strstr(data[pop].bc[data[pop].num], "EE333");
                    y[27] = strstr(data[pop].bc[data[pop].num], "EE444");
                    y[28] = strstr(data[pop].bc[data[pop].num], "EE555");
                    y[29] = strstr(data[pop].bc[data[pop].num], "EE666");
                    
                    if ((y[0] != NULL)||(y[1] != NULL)||(y[2] != NULL)||(y[3] != NULL)||(y[4] != NULL)||(y[5] != NULL)||(y[6] != NULL)||(y[7] != NULL)||(y[8] != NULL)||(y[9] != NULL)||(y[10] != NULL)||(y[11] != NULL)||(y[12] != NULL)||(y[13] != NULL)||(y[14] != NULL)||(y[15] != NULL)||(y[16] != NULL)||(y[17] != NULL)||(y[18] != NULL)||(y[19] != NULL)||(y[20] != NULL)||(y[21] != NULL)||(y[22] != NULL)||(y[23] != NULL)||(y[24] != NULL)||(y[25] != NULL)||(y[26] != NULL)||(y[27] != NULL)||(y[28] != NULL)||(y[29] != NULL)) {
                        cout << "\nSuccessful Transaction\n" << endl;
                        data[pop].num++;
                    }else if ((y[6] != NULL)||(y[7] != NULL)||(y[8] != NULL)||(y[9] != NULL)||(y[10] != NULL)||(y[11] != NULL)) {
                        cout << "\nSuccessful Transaction\n" << endl;
                        data[pop].num++;
                    }else if ((y[12] != NULL)||(y[13] != NULL)||(y[14] != NULL)||(y[15] != NULL)||(y[16] != NULL)||(y[17] != NULL)) {
                        cout << "\nSuccessful Transaction\n" << endl;
                        data[pop].num++;
                    }else if ((y[18] != NULL)||(y[19] != NULL)||(y[20] != NULL)||(y[21] != NULL)||(y[22] != NULL)||(y[23] != NULL)) {
                        cout << "\nSuccessful Transaction\n" << endl;
                        data[pop].num++;
                    }else if ((y[24] != NULL)||(y[25] != NULL)||(y[26] != NULL)||(y[27] != NULL)||(y[28] != NULL)||(y[29] != NULL)) {
                        cout << "\nSuccessful Transaction\n" << endl;
                        data[pop].num++;
                    }else{
                        cout << "\nInvalid Book Title\n" << endl;
                    }
                }
            }while(c==1);
            cout << "\nProfile created successfully\n" << endl;
            cout << "Amount to pay: \n" << endl;
            cout << "Creation fee (1500) + " << data[pop].ep << " = " << (data[pop].ep+1500) << endl;
            
            pop++;
            
        }else if (c==2){
            cout << "~~~~~~~~~~Borrow Books~~~~~~~~~~\n" << endl;
            cout << "Student's Card Number: \n" << endl;
            cin >> temp;
            for(int i=0; i<pop; i++){
                if(temp==data[i].id){
                    til=i;
                }
            }
            
            cout << "Student Name: " << data[til].name << endl;
            do{
                cout << "\nLoan books: \n" << endl;
                cout << "	1. Add\n" << endl;
                cout << "	2. Any key to stop adding\n" << endl;
                cin >> c ;
                
                if (c==1){
                    
                    cout << "\n\n	*Book Titles*\n\n" << endl;
                    cout << "\n\nAA111	AA222	AA333	AA444	AA555	AA666\n" << endl;
                    cout << "BB111	BB222	BB333	BB444	BB555	BB666\n" << endl;
                    cout << "CC111	CC222	CC333	CC444	CC555	CC666\n" << endl;
                    cout << "DD111	DD222	DD333	DD444	DD555	DD666\n" << endl;
                    cout << "EE111	EE222	EE333	EE444	EE555	EE666\n" << endl;
                    cout << "\nLoaned Book: \n" << endl;
                    cin >> data[til].bc[data[til].num] ;
                    
                    y[0] = strstr(data[til].bc[data[til].num], "AA111");
                    y[1] = strstr(data[til].bc[data[til].num], "AA222");
                    y[2] = strstr(data[til].bc[data[til].num], "AA333");
                    y[3] = strstr(data[til].bc[data[til].num], "AA444");
                    y[4] = strstr(data[til].bc[data[til].num], "AA555");
                    y[5] = strstr(data[til].bc[data[til].num], "AA666");
                    
                    y[6] = strstr(data[til].bc[data[til].num], "BB111");
                    y[7] = strstr(data[til].bc[data[til].num], "BB222");
                    y[8] = strstr(data[til].bc[data[til].num], "BB333");
                    y[9] = strstr(data[til].bc[data[til].num], "BB444");
                    y[10] = strstr(data[til].bc[data[til].num], "BB555");
                    y[11] = strstr(data[til].bc[data[til].num], "BB666");
                    
                    y[12] = strstr(data[til].bc[data[til].num], "CC111");
                    y[13] = strstr(data[til].bc[data[til].num], "CC222");
                    y[14] = strstr(data[til].bc[data[til].num], "CC333");
                    y[15] = strstr(data[til].bc[data[til].num], "CC444");
                    y[16] = strstr(data[til].bc[data[til].num], "CC555");
                    y[17] = strstr(data[til].bc[data[til].num], "CC666");
                    
                    y[18] = strstr(data[til].bc[data[til].num], "DD111");
                    y[19] = strstr(data[til].bc[data[til].num], "DD222");
                    y[20] = strstr(data[til].bc[data[til].num], "DD333");
                    y[21] = strstr(data[til].bc[data[til].num], "DD444");
                    y[22] = strstr(data[til].bc[data[til].num], "DD555");
                    y[23] = strstr(data[til].bc[data[til].num], "DD666");
                    
                    y[24] = strstr(data[til].bc[data[til].num], "EE111");
                    y[25] = strstr(data[til].bc[data[til].num], "EE222");
                    y[26] = strstr(data[til].bc[data[til].num], "EE333");
                    y[27] = strstr(data[til].bc[data[til].num], "EE444");
                    y[28] = strstr(data[til].bc[data[til].num], "EE555");
                    y[29] = strstr(data[til].bc[data[til].num], "EE666");
                    
                    if ((y[0] != NULL)||(y[1] != NULL)||(y[2] != NULL)||(y[3] != NULL)||(y[4] != NULL)||(y[5] != NULL)) {
                        cout << "\nSuccessful Transaction\n" << endl;
                        data[til].num++;
                    }else if ((y[6] != NULL)||(y[7] != NULL)||(y[8] != NULL)||(y[9] != NULL)||(y[10] != NULL)||(y[11] != NULL)) {
                        cout << "\nSuccessful Transaction\n" << endl;
                        data[til].num++;
                    }else if ((y[12] != NULL)||(y[13] != NULL)||(y[14] != NULL)||(y[15] != NULL)||(y[16] != NULL)||(y[17] != NULL)) {
                        cout << "\nSuccessful Transaction\n" << endl;
                        data[til].num++;
                    }else if ((y[18] != NULL)||(y[19] != NULL)||(y[20] != NULL)||(y[21] != NULL)||(y[22] != NULL)||(y[23] != NULL)) {
                        cout << "\nSuccessful Transaction\n" << endl;
                        data[til].num++;
                    }else if ((y[24] != NULL)||(y[25] != NULL)||(y[26] != NULL)||(y[27] != NULL)||(y[28] != NULL)||(y[29] != NULL)) {
                        cout << "\nSuccessful Transaction\n" << endl;
                        data[til].num++;
                    }else{
                        
                        cout << "\nInvalid Book Title\n" << endl;
                    }
                }
            }while(c==1);
            
}else if (c==3){
            cout << "~~~~~~~~~~Computing Overdue FEE~~~~~~~~~~\n" << endl;
            cout << "~~~~~~~~~~Returning Books~~~~~~~~~~\n" << endl;
            cout << "Student's Card Number: \n" << endl;
            cin >> temp ;
            for(int i=0; i<pop; i++){
                if(temp==data[i].id){
                    til=i;
                }
            }
            cout << "Student Name: " << data[til].name << endl;
            cout << "~~~~~~~~~~Book Code Return~~~~~~~~~~\n" << endl;
            cin >> s;
            for(int i=0; i<pop; i++){
                p = strstr(data[til].bc[i], s);
                if (p != NULL){
                    cout << "Book Found: " << data[til].bc[i] << endl;
                    
                    cout << "Input days borrowed\n" << endl;
                    cin >> days ;
                    
                    y[0] = strstr(data[til].bc[data[i].num], "AA111");
                    y[1] = strstr(data[til].bc[data[i].num], "AA222");
                    y[2] = strstr(data[til].bc[data[i].num], "AA333");
                    y[3] = strstr(data[til].bc[data[i].num], "AA444");
                    y[4] = strstr(data[til].bc[data[i].num], "AA555");
                    y[5] = strstr(data[til].bc[data[i].num], "AA666");
                    
                    y[6] = strstr(data[til].bc[data[i].num], "BB111");
                    y[7] = strstr(data[til].bc[data[i].num], "BB222");
                    y[8] = strstr(data[til].bc[data[i].num], "BB333");
                    y[9] = strstr(data[til].bc[data[i].num], "BB444");
                    y[10] = strstr(data[til].bc[data[i].num], "BB555");
                    y[11] = strstr(data[til].bc[data[i].num], "BB666");
                    
                    y[12] = strstr(data[til].bc[data[i].num], "CC111");
                    y[13] = strstr(data[til].bc[data[i].num], "CC222");
                    y[14] = strstr(data[til].bc[data[i].num], "CC333");
                    y[15] = strstr(data[til].bc[data[i].num], "CC444");
                    y[16] = strstr(data[til].bc[data[i].num], "CC555");
                    y[17] = strstr(data[til].bc[data[i].num], "CC666");
                    
                    y[18] = strstr(data[til].bc[data[i].num], "DD111");
                    y[19] = strstr(data[til].bc[data[i].num], "DD222");
                    y[20] = strstr(data[til].bc[data[i].num], "DD333");
                    y[21] = strstr(data[til].bc[data[i].num], "DD444");
                    y[22] = strstr(data[til].bc[data[i].num], "DD555");
                    y[23] = strstr(data[til].bc[data[i].num], "DD666");
                    
                    y[24] = strstr(data[til].bc[data[i].num], "EE111");
                    y[25] = strstr(data[til].bc[data[i].num], "EE222");
                    y[26] = strstr(data[til].bc[data[i].num], "EE333");
                    y[27] = strstr(data[til].bc[data[i].num], "EE444");
                    y[28] = strstr(data[til].bc[data[i].num], "EE555");
                    y[29] = strstr(data[til].bc[data[i].num], "EE666");
                    
                    if ((y[0] != NULL)||(y[1] != NULL)||(y[2] != NULL)||(y[3] != NULL)||(y[4] != NULL)||(y[5] != NULL)) {
                        if(days>10){
                            pay=(days-10)*20;
                            cout << "\nYou have exceded the allowed number of borrow days\n" << endl;
                            cout << "\nYou have a overdue fee of " << pay << endl;
                            cout << "\nYour E-Purse Balance " << data[til].ep << endl;
                            if((data[til].ep)<pay){
                                do{
                                    cout << "\nYour E-Purse balance is not enough to cover your fee\n" << endl;
                                    cout << "Please Avail of our Voucher Codes to continue\n" << endl;
                                    cout << "\nEP100	EP500	EP1000\n" << endl;
                                    cin >> v;
                                    
                                    x[0] = strstr(v, "EP100");
                                    x[1] = strstr(v, "EP500");
                                    x[2] = strstr(v, "EP100");
                                    if (x[0] != NULL){
                                        data[til].ep=data[til].ep+100;
                                        cout << "Thankyou for availing EP100\n" << endl;
                                    }if (x[1] != NULL){
                                        data[til].ep=data[til].ep+500;
                                        cout << "Thankyou for availing EP500\n" << endl;
                                    }if (x[3] != NULL){
                                        data[til].ep=data[til].ep+1000;
                                        cout << "Thankyou for availing EP1000\n" << endl;
                                    }
                                }while((data[til].ep)<pay);
                            }else{
                                cout << "\nYour fee has been charged to your E-Purse\n" << endl;
                            }
                            data[til].ep=data[til].ep-pay;
                            cout << "\nRemaining E-Purse Value: " << data[til].ep << endl;
                        }else{
                            cout << "\nYou have returned the book within the allowed borrow days\nThankyou\n" << endl;
                        }
                    }else if ((y[6] != NULL)||(y[7] != NULL)||(y[8] != NULL)||(y[9] != NULL)||(y[10] != NULL)||(y[11] != NULL)) {
                        if(days>8){
                            pay=(days-8)*35;
                            cout << "\nYou have exceded the allowed number of borrow days\n" << endl;
                            cout << "\nYou have a overdue fee of " << pay << endl;
                            cout << "\nYour E-Purse Balance " << data[til].ep << endl;
                            if((data[til].ep)<pay){
                                do{
                                    cout << "\nYour E-Purse balance is not enough to cover your fee\n" << endl;
                                    cout << "Please Avail of our Voucher Codes to continue\n" << endl;
                                    cout << "\nEP100	EP500	EP1000\n" << endl;
                                    cin >> v;
                                    
                                    x[0] = strstr(v, "EP100");
                                    x[1] = strstr(v, "EP500");
                                    x[2] = strstr(v, "EP100");
                                    if (x[0] != NULL){
                                        data[til].ep=data[til].ep+100;
                                        cout << "Thankyou for availing EP100\n" << endl;
                                    }if (x[1] != NULL){
                                        data[til].ep=data[til].ep+500;
                                        cout << "Thankyou for availing EP500\n" << endl;
                                    }if (x[3] != NULL){
                                        data[til].ep=data[til].ep+1000;
                                        cout << "Thankyou for availing EP1000\n" << endl;
                                    }
                                }while((data[til].ep)<pay);
                            }else{
                                cout << "\nYour fee has been charged to your E-Purse\n" << endl;
                            }
                            data[til].ep=data[til].ep-pay;
                            cout << "\nRemaining E-Purse Value: " << data[til].ep << endl;
                        }else{
                            cout << "\nYou have returned the book within the allowed borrow days\nThankyou\n" << endl;
                        }
                    }else if ((y[12] != NULL)||(y[13] != NULL)||(y[14] != NULL)||(y[15] != NULL)||(y[16] != NULL)||(y[17] != NULL)) {
                        if(days>5){
                            pay=(days-5)*50;
                            cout << "\nYou have exceeded the allowed number of borrow days\n" << endl;
                            cout << "\nYou have a overdue fee of " << pay << endl;
                            cout << "\nYour E-Purse Balance " << data[til].ep << endl;
                            if((data[til].ep)<pay){
                                do{
                                    cout << "\nYour E-Purse balance is not enough to cover your fee\n" << endl;
                                    cout << "Please Avail of our Voucher Codes to continue\n" << endl;
                                    cout << "\nEP100	EP500	EP1000\n" << endl;
                                    cin >> v ;
                                    
                                    x[0] = strstr(v, "EP100");
                                    x[1] = strstr(v, "EP500");
                                    x[2] = strstr(v, "EP100");
                                    if (x[0] != NULL){
                                        data[til].ep=data[til].ep+100;
                                        cout << "Thankyou for availing EP100\n" << endl;
                                    }if (x[1] != NULL){
                                        data[til].ep=data[til].ep+500;
                                        cout << "Thankyou for availing EP500\n" << endl;
                                    }if (x[3] != NULL){
                                        data[til].ep=data[til].ep+1000;
                                        cout << "Thankyou for availing EP1000\n" << endl;
                                    }
                                }while((data[til].ep)<pay);
                            }else{
                                cout << "\nYour fee has been charged to your E-Purse\n" << endl;
                            }
                            data[til].ep=data[til].ep-pay;
                            cout << "\nRemaining E-Purse Value: " << data[til].ep << endl;
                        }else{
                            cout << "\nYou have returned the book within the allowed borrow days\nThankyou\n" << endl;
                        }
                    }else if ((y[18] != NULL)||(y[19] != NULL)||(y[20] != NULL)||(y[21] != NULL)||(y[22] != NULL)||(y[23] != NULL)) {
                        if(days>3){
                            pay=(days-3)*85;
                            cout << "\nYou have exceded the allowed number of borrow days\n" << endl;
                            cout << "\nYou have a overdue fee of " << pay << endl;
                            cout << "\nYour E-Purse Balance " << data[til].ep << endl;
                            if((data[til].ep)<pay){
                                do{
                                    cout << "\nYour E-Purse balance is not enough to cover your fee\n" << endl;
                                    cout << "Please Avail of our Voucher Codes to continue\n" << endl;
                                    cout << "\nEP100	EP500	EP1000\n" << endl;
                                    cin >> v ;
                                    
                                    x[0] = strstr(v, "EP100");
                                    x[1] = strstr(v, "EP500");
                                    x[2] = strstr(v, "EP100");
                                    if (x[0] != NULL){
                                        data[til].ep=data[til].ep+100;
                                        cout << "Thankyou for availing EP100\n" << endl;
                                    }if (x[1] != NULL){
                                        data[til].ep=data[til].ep+500;
                                        cout << "Thankyou for availing EP500\n" << endl;
                                    }if (x[3] != NULL){
                                        data[til].ep=data[til].ep+1000;
                                        cout << "Thankyou for availing EP1000\n" << endl;
                                    }
                                }while((data[til].ep)<pay);
                            }else{
                                cout << "\nYour fee has been charged to your E-Purse\n" << endl;
                            }
                            data[til].ep=data[til].ep-pay;
                            cout << "\nRemaining E-Purse Value: "<< data[til].ep << endl;
                        }else{
                            cout << "\nYou have returned the book within the allowed borrow days\nThankyou\n" << endl;
                        }
                    }else if ((y[24] != NULL)||(y[25] != NULL)||(y[26] != NULL)||(y[27] != NULL)||(y[28] != NULL)||(y[29] != NULL)) {
                        if(days>2){
                            pay=(days-2)*190;
                            cout << "\nYou have exceded the allowed number of borrow days\n" << endl;
                            cout << "\nYou have a overdue fee of " << pay << endl;
                            cout << "\nYour E-Purse Balance: " <<  data[til].ep << endl;
                            if((data[til].ep)<pay){
                                do{
                                    cout << "\nYour E-Purse balance is not enough to cover your fee\n" << endl;
                                    cout << "Please Avail of our Voucher Codes to continue\n" << endl;
                                    cout << "\nEP100	EP500	EP1000\n" << endl;
                                    cin >> v;
                                    
                                    x[0] = strstr(v, "EP100");
                                    x[1] = strstr(v, "EP500");
                                    x[2] = strstr(v, "EP100");
                                    if (x[0] != NULL){
                                        data[til].ep=data[til].ep+100;
                                        cout << "Thankyou for availing EP100\n" << endl;
                                    }if (x[1] != NULL){
                                        data[til].ep=data[til].ep+500;
                                        cout << "Thankyou for availing EP500\n" << endl;
                                    }if (x[3] != NULL){
                                        data[til].ep=data[til].ep+1000;
                                        cout << "Thankyou for availing EP1000\n" << endl;
                                    }
                                }while((data[til].ep)<pay);
                            }else{
                                cout << "\nYour fee has been charged to your E-Purse\n" << endl;
                            }
                            data[til].ep=data[til].ep-pay;
                            cout << "\nRemaining E-Purse Value: " << data[til].ep << endl;
                        }else{
                            cout << "\nYou have returned the book within the allowed borrow days\nThankyou\n" << endl;
                        }
                    }else{
                        cout << "\nYou have not borrowed this book\n" << endl;
                    }
                    k=i;
                    i=pop;
                }
            }
            for(; k<=data[til].num; k++){
                strcpy(data[til].bc[k], data[til].bc[k+1]);
            }data[til].num--;
        }else if (c==4){
            cout << "~~~~~~~~~~Search Student Profile~~~~~~~~~~\n" << endl;
            cout << "\nSearch Student Name:\n" << endl;
            cin >> s;
            
            for(int i=0; i<pop; i++){
                p = strstr(data[i].name, s);
                if (p != NULL){
                    cout << "\nFOUND\n" << endl;
                    cout << "Student Name: " << data[i].name << endl;
                    cout << "Card Number: " << data[i].id << endl;
                    cout << "E-Purse Balance: " << data[i].ep << endl;
                    cout << "List of Books Currently Loaned: \n" << endl;
                    for(int j=0; j<data[i].num; j++){
                        cout << data[i].bc[j] << endl;
                    }
                    til=i;
                    f++;
                }}
            if(f==0){
                cout << "\nNot Found\n" << endl;
            }
        }else if(c==5){
            strcpy(r, "BOOKWORM");
        }
        if(c!=5){
            cout << "\nCLOSE SYSTEM(BOOKWORM)\n" << endl;
            cin >> r;
        }
        end = strstr(r, "BOOKWORM");
    }while(end==NULL);
    
    return 0;
}



	
