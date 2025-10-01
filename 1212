#include <cstdio>
#define M 1000000007
using ll = long long;
ll p(ll a,ll b){return b?p(a*a%M,b/2)*(b&1?a:1)%M:1;}
int main(){
    int n;
    scanf("%d",&n);
    ll r=0,c=1;
    for(int i=0,x;i<n;i++){
        scanf("%d",&x);
        r=(r + x*c) % M;
        c = i+1<n ? c*(n-1-i)%M * p(i+1, M-2) % M : c;
    }
    printf("%lld", r);
}
