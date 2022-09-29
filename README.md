C++ program for bank account more easy way
#include <iostream>
using namespace std;
class bank
{
protected:
    int acc_no;
    char name[100];
    char branch[15];
    char city[15];
    float deposit_amount;
    float withdrawal_amount;
public:
    void get_data();
    void display();
};
void bank::get_data()
    {
        cout<<"Enter acc_no"<<endl;
        cin>>acc_no;
        cout<<"Enter Name"<<endl;
        cin>>name;
       
        cout<<"Enter Branch"<<endl;
        cin>>branch;
        cout<<"Enter City"<<endl;
        cin>>city;
        cout<<"Enter deposit_amount"<<endl;
        cin>>deposit_amount;
        cout<<"Enter withdrawal_amount"<<endl;
        cin>>withdrawal_amount;
        
    }
    void bank::display()
    {
        cout<<"acc_no: "<<acc_no<<endl;
        cout<<" Name: "<<name<<endl;
        
        cout<<"Branch: "<<branch<<endl;
        cout<<"City: "<<city<<endl;
        cout<<"deposit_amount: "<<deposit_amount<<endl;
        cout<<"withdrawal_amount: "<<withdrawal_amount<<endl;
        
    }
int main()
{
    bank p[100];
    {
    int n;
    cout<<"Enter number of person: ";
    cin>>n;
    }
 for(int i=0;i<=100;i++)
{
     p[i].get_data();
     p[i].display();
}
    
    return 0;
}
Output:-

