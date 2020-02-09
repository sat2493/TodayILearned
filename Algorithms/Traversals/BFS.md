# Breadth-First Search

TIL that I could implement BFS in JavaScript through the following:

```
Code structure taken from: https://github.com/sat2493/TodayILearned/blob/master/Data%20Structures/Queues.md
I revised to add queue characteristics

function levelOrderSearch(rootNode) {
  // Check that a root node exists.
  if (rootNode === null) {
    return;
  }
  
  // Create our queue and push our root node into it.
  var queue = new Queue();
  queue.enqueue(rootNode);
  
  // Continue searching through as queue as long as it's not empty.
  while (!queue.isEmpty()) {
    // Create a reference to currentNode, at the top of the queue.
    var currentNode = queue.front();
    
    // If currentNode has a left child node, add it to the queue.
    if (currentNode.left !== null) {
      queue.enqueue(currentNode.left)
    }
    // If currentNode has a right child node, add it to the queue.
    if (currentNode.right !== null) {
      queue.enqueue(currentNode.right)
    }
    // Remove the currentNode from the queue.
    queue.dequeue()
  }
  
  // Continue looping through the queue until it's empty!
}
```
