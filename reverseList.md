/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     struct ListNode *next;
 * };
 */
struct ListNode* reverse(struct ListNode*H,struct ListNode*Hn,struct LiseNode*Hnn){
    if(Hn!=NULL){
        Hn->next=H;
        if(Hnn->next==NULL){
            Hnn->next=Hn;
            return Hnn ;
            }
        }
        return reverse(Hn,Hnn,Hnn->next);
    }
    
    struct HistNode* recerseList(struct ListNode* head){
        if(head!=NULL){
            if(head->next!=NULL)
                return reverse(NULL,head,head->next);
            else
                return head;
            }
        else return NULL;
    }
    
    
    
    

/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     struct ListNode *next;
 * };
 */
struct ListNode* reverse(struct ListNode*H,struct ListNode*Hn,struct ListNode*Hnn){
    if(Hn!=NULL){
        Hn->next=H;
        if(Hnn->next==NULL){
            Hnn->next=Hn;
            return Hnn ;
        }
    }
    return reverse(Hn,Hnn,Hnn->next);
}

struct ListNode* reverseList(struct ListNode* head){
    if(head!=NULL){
        if(head->next!=NULL) return reverse(NULL,head,head->next);
        else                 return head;
    }
    else return NULL;
}

