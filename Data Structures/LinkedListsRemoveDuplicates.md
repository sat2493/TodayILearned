# Removing Duplicates From Linked Lists

TIL how to remove duplicates from a linked list using JavaScript using a hashmap data structure

```
function removeDuplicates(head) {
    let hashMap = {};
    let cur = head;
    let prev;

    [4, 4, 4, 5]
    while(cur !== null) {
        if (hashMap[String(cur.val)] === undefined) {
            hashMap[String(cur.val)] = 1;
            prev = cur;
        } else {
            hashMap[String(cur.val)]++;
            prev.next = cur.next;
        }
        cur = cur.next;
    }
}
```
