## Linked Lists - They Are That Easy!

Linked lists are perhaps the first data structure people learn after becoming familiar with arrays. It has fairly simple logic but it can be hard for beginners to grasp all the technical aspects right away. But, we can simply relate it with more tangible concepts and it does not feel as hard anymore!

To get a better understanding of this particular data structure type, we have to first figure out what the name means. Breaking down the name, we get 'linked' and 'list'. The data structure is exactly that - a list of 'items', which are 'linked' (not by similarity, rather just a link created from one 'item' to another). 

All types of linked lists consist of these 'items.' Each 'item' is called to be a **node** of the list.

We will be exploring singly linked lists for now.

### Singly Linked Lists

The easiest of the three, a singly linked list joins nodes using a *single link*.

As shown below, think of the node as a box, with one end having a hook, and the other end having a loop. 

![SLL Node.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1599969876067/Mq-22qvus.png)

After taking a number of these, and then putting the hook of one box into the loop of another box, we end up with a singly linked list! The image below shows four nodes linked to one another.

![SLL.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1599970348359/HnoirqMky.png)

We can say that the hooks are the 'links' to the next box. Since there is a hook only at the front, each box links only to the one after it. This means that the box has no idea about anything behind it. The 'hooks' that we have are actually called **pointers** because they, un-ironically, point to the next **node**! 

If you noticed a small detail, the first box does not have any hook attached to it and the last box does not have anything to attach the hook to! Otherwise, there is **nothing** behind the first box and **nothing** in front of the last box. This is why we attach *a head*, while the last node points to **NULL**.

![headerll.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1599971302107/eaclEA48P.png)

We use one node and its pointer to get information about the next node. Thus, a head allows us to keep track of where the list starts from. The last node points to NULL because the last node has no other node to point to. Just like we are using a head, one might suggest the usage of a tail. That is a really good suggestion (and it will come to use later on!), but remember how the nodes only point towards a *forward* direction? Having a tail will not really be useful as we cannot go backwards in a singly linked list. However, you can still have a tail to know what you last element is.

In summary, a singly linked list consists of nodes which point in one direction only.
