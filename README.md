
#include <stdio.h>
#include <unistd.h>
#include <function.h>
#include <math.h>
#include <string.h>


//structure
struct Records
{
  int no;
  char name[100];
  char company[100];
  char phone[15];
  char email[255];
  struct Records *next;
};

//functions
void fshowall (struct Records *head)
    {
        printf ("No.\tName\tCompany\tPhone\tE-mail");
        struct Records *temp = head;
        while (temp != NULL){
            printf ("\n%d\t%s\t%s\t%s\t%s", temp->no, temp->name, temp->company, temp->phone, temp->email);
            temp = temp->next;
            
        }

void fadd (struct Records *head){
    struct Records *temp 
        printf ("Please input the Name: ");
        gets ("%s", temp->name);
        printf ("\nPlease input the Company: ");
        gets ("%s", temp->company);
        printf ("\nPlease input the Phone: ");
        gets ("%s", temp->phone);
        printf ("\nPlease input the E-mail: ");
        gets ("%s", temp->email);
        //puts in *head+n = *temp 
        //printf ("\nRegistered successfully!");
  }

void fmodify (struct Records *head) {
        //to find the number of contactlist
        //to change the infor using same function of adding contactlist
        //replace the info
        //close
  }

void fdelete (struct Records *head){
// find contact
// delete contact
// reread, renew 

  }

void fsearch (struct Records *head){
//ask for input
// partial names?
//find in files
// read from files
// close

  }

//quit the program
void fquit (){
  //  break;
  }


int main (){
    //condition
    struct Records *head = nullptr;
    int i, conc_counter = 0;

    // OPEN FILE
    FILE *fptr, *fw;
    fptr = fopen ("conctactlist.txt", "r");
    fw = fopen ("contactlist.txt", "w");


    // CLOSE FILE
    
    
    while(int rep=1){
    	printf (">Welcome to Coffee Contacts!\n");
    	printf ("\n");
    	char input;
    	printf (">Please input: \n");
    	printf ("(Note: please input single alphabet)\n ");
    	printf ("\n");
    	printf
    	  (" -> i -- show all contacts\n -> a -- add a new contact\n -> m -- modify a contact\n -> d -- delete a contact\n -> s -- search a contact by name\n -> q -- quit the program\n ");
    	scanf ("%c", &input);
    	switch (input)
    	  {
    	  case 'i':
    	    fshowall (*head);
    	    return rep;
    
    	  case 'a':
    	    fadd (*head);
    	    return rep;
    
    	  case 'm':
    	    // statements
    	    fmodify (*head);
    	    return rep;
    
    	  case 'd':
    	    // statements
    	    fdelete (*head);
    	    return rep;
    
    	  case 's':
    	    // statements
    	    fsearch (*head);
    	    return rep;
    
    	  case 'q':
    	    fquit ();
    	    printf ("Program Quitted!");
    	    break;

	  }

      fopen ()
      fclose ()
        
    }
  }
