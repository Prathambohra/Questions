The questions was to find sum of all the multiples of 3 or 5 below 1000

At first i just initalized sum=0 and then i used a for loop to check all the number from 1 to 1000 and divide them by 3 or 5 using or operator and if the reminder is 0 add them to the sum 
finally print the sum 

```cpp
#include<iostream>
using namespace std;
int main(){
    int sum=0;
    for(int i=1;i<=1000;i++){
        if(i%3==0 || i%5==0){
            sum+=i;
        }
    }
    cout << sum;
    return 0;
}
```