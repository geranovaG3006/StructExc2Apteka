# StructExc2Apteka
Да се напише програма, която създава структура Apteka с полета name, mg, number, и price, указващи наименованието, милиграмите, количеството опаковки и цена на лекарствта. Да се въведе цяло число n и след него n на брой данни за лекарствени препарати.В) Да се изведе информацията за лекарствата с основно лекарствено вещество 10 mg.

#include<iostream>
#include<cstring>
#include <iomanip>
using namespace std;
struct Apteka
{
    string name;
    float mg;
    int number;
    double price;
};
int main()
{
    int n;
    cout<<"Number of medicines: ";
    cin>>n;
    Apteka medicine[n];
    for(int i=0;i<n;i++)
    {
        cout<<"*****Medicine*****"<<i+1<<endl;
        cout<<"Name: ";
        cin.get();
        cin>>medicine[i].name;
        cout<<"Mg: ";
        cin.get();
        cin>>medicine[i].mg;
        cout<<"Number: ";
        cin>>medicine[i].number;
        cout<<"Price: ";
        cin>>medicine[i].price;
    }
    cout<<"10: "<<endl;
    for(int i=0;i<n;i++)
    {
            if(medicine[i].mg==10)
            {
                 cout<<"Name: "<<medicine[i].name<<endl;
                 cout<<"Mg: "<<medicine[i].mg<<endl;
                 cout<<"Number : "<<medicine[i].number<<endl;
                 cout<<"Price: "<<medicine[i].price<<endl;
            }
       
    }
    
    
    system("pause");
    return 0;
}

