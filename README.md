#include<stdio.h>
int main()
{
		int n,w,q,b,s,g;
		scanf("%d",&n);
		g=n%10;
		s=n/10%10;
		b=n/100%10;
		q=n/1000%10;
		w=n/10000%10;
		if(w!=0) printf("5\n%d %d %d %d %d\n%d%d%d%d%d\n",w,q,b,s,g,g,s,b,q,w);
		else if(q!=0) printf("4\n%d %d %d %d\n%d%d%d%d\n",q,b,s,g,g,s,b,q);
		else if(b!=0) printf("3\n%d %d %d\n%d%d%d\n",b,s,g,g,s,b);
	else if(s!=0) printf("2\n%d %d\n%d%d\n",s,g,g,s);
		else  printf("1\n%d\n%d\n",g,g);
		return 0;
}
