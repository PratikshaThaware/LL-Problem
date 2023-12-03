# LL-Problem
 static void PrintLL(Node head){
    while(head != null){
        System.out.println(head.data+" ");
        head = head.next;
    }
}
public static void main(String []args){
  Scanner sc = new Scanner(System.in);
  int n = sc.nextInt();
 Node head = null;
Node temp = null;
  for(int i=0; i<n; i++){
     int curr = sc.nextInt();
  
  if(head == null){
 head = new Node(curr);
  temp = head;
}
else{
    temp.next = new Node(curr);
    temp = temp.next;
    
}
}
PrintLL(head);
}
}
Input: 5
10 20 3 8 7 
output: 10 20 3 8 7
