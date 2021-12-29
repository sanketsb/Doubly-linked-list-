#include<stdio.h>
#include<conio.h>
#include<stdlib.h>
struct node
{
   int data;
   struct node *Llink,*Rlink;
};
  struct node *head=NULL,*NEW;
   int item;
void create();
void insert_beg();
//void delete_beg();
//void insert_end();
//void delete_end();
//void insert_pos();
//void delete_pos();
void Ftraverse();
void Btraverse();
 int main()
 {
    int ch;
    clrscr();
    printf("\n1.Insert at begin,\n2.delete at begin,\n3.Insert at end,\n4.delete at end,\n5.insert at position,\n6.delete at position,\n7.Ftraverse,\n8.Btraverse,\9.exit\n");
    do
    {
    printf("\nEnter the choice: ");
    scanf("%d",&ch);
       switch(ch)
       {
	 case 1: insert_beg();
		 break;
	/* case 2: delete_beg();
		break;
	 //case 3: insert_end();
		break;
	 //case 4: delete_end();
		break;
	 //case 5:insert_pos();
		break;
	  case 6:delete_pos();
	       break;*/
	 case 7:Ftraverse();
		break;
	 case 8:Btraverse();
		break;
	 case 9: exit(0);
	  default: printf("Enter correct choice");
	  }
    }while(ch<10);
    getch();
    return 0;
 }
   void create()
   {
     NEW=(struct node*)malloc(sizeof(struct node));
    printf("\nEnter the  number: ");
    scanf("%d",&item);
    NEW->Llink=NULL;
    NEW->data=item;
    }

    void insert_beg()
    {
      create();
      if(head==NULL)
      {
	 head=NEW;
	    NEW->Rlink=NULL;
      }
      else
      {
	   NEW->Rlink=head;
	   head->Llink=NEW;
		 head=NEW;
      }

    }
    void Ftraverse()
    {  struct node   *temp;
      if(head==NULL)
      {
	  printf("\nlinked list is empty");
    }
     else
     {
     temp=head;
	while(temp!=NULL)
	{
	 printf("%d->",temp->data);
	 temp=temp->Rlink;
	}
	printf("NULL");

     }
    }

    void Btraverse()
    {
     struct node *temp=head;
     printf("NULL->");
     while(temp->Rlink!=NULL)
     {
      temp=temp->Rlink;
     }
     while(temp!=NULL)
     {
	printf("%d->",temp->data);
	temp=temp->Llink;
     }
    }
