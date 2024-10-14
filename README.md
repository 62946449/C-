# C-
#include<math.h>
double A(double V)
{
	double angle, sin_result;
	angle = V;
	angle = V * 3.14159 / 180.0;
	sin_result = sin(angle);//M_PI换3.14159
	return sin_result;
}
int F(int x,int y)
{
	int w = pow(x,5);
		return x*y*w;
}
int arr[] = {10,2,60,35,25,26,58};
int a = arr[5];
int b = arr[3];

int M(int x, int y)
{
	return x+y;
}


#pragma warning(disable:4996)
#include<stdio.h>
extern int F(int x, int y);
extern int M(int x, int y);
extern double A(double V);
#define add(x, y)(x / y )
extern int a, b;
 int main()
{
	double H;
	printf("请输入一个角度\n");
	scanf("%lf",&H);
	printf("%.4lf\n",A(H));
	int m, n;
	printf("请输入两个数\n");
	scanf("%d%d", &m, &n);
	printf("%d\n",  F(m,n));
	printf("请输入十个数\n");
	int num, max, i = 1, sum;
	scanf("%d",&num);
	max = num;
	while (i < 10)
	{
		scanf("%d", &num);
		i++;
		if (max < num)
			max = num;
		sum = max;
	}
	  printf("max=%d\n",sum);
	  int D=15;
	  printf("请输入一个数\n");
	  scanf("%d",&D);
	  printf("%d\n",M(D,sum));
	  printf("%d\n",add(a,b));
	  return 0;
}



