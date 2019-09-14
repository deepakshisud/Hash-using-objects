#include<iostream>
using namespace std;
struct node
{
	int data;
	node* next;
};
class LinkedList
{
	public:
		node* head=NULL;
    //inserting the element in same linked list
		void insertend(int new_data)
		{
		struct node* newn=new node();
		newn->data=new_data;
		newn->next=NULL;
		if(head==NULL)
		head=newn;
		else
		{
		struct node* temp=head;
		while(temp->next!=NULL)
			temp=temp->next;
		temp->next=newn;
		}
		}
		void disp()
		{
			node* temp=head;
			while(temp!=NULL)
			{
				cout<<temp->data<<" ";
				temp=temp->next;
			}
		}
};
int main()
{
	int m,n,k;
  //m is the number to be divided by
  //n is the no of elements
  //k contains each element in the loop
	cout<<"Enter the value of m: ";
	cin>>m;
	LinkedList ob[m];
	cout<<"Enter the no. of elements: ";
	cin>>n;
	cout<<"Enter the elements: "<<endl;
	for(int i=0;i<n;i++)
	{
		cin>>k;
		int h=k%m;
		ob[h].insertend(k);
	}
	for(int i=0;i<m;i++)
	{
		cout<<i<<":";
		ob[i].disp();
		cout<<endl;
	}
}
