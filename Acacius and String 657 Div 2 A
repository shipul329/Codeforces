#include<bits/stdc++.h>
using namespace std;
typedef long long LL;

string tar = "abacaba";

bool good(string s) {
    int cnt = 0;
    for (int i=0; i+6<s.size(); i++) {
        string sub = string(s.begin()+i, s.begin()+i+7);
        if (sub == tar) cnt++;
    }
    return cnt == 1;
}

int main() {
    ios::sync_with_stdio(0);
    cin.tie(0);

    int t;
    cin>>t;

    while (t--) {
        int n;
        string t;
        cin>>n>>t;

        bool found = false;
        for (int i=0; i+6<n; i++) {
            string s = t;
            for (int j=0; j<7; j++)
                if (s[i+j] == '?')
                    s[i+j] = tar[j];

            for (int j=0; j<n; j++)
                if (s[j] == '?')
                    s[j] = 'd';

            if (good(s)) {
                found = true;
                cout<<"Yes\n"<<s<<endl;
                break;
            }
        }
        if (!found) cout<<"No"<<endl;
    }
}
