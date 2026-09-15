What is the largest prime factor of the number 600851475143?

First i initialized n=600851475143 and largest=0 then i used a for loop to check the factors of n if n is divisible by i stored i in largest and divided n by i repeated this until all the factors were removed finally I printed largest which is 6857

```cpp
#include <iostream>
using namespace std;
int main(){
    long long n=600851475143;
    long long largest=0;
    for(long long i=2;i<=n;i++){
        while(n%i==0){
            largest=i;
            n=n/i;
        }
    }
    cout << largest;
    return 0;
}
```