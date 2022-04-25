# reverse-of-words-in-a-string-in-c++


#include<bits/stdc++.h>
using namespace std;


int main()
{
    int i=0,j,n;
    
    string s, s1;

    getline(cin,s);
    n=s.size();

    while (i<n)
    {

    while(i<n&&s[i]==' ')
        i++;
    if(i>=n) break;
        j=i+1;
    while(j<n&&s[j]!=' ')
        j++;
    string s3=s.substr(i,j-i);

    if (s1.size()==0)
    {
        s1=s3;
    }
    else
        
    {       s1=s3+" "+s1;
                
    }
    i=j+1;

    }

    cout <<s1 << endl; 

}
