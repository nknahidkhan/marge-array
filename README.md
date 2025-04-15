# marge-array
#include<stdio.h>
int main()
{
  int m,n,i;
  scanf("%d",&m) ;
  scanf("%d",&n) ;
  int a[m],b[n];
  int marge[m+n];
  for(i=0;i<m;i++)
  {
      scanf("%d",&a[i]);
  }

  for(i=0;i<n;i++)
  {
      scanf("%d",&b[i]);
  }
  for(i=0;i<m;i++)
  {
      marge[i]=a[i];
  }
  for(i=0;i<n;i++)
  {
      marge[i+m]=b[i];
  }

  for(i=0;i<m+n;i++)
  {
      printf("%d",marge[m+n]);
  }




    return 0;
}
