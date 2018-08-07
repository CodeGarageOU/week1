## Solution 1

#### Code

```
#include<iostream>
using namespacestd;

int main() {

 int t;
 cin>>t;

  while(t--){
   
   int n;

   cin>>n;   

   int a[n]; 
    
   for(int i =0;i<n;i++)
      cin>>a[i];

  cout<<(n*(n-1))/2<<endl;  

  }

}
```

## Solution 2 

#### Code

```
#include<iostream> 
using namespace std;
 
int main()
{
	int t;
	int ar[11];
	cin>>t;
	
	while(t--)
	{
	    int a,b,i=0,k=0;
		
		cin>>a>>b;
		
		while(a || b)
		{
			int k=0;
			
			k=a%10+ b%10;
			
			ar[i++]=k%10;
			
			a/=10;
			b/=10;		
		}
		
		for(int j=i-1;j>=0;j--) 
		{
			if(ar[j]==0 && k==0 && j!= 0) continue;
			else
			{
				k=1;
				cout<<ar[j];
			} 
		}
		cout<<endl;
	}
}
```

## Solution 3

#### Code

```
#include<iostream>
#define ll long long
 
using namespace std;

int main() {
 
  ll a,k,n;
  cin >>a>>n>>k;
  
  ll ans[k];
  ll temp=a;
  
  for(int i=0;i<k;i++) {
    ans[i]= temp%(n+1);
    temp =temp/(n+1);
  }
  cout<<endl;
  for(int i=0;i<k;i++){ 
    cout<<ans[i]<<" ";     
  }
  return 0;
} 
```

## Solution 4

#### Code

```
#include<iostream>
#include<string>
using namespace std;
 
int main()
{
    int t;
    cin>>t;
    
    string s;
    int flag=0,a=0,d=0,b=0;
    
    for(int i=0;i<t;i++)
    {
        cin>>s;
        a=0;
        b=0;
        d=0;
        flag=0;
        
        for(int j=0;j<s.length();j++)
        {
            if(s[j]=='A')
            {
                if(flag==1)
                    a+=d;
                d=0;
                a++;
                flag=1;
            }
            else if(s[j]=='B')
            {
                if(flag==2)
                    b+=d;
                d=0;
                b++;
                flag=2;
            }
            else
            d++;
        }
        
        cout<<a<<" "<<b<<endl;
    }
}  
```

## Solution 5

#### Code

```
#include <bits/stdc++.h>
using namespace std;
 
int countNegative(int M[][4], int n, int m)
{ 
    // initialize result
    int count = 0; 
 
    // Start with top right corner
    int i = 0;
    int j = m - 1; 
 
    // Follow the path shown using
    // arrows above
    while( j >= 0 && i < n )
    {
        if( M[i][j] < 0 )
        {
            // j is the index of the
            // last negative number
            // in this row. So there
            // must be ( j+1 )
            count += j + 1;
 
            // negative numbers in 
            // this row.
            i += 1;
        }
             
        // move to the left and see 
        // if we can find a negative
        // number there
        else
        j -= 1;
    }
 
    return count;
}
 
int main () 
{
    int M[3][4] = { {-3, -2, -1, 1},
                    {-2, 2, 3, 4},
                    {4, 5, 7, 8} };
     
    cout << countNegative(M, 3, 4);
     
    return 0;    
}
```

## Solution 6

#### Code

```
#include<bits/stdc++.h>
using namespace std;

typedef long long ll;

int main()
{
    
    ll t;
	cin>>t;
	
	ll n;
	for(ll i=0;i<t;i++)
	{
        cin>>n;
        
        if(n%2==0)
        {
            n=n-2;
            n/=2;
        }
        else
        {
            n=n-3;
            n/=2;
        }
        cout<<(n*(n+1))/2<<endl;
     }
}
```
