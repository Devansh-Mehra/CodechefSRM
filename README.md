# CodechefSRM

# TASK 1
## Q1
Error is in the 5th Line -> printf(" Enter a number"4589);

## Q2
Line 1 -> correct statemnet -> int *arr
Line 4 -> if to include all the value in the array loop should be -> for(int i=0;i<len;i++) as len-1 will add sum till 2nd last value and will not include the value at the last position
Line 7 -> correct statement sum+=*(arr+i)

## Q3
Line 4 -> for(int i=1;i<=4;i--) instead of i-- should  be i++ as incrementing value of i from 1 to 4

## Q4
Line 2 -> replace void main() by int main() as returning value
Line 4-> a>10?printf("Yes");:printf("No");  -> a (;) before (:) should not be there

## Q5
Line 4 -> corrected statemnet -> int o,i,s;
Line 7 -> coorected loop -> for(s=1 ; s<=5-o ; s++)
Line 9 -> corrected loop -> for (i=1 ; i<=o ; i++)
Line 10 -> correct statement -> cout<<"*";
Line 12 -> remove 1 (})

## Q6
Line 2-> invalid syntax
Line 3-> x is not defined/declared


## Q7
Line 4 -> ; after class is end 
Line 8,10,13 -> std function was not defined
Line 8,9 -> my-variable is private 
Line 13 -> odd is not declared

## Q8
Line 2 -> ; at the end required
Line 14 -> j was not declared , ; before <= , and ; before j , I was not declared
Line 20 -> ; after break
Line 30 -> s capital in printsums() as it's not declared

## Q9
Line 4 -> ; after Length
Line 5 -> " before enter
Line 7 -> [ instead of (
Line 11 -> , instead of ;
Line 19 -> return 0 instead of return std

## Q10
Line 2 -> # instead of *]
Line 3 -> no return type ex-> int main()
Line 6 -> , instead of ; before & and ; after scanf
Line 7 -> ; instead of , at the end of statement
Line 8 -> - istead of + as no. of test cases should decrease
Line 12 -> one of the = should be removed
Line 14 -> add 1 more } after }

# TASK 2

## Q1






## Q2

#include<bits/stdc++.h>
using namespace std;

int main(){
    int n;
    cout<<"size of array = ";
    cin>>n;
    int a[n];
    cout<<"Array [] = ";
    for(int i=0;i<n;i++){
        cin>>a[i];
    }
    int k;
    cout<<"Kth element = ";
    cin>>k;
    sort(a,a+n);
    for(int i=0;i<n;i++){
        if(k==i+1){
            cout<<a[i]<<endl;
        }
        
    }
    return 0;
}

## Q3
#include<bits/stdc++.h>
using namespace std;

int main(){
    char a;
    for(a='A';a<='Z';a=a+2){
            if(a=='C' || a=='G' || a=='K' || a=='O' || a=='S' || a=='W'){
                a=a+32;
                cout<<a<<endl;
                a=a-32;
            }
            else
                cout<<a<<endl;
         }
}

## Q4


#include <bits/stdc++.h>

using namespace std;

int main()
{
    int n;
    cin>>n;
    int sq=pow(n,2);
    
    int count=0;
    int c=sq;
    int b=sq;
    int num1=0,m=0;
    while (sq != 0)
    {
        sq = sq / 10;
        count++;
    }
    if(count%2!=0){
        m=count/2 +1;
    }
    else{
        m=count/2;
    }
    for(int i=0;i<m;i++){
         int rem= c%10;
         num1=rem+10*num1;
         c = c / 10;
        
    }
    int d=0;
    while(num1!=0){
        int rem= num1%10;
         d=rem+10*d;
         num1 = num1 / 10;
    }
    b=b-num1;
    int num2=b/pow(10,m);
    
    if((d+num2)==n){
        cout<<"Chef Number"<<endl;
    }
    else
        cout<<"Not Chef Number"<<endl;
    return 0;
}    
    





