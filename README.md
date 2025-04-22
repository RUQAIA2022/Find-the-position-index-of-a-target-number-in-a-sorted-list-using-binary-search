# Find-the-position-index-of-a-target-number-in-a-sorted-list-using-binary-search
Algorithm Steps:
1.
low = 0 (beginning of the list)
high = length of the list - 1 (end of the list)
2.
Repeat the following steps while low is less than or equal to high:

Calculate the middle index:
mid = (low + high) // 2

Check the value at the middle:

If arr[mid] equals the target →  Return mid

If arr[mid] is less than the target →  Move to the right half:
low = mid + 1

If arr[mid] is greater than the target → Move to the left half:
high = mid - 1
3.
If the loop ends without finding the target:
Return -1 (target not found)

 Example:
For the array: [2, 4, 6, 8, 10, 12, 14]
And target: 10

The algorithm finds 10 at index 4
