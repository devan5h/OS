#include<stdio.h>
#include<stdlib.h>
void FIFO(char [J,char [ ],int,int);|
void Iru(char [ ],char [ ],int,int);|
void opt(char [ ],char [ J,int,int);
int main()
{
int ch, YN=1,i,l,f;
char F[10],s[25];
printf("|n|n\tEnter the no of empty frames: "):
scanf("%d",&f);
printf("|n|n\tEnter the length of the string: ");
scanf("%d", &1);
printf("|n|n|tEnter the string: "):
scanf("%s",.s);
for(i=0;i<f;i++)
F＝-1；
do
{
printf("n|n\*********** MENU ***********");
printf("|n|n|t1:FIFO|n|n|2:LRU (n|n\t4:EXIT";
printi("|n\n|tEnter your choice: ");
scanf("%d",&ch);|

switch(ch)
{
case 1:
for(i=0;i<f;i++)
FIFO(s,F,1,f):
break; case 2:
for(i=0;i<f;i++)
Fi=1：
}
Iru(s,F,I,f);
break; case 4:
exit(0);
printf("(n\n|tDo u want to continue IF YES PRESS 1\n\n|tIF NO PRESS 0: "):
scanf("%d",& YN);
/while(YN==1):
return(0):
｝
//FIFO
void FIFO(char sO.char F[.int l,int f)
{
int i.j=0,k,flag=0,cnt=1; |
printf("n\tPAGE\t FRAMES(t FAULTS");
for(i=0;i<l;i++)
{
for(k=0;k<f;k++)
{
if(F[k)==s[i))
flag=1;
}
if(flag==0)
{
printf("\n\t%c\t*,s[i|):
Fil=sil:
j++;
for(k=0;k<f;k++)
{
printf(" %c", F[k);
｝
printf("\tPage-fault%d",cnt);
cnt++;
else
{
flag=0;
printf("|n\t%c\t",s[il):
fork=0;k<f;k++)
{
printf(" %c",F[k]);
}
printf("\tNo page-fault"):
if（j==f）
j=0;
｝
}
//LRU
void Lru(char s[].char F(,int l,int f)
{
int i.j=0,k,m,flag=0,cnt=1,top=0; |
printf"\n\tPAGE)t FRAMES(t FAULTS");
for(i=0;i<l;i++)
{
fork=0;k<f;k++)
{
if(F[k)==s[i)
{
flag=1; break;}
}
printf("\n\t%c\t",s(i);
if(j!=f&& flag!=1)
{
F[top)=s[i);
j++;
if(j!=1)
  top++;
else
{
if(flag!=1)
{
if(flag==1)
{
for(k=0;k<top;k++)
FIK=FIk+11：
}
F[top)=s[i):
}
if(flag==1)
{
for(m=k;m<top;m++)
F(m)=F(m+1];
}
F[top]=s[i);
｝
｝
fork=0;k<f;k++)
{
printf(" %c",F(k]):
}
if(flag==0)
{
printi("|tPage-fault%d",cnt);
cnt++;
}
else
printf("Print No page fault);

flag=0;
}
