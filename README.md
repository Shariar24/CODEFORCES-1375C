///# CODEFORCES-1375C
///HELLO SHARIAR :)
#include<bits/stdc++.h>
#define pb push_back
#define pob pop_back
typedef long l;
typedef long long ll;
typedef unsigned u;
typedef unsigned long ul;
typedef unsigned long long ull;

using namespace std;
int main()
{
    int t;
    cin >> t;
    while(t--)
    {
      ll n,mx,mn,i,j,p,last,actv=1,joma;
    vector <ll> l;
    vector <ll>:: iterator it;
    vector <ll> a;
    cin >> n;
    for(i=0;i<n;i++)
    {
        cin >> p;
        l.pb(p);
        a.pb(p);
    }
    sort(a.begin(),a.end());
  
    if(a[n-1] == l[0] || a[0] == l[n-1])
       {
           cout << "NO" << endl;
           l.clear();
          continue;
       }
    if(a[n-1] == l[n-1])
       {
           cout << "YES" << endl;
           l.clear();
           continue;
       }

   joma = l[n-1];
   
   l.pob();
   
   mx = max_element(l.begin(),l.end())-l.begin();
   
   if(l[0]>=joma) actv = 0;
   
   if(actv == 1)  cout << "YES" << endl;
   
   else cout << "NO" << endl;
   
   l.clear();
   
    }
}
///GOODBYE SHARIAR :(
