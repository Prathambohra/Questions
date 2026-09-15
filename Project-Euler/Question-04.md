Find the largest palindrome made from the product of two 3-digit numbers.

First i initialized res=0 to store the largest palindrome then i used two for loops to check all the products of two 3 digit numbers from 100 to 999 for each pair i multiplied them and stored the result in n then i reversed the number using a while loop and stored the reversed number in rev if n and rev are equal then it is a palindrome so i checked if it is greater than res and stored it in res finally i printed res which is 906609

```cpp
#include <iostream>
using namespace std;
int main(){
    long long res=0;
    long long rev,temp,n;
    for(long long i=100;i<=999;i++){
        for(long long j=100;j<=999;j++){
            n=i*j;
            temp=n;
            rev=0;
            while(temp!=0){
                rev=rev*10+temp%10;
                temp/=10;
            }
            if(n == rev && n > res) {
                res = n;
            }
        }
    }
    cout << res;
    return 0;
}
```