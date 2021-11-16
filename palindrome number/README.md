class Solution {
public:
bool isPalindrome(int &num){
long long rev=0;
int digit,a;
a=num;
if(num < 0)
return false;
else if(num < 10)
return true;
else if(num % 10 == 0)
return false;
while(num>0){
digit=num%10;
rev=(rev*10)+digit;
num=num/10;
}
return a==rev;
}
};

