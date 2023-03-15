#include<iostream>    
using namespace std;    
     
int main(){    
    int n=0; //聲明一個名為n的變量，並將其初始值設為0   
    int bin[8]; //聲明一個名為bin的數組，並指定其大小為8   
    cin>>n; //讀取輸入值儲存到n   
    if (n<0)    
    {    
        n+=256; //n小於0就將上256   
    }    
    for (int i = 7; i >= 0; i--) //i的初始值為7，如果i>=0，就繼續執行循環，每次-1   
    {    
        bin[i]=n%2;    
        n/=2; //將n除2取餘數儲存在i    
    }    
    for (int i = 0; i < 8; i++)    
    {    
        cout<<bin[i]; //將轉換好的二進制數i輸出到電腦上   
    }    
    cout<<"\n"; //換行    
         
     
         
     
}  
