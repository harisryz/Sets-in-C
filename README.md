# Sets-in-C
#include<stdio.h>
#include<conio.h>
int main()
{
int a[10],b[10],i,j,n,m,rel;
clescr();
printf("enter the limt for domain a\n");
scanf("%d",&n);
printf("enter the values of domian a\n");
for(i=0;i<n;i++)
{
scanf("%d",&a[i]);
}
printf("enter the limt for codomain\n");
scanf("%d",&m);
printf("enter the values for codomain\n");
for(j=0;j<m;j++)
{
scanf("%d",&b[j]);
}
printf("for realtion a*b press 1,\n for realation a/b press 2\n ");
printf("for realtion a=b press 3\n for realation a^2 press 4\n");
scanf("%d",&rel);
switch(rel)
{
case 1:
if(rel==1)
{
for(i=0;i<n;i++)
{
for(j=0;j<m;j++)
{
printf("%d*%d\t=%d\n",a[i],b[j],a[i]*b[j]);
}
}
}
case 2:
if(rel==2)
{
for(i=0;i<n;i++)
{
for(j=0;j<m;j++)
{
if(a[i]%b[j]==0)
{
printf("(%d,%d)",a[i],b[j]);
}
}
}
}
case 3:
if(rel==3)
{
for(i=0;i<n;i++)
{
for(j=0;j<m;j++)
{
if(a[i]==b[j])
{
printf("(%d,%d)",a[i],b[j]);
}
}
}
}
case 4:
if(rel==4)
{
for(i=0;i<n;i++)
{
for(j=0;j<m;j++)
{
if(b[j]==a[i]*a[i])
{
printf("(%d,%d)",a[i],b[i]);
}
}
}
}
}

getch();
return(0);
}
