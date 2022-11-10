//# palindrom-number.c//
#include<stdio.h>
int main()
{
    int n,rev=0,rem,org;
    printf("Enter four digit number");
    scanf("%d",&n);
    org=n;
    while(n!=0)
    {
        rem=n%10;
        rev=rev*10+rem;
        n/=10;
    }
    if(org==rev)
    {
        printf("%d is palindrome.",org);
    }
    else
    {
        printf("%d is not a palendrome.",org);
    }
    return 0;
}
