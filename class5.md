# Linked Lists
  Linked lists are linear data structures that hold data in individual objects called nodes. These nodes hold both the data and a reference to the next node in the list.
  
  
  ![s](https://res.cloudinary.com/practicaldev/image/fetch/s--y3j6aJXJ--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://res.cloudinary.com/practicaldev/image/fetch/s--_PwtVEkJ--/c_limit%252Cf_auto%252Cfl_progressive%252Cq_auto%252Cw_880/https://www.educative.io/api/edpresso/shot/5077575695073280/image/5192456339456000)
  

### Linked types:

  - Singly : Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.

  - Doubly : Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

  - Node : is the individual items/links that live in a linked list. Each node contains the data for each link.

  - Singly : refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the `Next` node in a linked list.

  - Doubly : refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the `Next` and `Previous` node.

  - Next : This property contains the reference to the next node.

  - Head : This property contains the reference to the first node in a linked list.

  reference is a reference type of type Node that is currently being looked at. This node is traditionally used when traversing through a full linked list. When traversing, you typically reset the current to the head to guarantee you are starting from the beginning of the linked list.

  >The `Next` property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.

  >The best way to approach a traversal is through the use of a while loop. This allows us to continually check that the Next node in the list is not null.
