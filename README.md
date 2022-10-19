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

## 2. 
