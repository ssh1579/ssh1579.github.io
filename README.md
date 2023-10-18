# ssh1579.github.io
ssh1579.me

```cpp
#include <bits/stdc++.h>
using namespace std;
long long n, k, d1, d2, ans, newmoo, extmoo;
int main() {
    ios::sync_with_stdio(false);
    cin.tie(nullptr);
    cin >> n >> k;
    ans = k + 1;
    cin >> d1;
    for(int i = 2; i <= n; i++) {
        cin >> d2;
        if(d2 - d1 >= k + 1) ans += k + 1;
            else ans += d2 - d1;
        d1 = d2;
    }
    cout << ans;
    return 0;
}
```
