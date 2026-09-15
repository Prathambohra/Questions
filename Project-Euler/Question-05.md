What is the smallest positive number that is evenly divisible by all of the numbers from 1 to 20?

First I initialized n=2. Then I used a for loop to check if n is divisible by all the numbers from 1 to 20. If n is not divisible by any number I increased n by 1 and used goto to restart the loop from i=1. If n is divisible by all the numbers from 1 to 20 the loop finishes. Finally I printed n which is 232792560

```cpp
#include <iostream>
using namespace std;
int main(){
    int n=2;
    label:
        for(int i=1;i<=20;i++){
            if(n%i!=0){
                n++;
                goto label;
            }
        }
    cout << n;
    return 0;
}