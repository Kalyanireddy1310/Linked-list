# Linked-list
#singly linked list
import java.util.Scanner;
class node{
    int data;
    node next;
    node(int ele)
    {
        this.data=ele;
        this.next=null;
        
    }
}
    class LinkedList{
         node head=null, tail=null;
         void insert(int ele)
        {
            node nw=new node(ele);
            if(head==null)
            {
                head=nw;
                tail=nw;
            }
        
        else
        {
            tail.next=nw;
            tail=nw;
        }
        
    }
   void display()
    {
        node temp=head;
        while(temp!=null)
        {System.out.print(temp.data+" ");
        temp=temp.next;
        }
      }
    }
     class Main
      {
    
     
        
            public static void main(String[]args){
            Scanner sc= new Scanner(System.in);
            int ele;
              int n= sc.nextInt();
              
            LinkedList ll=new LinkedList();
            
            for(int i=0;i<n;i++)
            {
                ele=sc.nextInt();
               
                
                ll.insert(ele);
            }
                ll.display();
                } 
    
            
        }
