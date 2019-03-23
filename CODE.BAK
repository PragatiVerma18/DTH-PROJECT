#include<ctype.h>
#include<string.h>
#include<conio.h>
#include<stdio.h>
#include<fstream.h>
#include<process.h>
 int g=0;  char w[30];   char z[30];
void entry();
void exit();
void logout()
{                char j;
cout<<"\nDO YOU WISH TO LOGOUT\n enter y for yes\nor press any key to continue";
	  cin>>j;
	  cout<<"\n --*** THANK YOU ***--\n";
 getch();   }

void channelspace()
{     int c;
int chcode;
char chname[30],category[30];
ofstream f1("daily.txt");
ofstream f2("movies.txt");
ofstream f3("sports.txt");
ofstream f4("news.txt");
ofstream f5("music.txt");
ofstream f6("science.txt");
cout<<"enter no of channel to be offered";
cin>>c;
for(int i=0;i<c;i++)
{
cout<<"\n enter chcode,chname and category";
cin>>chcode>>chname>>category;

if(strcmpi(category,"daily")==0)
f1<<chcode<<' '<<chname<<'\n';
else
if(strcmpi(category,"movies")==0)
f2<<chcode<<' '<<chname<<'\n';
else
if(strcmpi(category,"sports")==0)
f3<<chcode<<' '<<chname<<'\n';
else
if(strcmpi(category,"news")==0)
f4<<chcode<<' '<<chname<<'\n';
else
if(strcmpi(category,"music")==0)
f5<<chcode<<' '<<chname<<'\n';
else
if(strcmpi(category,"science")==0)
f6<<chcode<<' '<<chname<<'\n';
}
f1.close();
f2.close();
f3.close();
f4.close();
f5.close();
f6.close();    }

 int chcode;
char chname[30];
void showmusic()
{
 cout<<"\nMUSIC:" <<endl;
ifstream f10("music.txt");
while(1)
{
f10>>chcode>>chname;
if(f10.eof())
break;
cout<<chcode<<' '<<chname<<endl;
}
f10.close();}
void showsports()
{
 cout<<"\nSPORTS :"<<endl;
 ifstream f20("sports.txt");
while(1)
{
f20>>chcode>>chname;
if(f20.eof())
break;
cout<<chcode<<' '<<chname<<endl;}
f20.close();  }
void shownews()
{
cout<< "\nNEWS:"<<endl;
ifstream f30("news.txt");
while(1)
{
f30>>chcode>>chname;
if(f30.eof())
break;
cout<<chcode<<' '<<chname<<endl;}
f30.close();}
void showscience()
{
cout<<"\nSCIENCE:"<<endl;
ifstream f40("science.txt");
while(1)
{
f40>>chcode>>chname;
if(f40.eof())
break;
cout<<chcode<<' '<<chname<<endl;}
f40.close();}
void showmov()
{
cout<<"\nMOVIES:"<<endl;
ifstream f50("movies.txt");
while(1)
{
f50>>chcode>>chname;
if(f50.eof())
break;
cout<<chcode<<' '<<chname<<endl;}
f50.close();}
void showdaily()
{
cout<<"\nDAILY SOAP:"<<endl;
ifstream f60("daily.txt");
while(1)
{
f60>>chcode>>chname;
if(f60.eof())
break;
cout<<chcode<<' '<<chname<<endl;}
f60.close(); }

class package
{
int pckgcode;
char pckgname[30];
int price;
int discount;
int amount;
int noc;
public:
int retpckgn(char a[])
{ return(strcmpi(a,pckgname));
}
int retprice()
{
return price;}
char * retpckgname()
{return pckgname;
}
void pckin()
{         clrscr();
 cout<<"enter package code\t";
cin>>pckgcode;
cout<<"enter package name\t";
gets(pckgname);
cout<<"enter price for the package\t";
cin>>price;
cout<<"\n-------***-------"<<endl;}

void showpack()
{
 cout<<"\n package code--\t";
cout<<pckgcode;
cout<<"\npackage name--\t";
puts(pckgname);
cout<<"price for the package--\t";
cout<<price;
cout<<"\n-------***-------"<<endl;}
};

class user
{
int userid;
char username[40];
char category[20];
char phno[15];
long areacode;
int noc;
char type;
int bal;
package p;
public:
void input()
{ clrscr();
cout<<"\nenter userid(in numbers)\t";
cin>>userid;
cout<<"\nenter username\t";
gets(username);
cout<<"\nenter selected pack\n(daily,music,news,sports,science,movies)\t";
gets(category);
cout<<"\nenter phno(in 10 digits)\t";
cin>>phno;
cout<<"\n enter areacode(in 2 digits)\t";
cin>>areacode;
cout<<"\nenter no ofconnections(in digits)\t";
cin>>noc;
cout<<"\n enter type of connection(H for HD/ N for normal)\t";
cin>>type;
cout<<"\n-------***-------"<<endl;
}
void display()
{ clrscr();
cout<<"\n---*USER DETAILS ARE*---\n"<<endl;
cout<<"\nuserid--\t";
cout<<userid;
cout<<"\nusername--\t";
puts(username);
cout<<"\ncategory--\t";
puts(category);
cout<<"\nphno--\t";
cout<<phno;
cout<<"\nareacode--\t";
cout<<areacode;
cout<<"\nno ofconnections--\t";
cout<<noc;
cout<<"\ntype of connection--\t";
cout<<type;
calcbal();
cout<<"\nbalance--";
cout<<bal;
cout<<"\n-------***-------"<<endl;
}

char* retname()
 { return username;}
 char* retcat()
 { return category;}
 int retid()
 {
 return userid;}
void update1( char a[])
{
strcpy(category,a);}
int update2();
void updaten(char j[])
{
strcpy(username,j);}
void updatephn(char b[15])
{
strcpy(phno,b);}
void updatea(int a)
{
areacode=a;}
void updatenoc(int l)
{  noc=l;}
void updatet(char b)
{
type=b;}
void calcbal()
{
  bal=bal-update2(); }
};

int user::update2()
{
if(noc==1&&(type=='H'||type=='h'))
{return 300; }
else
if(noc>1&&(type=='H'||type=='h'))
{return 250; }
else
if(noc>1&&(type=='N'||type=='n'))
{return 200; }
else
if(noc==1&&(type=='N'||type=='n'))
{return 150;}
else
return 0;
}




 void writepackage()
{
package p;  int t;
ofstream f("package.txt",ios::binary);
cout<<"\n---*ENTER PACKAGE DETAILS*---\n"<<endl;
cout<<"enter no of packages being offered\t";
cin>>t;
for(int i=0;i<t;i++)
{p.pckin();
f.write((char *)&p,sizeof(p));}
f.close();
cout<<"\n-------***-------"<<endl;
}
void writeuser()
{int n;
user u1;
ofstream f1("user.txt",ios::binary);
cout<<"\n---*ENTER USER DETAILS*---\n";
cout<<"\n enter no of users\t";
cin>>n;
for(int i=0;i<n;i++)
{
u1.input();
f1.write((char *)&u1,sizeof(u1));
}
f1.close();
}

void showuser()
{   clrscr();
user u2;
ifstream f2("user.txt",ios::binary);
while(f2.read((char *)&u2,sizeof(u2)))
{
u2.display();}
f2.close();
}

void newuser()
 {user o;    clrscr();
ofstream f1("user.txt",ios::binary|ios::app);
o.input();   strcpy(o.retname(),w);
f1.write((char *)&o,sizeof(o));
f1.close();                         g=1;
cout<<"\nWELCOME TO THE VIDEOCON FAMILY"<<endl;
cout<<"\n-------***-------"<<endl;
}
void  welcome()
{ clrscr();
cout<<"\t------------CONGRAUTLATIONS!!-----------------"<<endl;
cout<<" you now have the world of unlimited fun at your disposal."<<endl;
cout<<"We at VIDEOCON D2H are pleased to see you taking the first step with us"<<endl;
cout<<"GET inside and OPEN up FUN, chose from a wide variety of channels and services"<<endl;
cout<<"\t-----------------------------------------------------------\n"<<endl;     char c,b,j,k,l;
cout<<"do you want to continue\n enter y or Y to explore more\n"<<endl;
cin>>c;
if(c=='y'||c=='Y')
{
clrscr();
entry();
}
}

void run()
  { clrscr();
   char c,m,n,q;
 if(g==1)
 {
 do
 {
cout<<"\n1- Want to explore our services?\n2-manage your account?"<<endl;
cout<<"enter your choice";
cin>>c;
switch(c)
{
case '1':
 char b;                     clrscr();
cout<<"menu is\n1- view all the channels offered\n2-view all the packages\n"<<endl;
cin>>b;
switch(b)
{
case '1':           clrscr();
 showmov();     cout<<endl;
showsports();   cout<<endl;
/*shownews();cout<<endl;
showmusic();
cout<<endl;
showscience();
cout<<endl;
showdaily();
cout<<endl; */
break;

 case '2': clrscr(); package p10;
 ifstream f0("package.txt",ios::binary);
 while(1)
 {
 f0.read((char *)&p10,sizeof(p10));
 if(f0.eof())
 break;
 p10.showpack();   getch();
 }
 f0.close();  break;
 default:cout<<"\nSERVICE UNAVAILABLE\n";
 }
 break;
case '2':  char a; clrscr();
do{
cout<<"menu is\n1-view your account details\n2-view active package details\n3-change your package\n4-delete account\n5-change user details"<<endl;
cin>>a;
switch(a)
{
case '1': clrscr();
user t;
ifstream f2("user.txt",ios::binary);
while(f2.read((char *)&t,sizeof(t)))
{
if(strcmpi(t.retname(),w)==0)

t.display();  }

f2.close();

break;
case '2':  package p;
 user u;
ifstream f22("user.txt",ios::binary);
while(f22.read((char *)&u,sizeof(u)))
{
if(strcmpi(u.retname(),w)==0)
strcpy(z,u.retcat());   }
f22.close();
ifstream f1("package.txt",ios::binary);
while(f1.read((char *)&p,sizeof(p)))
{
if(strcmpi(p.retpckgname(),z)==0)
p.showpack();}
f1.close();
break;
case '3':clrscr();  user u1;    char l[30];
ofstream f23("abc.txt",ios::binary);
ifstream f33("user.txt",ios::binary);
while(f33.read((char *)&u1,sizeof(u1)))
{
if(strcmpi(u1.retname(),w)==0)
{cout<<"\n Enter your desired package name\n";
gets(l);
u1.update1(l);}
f23.write((char *)&u1,sizeof(u1));
  }
f23.close();
f33.close();
remove("user.txt");
rename("abc.txt","user.txt");
break;

case '4':      clrscr();
 user u5;
ofstream f7("rty.txt",ios::binary);
ifstream f8("user.txt",ios::binary);
while(f8.read((char *)&u5,sizeof(u5)))
{
if(strcmpi(u5.retname(),w)!=0)
{cout<<"\nARE YOU SURE TO DELETE THIS ACCOUNT(y/n)"<<endl;
cin>>q;
if(q=='y'||q=='Y')
{
cout<<"\n DELETION SUCCESSFUL\n";
getch();
exit(0);}
f7.write((char *)&u5,sizeof(u5));
 }  }
f7.close();
f8.close();
remove("user.txt");
rename("rty.txt","user.txt");     break;

case '5': clrscr(); user u6; char v,x;    char d[30];   char h[10];int a;

cout<<"\n1-Modify name\n2-modify phno\n3-modify area code\n4-modify type\n5-mofify no of connections"<<endl;
cin>>v;
switch(v)
{
case '1': clrscr();  ofstream f91("asd.txt",ios::binary);
ifstream f01("user.txt",ios::binary);
while(f01.read((char *)&u6,sizeof(u6)))
{
if(strcmpi(u6.retname(),w)==0)
{   cout<<"your old name was="<<w<<endl;
 cout<<"enter the name to be input"<<endl;
gets(d);   strcpy(w,d);
u6.updaten(d); }
f91.write((char *)&u6,sizeof(u6)); }
f91.close();
f01.close();
remove("user.txt");
rename("asd.txt","user.txt");
break;
case '2': clrscr(); ofstream f92("qwer.txt",ios::binary);
ifstream f02("user.txt",ios::binary);
while(f02.read((char *)&u6,sizeof(u6)))
{
if(strcmpi(u6.retname(),w)==0)
{ cout<<"enter your new phno"<<endl;
cin>>h;
u6.updatephn(h); }
f92.write((char *)&u6,sizeof(u6)); }
f92.close();
f02.close();
remove("user.txt");
rename("qwer.txt","user.txt");
break;
case'3': clrscr(); ofstream f93("ewr.txt",ios::binary);
ifstream f03("user.txt",ios::binary);
while(f03.read((char *)&u6,sizeof(u6)))
{
if(strcmpi(u6.retname(),w)==0)
{ cout<<"enter your new area code"<<endl;
cin>>a;
u6.updatea(a); }
f93.write((char *)&u6,sizeof(u6)); }
f93.close();
f03.close();
remove("user.txt");
rename("ewr.txt","user.txt");

break;
case '4':clrscr();  ofstream f94("uio.txt",ios::binary);
ifstream f04("user.txt",ios::binary);
while(f04.read((char *)&u6,sizeof(u6)))
{
if(strcmpi(u6.retname(),w)==0)
{cout<<"enter your new connection type(H/N)"<<endl;
cin>>x;
u6.updatet(x); }
f94.write((char *)&u6,sizeof(u6)); }
f94.close();
f04.close();
remove("user.txt");
rename("uio.txt","user.txt");
break;
case '5': clrscr(); ofstream f95("plo.txt",ios::binary);
ifstream f05("user.txt",ios::binary);
while(f05.read((char *)&u6,sizeof(u6)))
{
if(strcmpi(u6.retname(),w)==0)
{ cout<<"enter new no of connections\n"<<endl;
cin>>a;
u6.updatenoc(a);  }
f95.write((char *)&u6,sizeof(u6)); }
f95.close();
f05.close();
remove("user.txt");
rename("plo.txt","user.txt");
break;
default:cout<<"SORRY WE CANNOT UPDATE YOUR ENTERED INFO"<<endl;
}
 break;
default:cout<<"SORRY REQUEST CANNOT BE FULFILLED\n";}

cout<<"\n Do you want to continue\n";
cin>>m;
}while(m=='y'||m=='Y');
break;

default:cout<<"SORRY YOUR REQUEST CANNOT BE FULFILLED\n";}

cout<<"\n do you want to return to main menu\n";
cin>>n;
}while(n=='y'||n=='Y');
 }


 exit(); }
 void login()
 {  clrscr();
 char a[30],n;
 cout<<"\n enter your name\t";
gets(a);
strcpy(w,a);
user u;
int l=0;
 char p[30];
ifstream f("user.txt",ios::binary);
while(f.read((char *)&u,sizeof(u)))
{
if(strcmpi(u.retname(),a)==0)
{l=1; g=1; clrscr(); }
}

if(l==1)
cout<<"\n--*** LOGIN SUCCESSFUL ***--"<<endl;
else
cout<<"\n data not found"<<endl;
f.close();
clrscr();
 }

  void entry()
{     char b,j,k,l;
cout<<"\nGET STARTED:\n1- login \n2-new user? create account\n3-logout\n4-exit";
cin>>b;
switch(b)
{
case '1':  clrscr();
	   login();

	   run(); break;

case '2': clrscr();
	  newuser();
	   run();  break;
case '3': clrscr();  logout(); exit();
	     break;
case '4': clrscr();
	  exit();

break;
default: cout<<"\nWE ARE SORRY, SERVICE UNAVAILABLE"<<endl;
}

}


  void exit()
  {    char k,l; clrscr();
  cout<<"\nDO YOU WISH TO EXIT\n enter y to exit\n or press any key to continue\n";
cin>>k;
if(k=='y')
{ cout<<"\n--*** THANK YOU ***--\n"; exit(0);}
else
if(k!='y')
{ cout<<"\nDO YOU WISH TO CONTINUE(y/n)\n";
cin>>l;
if(l=='y'||l=='Y')
{  entry();
 run(); }
 else
 run();}
 }




 void main()
{     char c,m,n,q;   clrscr();
cout<<"\n--*** WRITING OF CHANNEL DATA ***--\n"<<endl;
 channelspace();
 clrscr();
cout<<"\n --*** WRITING OF USER DATA ***--\n"<<endl;
 writeuser();
 clrscr();
 cout<<"\n --*** WRITING OF PACKAGE DATA ***-\n"<<endl;
 writepackage();
 clrscr(); 
welcome();
getch();
}
