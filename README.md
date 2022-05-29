# -
找走丢的数（找单身狗）
int missingnumber(int* nums,int numsize)
{
	int x=0;
	for (int i = 0; i <=numsize; ++i)//先跟0~N异或
	{
		x ^= i;

	}
	for (int i = 0; i < numsize;++i)//在跟数组中的值异或
	{
		x ^=nums[i];

	}
	return x;
}
