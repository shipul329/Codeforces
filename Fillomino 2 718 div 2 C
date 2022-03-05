#include<bits/stdc++.h>

using namespace std;

typedef long long ll;

void solve()
{
      ll n;
      cin >> n;
      
      ll a[n][n];
      
      memset(a, false, sizeof(a));
      
      ll x, y, z;
      
      for(ll i=0; i<n; i++)
      {
            cin >> x;
            
            y=i, z=i;
            
            ll ok=x;
            
            while(x--)
            {
                 a[y][z]=ok; ///  stored that value at ith grid
                 
                 if(z!=0 && a[y][z-1]==0)
                 {
                       z--; /// cheacking from ith grid is there any left grid empty or not
                 }
                 
                 else y++; /// otherwise go for next
            }
      }
      
      for(ll i=0; i<n; i++)
      {
            for(ll j=0; j<=i; j++)
            {
                  cout << a[i][j] << " ";  /// print all grids
            }
            
            cout << '\n';
      }
}

int32_t main()
{
      ios_base::sync_with_stdio(0);
      cin.tie(0);
      cout.tie(0);
      
      solve();
      
      return 0;
}
