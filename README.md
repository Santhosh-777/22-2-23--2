#include<stdio.h>
 main()
{
    int n,k,i,esum,osum,cnt;
    cnt=esum=osum;
    scanf("%d%d",&n,&k);
    i=1;
    while(i<=n)
    {
        if(i%k==0)
        {
        printf("%d\n",i);
        cnt++;
        if(i%2==0)esum=esum+i;
        else
        osum+=i;
        }
        i++;
    }
    
    printf("\n count=%d",cnt);
    printf("\neven sum=%d",esum);
    printf("\nodd sum=%d",osum);
}
