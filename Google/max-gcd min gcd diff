// Problem Statement @: https://leetcode.com/discuss/interview-question/396996/

#include<bits/stdc++.h>
using namespace std;

int main(){
    int n;
    cin>>n;
    if(n==-1)
      cout<<0;
    else{
        int max_GCD= INT_MIN;
        int min_GCD= INT_MAX;
        
    for(int i=0;i<=n;i++){
        if(i==0){
            int temp;
            cin>>temp;
        }
          
        else{
            for(int j=0;j<pow(2,i);j+=2){
                int a,b;
                cin>>a>>b;
                if(a==-1 || b==-1)
                  continue;
                int new_GCD= __gcd(a,b);
                if(new_GCD> max_GCD){
                    max_GCD= new_GCD;
                }
                if(new_GCD< min_GCD){
                    min_GCD= new_GCD;
                }
            }
        }
    }
    cout<<max_GCD- min_GCD;
    }
    
    return 0;
}
