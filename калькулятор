#include <bits/stdc++.h>
typedef long long ll;
using namespace std;

unsigned long long pow2(unsigned long long a, unsigned long long k)
{
unsigned long long n=1;
for(int i=0;i<k;i++) n=n*a;
return n;
}

int main()
{

ll n1,n2;
cin>>n1>>n2;
string s;
cin>>s;
if(s=="0") {cout<<"0"; return 0;}
unsigned long long sum=0;
ll k=0;
for(int i=s.size()-1;i>=0;i--)
{
if(s[i]>='0'&&s[i]<='9') sum=sum+(int(s[i])-'0')*pow2(n1,k);
else if(s[i]>='a'&&s[i]<='z') sum=sum+(int(s[i])-'a'+10)*pow2(n1,k);
k++;
}
string s1="";
while(sum!=0)
{
ll p=sum%n2;
if(p>=0&&p<=9) s1=s1+char(p+'0');
else s1=s1+char(p+'a'-10);
sum/=n2;
}
reverse(s1.begin(),s1.end());
cout<<s1;

}
