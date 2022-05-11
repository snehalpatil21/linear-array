# linear-array
#include<iostream.h>
#include<conio.h>
class arr
{
	int a[10],n,s;

	public:
		arr()
	{
		s= -1;
	}
	void get();
	void search();
};


void arr::get()
{
	cout<<"enter size of array"<<endl;
	cin>>n;
	cout<<"enter array elements "<<endl;
	for(int i=0;i<=n;i++)
	{
		cin>>a[i];
	}
	cout<<"Elements are"<<endl;
	for(int j=0;j<=n;j++)
	{
		cout<<a[j]<<"  "<<endl;
	}
	cout<<endl;
}
void arr::search()
{
	int ele;
	cout<<"Enter any element ";
	cin>>ele;
	for(int i=0;i<n;i++)
	{
		if (a[i]==ele)
		{
			s=i;
		}
	}
	if (s==-1)
	{
		cout<<"Element Are Not Found";
	}
	else
	{
		cout<<"Element Are Found";
		cout<<endl;
		s=s+1;
		cout<<"Position Of Element   ";
		cout<<s;
	}
}
int main()
{
	clrscr();
	arr a;
	a.get();
	a.search();
	getch();
	return(0);
}
