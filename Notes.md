##### Add Element to LinedList
```
public class Main {
    public static void main(String[] args) {
        int arr[] = {2, 4, 5, 1, 7, 7, 1};
        Node obj = new Node(arr[2]);
        System.out.println(obj.data);
    }
}

class Node {
    int data;
    Node next;

    Node(int data, Node next) {
        this.data = data;
        this.next = next;
    }

    Node(int data) {
        this.data = data;
        this.next = null;
    }
}

```

##### Convert Array to LinkedList 
```
public class Main {
    public static void main(String[] args) {
        int arr[] = {2, 4, 5, 1, 7, 7, 1};
        Node head = convertARRtoLL(arr);
        System.out.println(head.data);
    }

    private static Node convertARRtoLL(int[] arr) {
        Node head = new Node(arr[0]);
        Node mover = head;
        for (int i = 1; i < arr.length; i++) {
            Node temp = new Node(arr[i]);
            mover.next = temp;
            mover = temp;
        }
        return head;
    }
}

class Node {
    int data;
    Node next;

    Node(int data, Node next) {
        this.data = data;
        this.next = next;
    }

    Node(int data) {
        this.data = data;
        this.next = null;
    }
}

```
##### Traverse to LinkedList 
```
public class Main {
    public static void main(String[] args) {
        int arr[] = {2, 4, 5, 1, 7, 7, 1};
        Node head = convertARRtoLL(arr);
        Node temp = head;

        while(temp != null){
            System.out.println(temp.data);
            temp = temp.next;

        }

    private static Node convertARRtoLL(int[] arr) {
        Node head = new Node(arr[0]);
        Node mover = head;
        for (int i = 1; i < arr.length; i++) {
            Node temp = new Node(arr[i]);
            mover.next = temp;
            mover = temp;
        }
        return head;
    }
}

class Node {
    int data;
    Node next;

    Node(int data, Node next) {
        this.data = data;
        this.next = next;
    }

    Node(int data) {
        this.data = data;
        this.next = null;
    }
}

```
#####Length of the LinkedList

```
public class Main
{
	public static void main(String[] args) {
	    int arr[] = {2,4,5,1,7,7,1};
		Node head = convertARRtoLL(arr);
		Node temp = head;
		int count = 0;
		while(temp != null){
		    count++;
		    temp = temp.next;
		}
		System.out.println("length of this LinkedList is: " + count);
		
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
```
#####Length of the LinkedList

```

public class Main {
    public static void main(String[] args) {
        int arr[] = {2, 4, 5, 1, 7, 7, 1};
        Node head = convertARRtoLL(arr);
        System.out.print("Length of LinkedList is: " + LengthofLinkedList(head));
        
}
    private static Node convertARRtoLL(int[] arr) {
        Node head = new Node(arr[0]);
        Node mover = head;
        for (int i = 1; i < arr.length; i++) {
            Node temp = new Node(arr[i]);
            mover.next = temp;
            mover = temp;
        }
        return head;
    }
    public static int LengthofLinkedList(Node head){
        Node temp = head;
        // if(temp = null){
        //     return null;
        // }
        int count = 0;
        while (temp != null) {
            count++;
            temp = temp.next;
        }
        return count;
        
    }
}

class Node {
    int data;
    Node next;

    Node(int data, Node next) {
        this.data = data;
        this.next = next;
    }

    Node(int data) {
        this.data = data;
        this.next = null;
    }
}

```
#####  

   

