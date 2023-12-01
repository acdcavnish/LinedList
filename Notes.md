## Add Element to LinedList

public class Main
{
	public static void main(String[] args) {
	    int arr[] = {2,4,5,1,7,7,1};
 	    Node obj = new Node(arr[2]);
 		  System.out.println(obj.data);
	}
}

class Node{
    int data;
    Node next;
    
    Node(int data, Node next){
        this.data = data;
        this.next = next;
    }
    
    Node(int data){
        this.data = data;
        this.next = null;
    }
    
}

## Convert Array to LinkedList 

public class Main
{
	public static void main(String[] args) {
	  int arr[] = {2,4,5,1,7,7,1};
		Node head = convertARRtoLL(arr);
		System.out.println(head.data);
	}
	
	    private static Node convertARRtoLL(int[] arr){
        Node head = new Node(arr[0]);
        Node mover = head;
        for(int i = 1;i<arr.length;i++){
            Node temp = new Node(arr[i]);
            mover.next = temp;
            mover = temp;
        }
        return head;
    }
}

class Node{
    int data;
    Node next;
    
    Node(int data, Node next){
        this.data = data;
        this.next = next;
    }
    
    Node(int data){
        this.data = data;
        this.next = null;
    }
    
}

