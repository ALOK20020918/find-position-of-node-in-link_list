# find-position-of-node-in-link_list
# You have been given a singly linked list of integers. Write a function that returns the index/position of integer data denoted by 'N' (if it exists). Return -1 # #    otherwise.

	public static int  position(Node<Integer>head,int n) {
		if(head==null) {
			return -1;
		}
		int len=0;
		Node<Integer>temp=head;
		while(temp!=null) {
			if(temp.data.equals(n)) {
				return len;
			}
			len++;
			temp=temp.next;
		}
		return -1;
	}


