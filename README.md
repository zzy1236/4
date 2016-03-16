#include &lt;stdlib.h&gt;
#include &lt;string.h&gt;
#include &lt;stdio.h&gt;
#include &lt;iostream.h&gt;

int main(int argc, char* argv[])
{

char x[1000];
unsigned int i=0 ;
int n=0 ;
char flag=0;


cin.getline(x,255);
strcat(x," ");

for(i=0;i&lt;strlen(x);i++)
{
 if(((x[i]&gt;='a')&amp;&amp;(x[i]&lt;='z'))||((x[i]&gt;='A')&amp;&amp;(x[i]&lt;='Z')))
 { flag=1;}
 else
 {
 if (flag==1 ) n++; 
 flag=0;
 }

}


printf("%d\n",n);

getchar();
return 0;
}
