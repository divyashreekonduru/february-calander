# include<stdio.h>
# include<stdlib.h>
{
int   n,days;
char a[5];
scanf(“%d  %s”,&n,a);
if(n%4==0)
{
if(n%100==0)
{
if(n%400==0)
days=29;
else days=28;
}
else
days=19;
}
else  days=28;
char  b[]={ “SUN”,”MON”,”TUE”,”WED”,”THU”,”FRI”,”SAT”};
int I,j,k=31,count,l=1;
for(i=0;i<7;i++)
{
printf(“%c  “,b[i]);
}
for(i=0;i<7;i++)
{
if(strcmp(a,b[i])==0)
{
count=I;
break;
}
}
int x=(k+count)%7;
printf(“\n”);
for(i=0;i<7;i++)
{
if(x==i)
{
printf(“%d  ”,l++);
printf(“\n”);
while(1)
{
for(i=0;i<7&&l!=days+1;i++,l++)
{
printf(“%d   “,l);
if(l==days+1)
break;
else
printf(“\n”);
}
for(j=i;j<7;j++)
printf(“*  “);
