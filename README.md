# program-for-removing-duplicates-in-a-linked-list-in-c-
prgrm for removing duplicate node in a SLL in c++
Node* removeDuplicates(Node* head) {
        // code here
        Node* temp=head;
        while(temp!=NULL && temp->next!=NULL){
            if(temp->data==temp->next->data){
                temp->next=temp->next->next;
            }
            else{
                temp=temp->next; 
            }
            
        }
        return head;
        
    }
