#include <iostream>
using namespace std;

long long sequence(long long sum){
    int n; cin >> n;
    if(n!=0){
        sum += n;
        return sequence(sum);
    }
    return sum;
}

int main(){
    cout << sequence(0);
}
