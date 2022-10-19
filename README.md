# LeetCode_Interview_Questions

## 1. Two Sum

```c
class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        
        vector<int> temp;
        int size = nums.size();
        
        for(int i=0;i<(size-1);i++)
        {
            for(int j=i+1;j<size;j++)
            {
                if(nums[i]+nums[j]==target)
                {
                    temp.push_back(i);
                    temp.push_back(j);
                    return temp;
                }
            }
        }
        return temp;
    }
};
```
---

## 2. Add Two Numbers

```c
class Solution {
public:
    ListNode* addTwoNumbers(ListNode* l1, ListNode* l2) {
        ListNode* preHead = new ListNode();
        ListNode* curr = preHead;
        int sum = 0;
        int carry = 0;
        while(l1 != NULL || l2 != NULL || carry){
            if(l1 != NULL){ sum += l1->val; l1 = l1->next; }
            if(l2 != NULL){ sum += l2->val; l2 = l2->next; }
            curr->next = new ListNode(sum%10);
            curr = curr->next;
            sum = carry = sum > 9;
        }
        return preHead->next;
    }
};
```
----

## 3. Longest Substring Without Repeating Characters

```c

```
---

## 4. Median of Two Sorted Arrays

```c

```
---

## 5. Longest Palindromic Substring

```c

```
---

## 7. Reverse Integer

```c
class Solution {
public:
    int reverse(int x) {
        
         long long rev = 0;
        
        while(x){
            
            int digit = x%10;
            x = x/10;
            rev = rev*10 + digit;
            
            //checking boundaries
            if(rev<INT_MIN or rev>INT_MAX)
                return 0;
        }
        
        return (int)rev;
        
    }
};

```
---

## 8. String to Integer (atoi)

```c

```
---

## 10. Regular Expression Matching

```c

```
---

## 11. Container With Most Water

```c

```
---

## 13. Roman to Integer

```c

```
---

## 14. Longest Common Prefix

```c

```
---

## 15. 3Sum

```c

```
---

## 17. Letter Combinations of a Phone Number

```c

```
---

## 19. Remove Nth Node From End of List 

```c

```
---

## 20. Valid Parentheses
