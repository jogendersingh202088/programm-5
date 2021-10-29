# programm-5
#include<iostream>
using namespace std;
int length(string s1)
{

	int i=0;
while(s1[i]!='\0')
{i++;
}
cout<<"length of the string is "<<i<<"\n";	
return i;	
}
void con(string s1)
{string s2;
cout<< "enter the second to concat  ";
cin>>s2;
s2=s1+s2;
cout<<s2<<"\n";
}
void copy(string s1)
{ string s2;
s2=s1;
cout<<"s1 is copied to s2 \n"<<s2<<"\n";

}
void string_reverse(string s1,int len)
{ int i;
	for(i=len-1;i>=0;i--)
	cout<<s1[i];
}
int main()
{ int len;
	string s1;
	cout<<"enter the string ";
	cin>>s1;
	// length of string
	len=length(s1);
	//cancatnation
	con(s1);
	//string copy
	copy(s1);
	//reversing
	string_reverse(s1,len);
	return 0;	
	
}
