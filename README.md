# Power-Function-Code
This is a beginner level code.
We had done this code in V.S. Code using C++.

#include<iostream>
using namespace std;

class Solution{
    public:
    double mypow(double x, int n){
        if(n==0)return 1.0;
        if(x==0)return 0.0;
        if(x==1)return 1.0;

        if(x==-1){
            if(n%2==0) return 1.0;
            else return -1.0;
        }
        long long binForm=n;
//Using long long for wider range
        if(x==-1){
            if(n%2==0)return 1.0;
            else return -1.0;
        }
        double ans=1.0;
        while (binForm>0){
          if(binForm % 2 == 1){
            ans*=x;
          }
        }
        x*=x;
        binForm/=2;
    }
    returm ans;
};
