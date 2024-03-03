/**
 * Definition for singly-linked list.
 * public class ListNode {
 * int val;
 * ListNode next;
 * ListNode() {}
 * ListNode(int val) { this.val = val; }
 * ListNode(int val, ListNode next) { this.val = val; this.next = next; }
 * }
 */
class Solution {
    public ListNode removeNthFromEnd(ListNode head, int n) {

        int length = 0;
        ListNode temp = head;
        while (temp != null) {
            length++;
            temp = temp.next;
        }
        int nthfromstart = length - n - 1;
        if (nthfromstart == -1) {
            return head.next;
        }
        int i = 0;
        ListNode curr = head;
        while (i < nthfromstart) {
            curr = curr.next;
            i++;
        }

        curr.next = curr.next.next;
        return head;
    }
}
