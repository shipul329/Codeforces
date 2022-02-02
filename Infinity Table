/// Infinity Table ->>
/// In this problem we are going to solve this problem
/// There are some rules.. according to those rules
/// we have to fill a square matrix and after that
/// we have to tell the row and column number of a given number of K
#include<bits/stdc++.h>

using namespace std;

typedef long long ll;

void solve()
{
    ll n;
    cin >> n;

    ll n2=sqrtl(n);

    if(n==1)
    {
        cout << 1 << " " << 1 << '\n';
        return;
    }

    if(n2*n2==n)
        {
            cout << n2 << " " << 1 << '\n';   /// if given number is a perfect square
            return;
        }                                    /// then row = sqrt(n), col = 1
                                            /// ex: n=9, row=3, col=1 

    n2++;   /// find nearest perfect number which is greater

    ll d=n2*n2;
    ll q=n2-1;

    ll rr=d-q; /// right range of particular square nubmer
    ll up=rr-q; /// up range

    ll row=n2;
    ll col=n2;

    if(n>=rr)
    {
        col=d-n+1;  /// number is in right range then row will be same 
    }

    else{
        row=n2-(rr-n);  /// number is in up range then column will be same
    }

    cout << row << " " << col << '\n';
}

int32_t main()
{
    ios_base::sync_with_stdio(0);
    cin.tie(0);
    cout.tie(0);

    int t;
    cin >> t;

    while(t--)
    {
        solve();
    }

    return 0;
}
