#include<iostream>
using namespace std;

struct node {
	public:
	int data;
	node *next ; 
};
 node *head =NULL;
 
 void insert (int n){
 node *newnode = new node();
 newnode->data = n;
 newnode->next =  head;
 head = newnode;
 
 }
 void print(){
 	cout<<"Data element in single link list:"<<endl;
 	 node *temp = head;
 	  while(temp!=NULL){
 	  cout<<	temp->data<<" ";
 	     temp= temp->next;
	   }
 }
 
	
int main(){
	insert(1);
	insert(2);
	insert(3);
	insert(4);
	insert(5);
	print();
	
}
