#include<iostream>
using namespace std;

struct Element{
	int data;
	Element *link;
};

class Stack{
	private:
		Element *top;
	public:
		Stack(){
			top==NULL;
		}
		
	void push(int i);
	int pop();
	void viewAll();
	
	~Stack(){
		if (top==NULL)
		return;
		Element *temp;
		while (top!=NULL){
			temp=top;
			top=top->link;
			delete temp;
		}
	}
};
void Stack::push(int i){
	Element *temp;
	temp=new Element;
	temp->data=i;
	temp->link=NULL;
	if (top==NULL){
		top=temp;
	}
	else{
		temp->link=top;
		top=temp;
	}
}

int Stack::pop(){
	Element *temp;
	int n;
	if (top==NULL){
		cout<<"Stack Empty"<<endl;
		return NULL;
	}
	else{
		n=top->data;
		temp=top;
		top=top->link;
		delete temp;
	}
	return n;
}

void Stack::viewAll(){
	Element *temp;
	temp=top;
	while(temp->link !=NULL){
		cout<<temp->data<<endl;
		temp=temp->link;
	}
}

int main(){
	Stack q;
	int temp;
	int pil;
	while(1){
		cout<<"=====Implementasi Stack dengan Linked List====="<<endl;
		cout<<"=============Annisa Nurwalikadani=============="<<endl;
		cout<<"==================1817051037==================="<<endl<<endl;
		cout<<"1. Push data"<<endl;
		cout<<"2. Pop data"<<endl;
		cout<<"3. View All Data"<<endl;
		cout<<"4. Exit"<<endl;
		cout<<"Tentukan pilihanmu : ";
		cin>>pil;
	switch(pil){
		cout<<endl;
		case 1:
			cout<<"Masukkan data : "<<endl;
			cin>>temp;
			q.push(temp);
			break;
		case 2:
			temp=q.pop();
			cout<<temp<<" tehapus"<<endl;
			break;
		case 3:
			q.viewAll();
			break;
		case 4:
			return 0;
		default:
			cout<<endl<<"Pilihan anda tidak tersedia"<<endl;
		}
	}
	return 0;
	}
