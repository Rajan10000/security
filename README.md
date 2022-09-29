#include<iostream>
using namespace std;
class security
{
    int password;
    //user_id;


public:
    int user_id;
    void get_input();
    void display();
    void password1();
    void user_id1();


};
void security::get_input()
{
    cout<<"Enter your password: ";
    cin>>password;
    cout<<"Enter your user_id: ";
    cin>>user_id;

}
void security::display()
{
    cout<<"your Entered password: "<<password<<endl;

    cout<<"your Entered user_id: "<<user_id<<endl;
}
void security::password1()

{
    if(password==123456||password==6112001)


    {
        cout<<"__________________________"<<endl;
        cout<<"hello sir "<<endl;
        cout<<"__________________________"<<endl;
    }
    else
    { cout<<"**********************"<<endl;
        cout<<"pRE HO ";
        cout<<"**************************"<<endl;
    }
}
void security::user_id1()

{
    if(user_id==123456)
    { cout<<"___________________________"<<endl;
        cout<<"how are you"<<endl;
        cout<<"______________________________"<<endl;
    }
    else
    { cout<<"*****************************"<<endl;
        cout<<"tu"<<endl;
        cout<<"*****************************"<<endl;
    }
}
int main()
{

    security s[20];


    for(int i=0; i<20; i++)
    {
        s[i].get_input();
        s[i].display();
        s[i].password1();
        s[i].user_id1();

    }
    return 0;

}

