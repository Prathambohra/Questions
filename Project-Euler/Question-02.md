Questions is about finding the sum of all the even-valued terms in the fibonacci sequence whose values do not exceed 4000000

First i initialized a=1 b=2 and sum=0 then i used a while loop to generate Fibonacci numbers up to 4000000 for every number i checked if it is divisible by 2 using % if the remainder is 0 i added that number to sum then i generated the next fibonacci number by adding a and b finally i printed the sum which is 4613732

```cpp
#include <iostream>
using namespace std;
int main(){
    int a=1,b=2;
    int sum=0;
    while(b<=4000000){
        if(b%2==0){
            sum+=b;
        }
        int c=a+b;
        a=b;
        b=c;
    }
    cout << sum;
    return 0;
}
```