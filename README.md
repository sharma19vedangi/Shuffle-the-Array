# Shuffle-the-Array
#Array Leetcode Problem Solution
class Solution {
    public int[] shuffle(int[] nums, int n) {
        int a[]=new int[n+n];
        int k=0;
        for(int i=0;i<n;i++)
        {
            a[k]=nums[i];
            a[k+1]=nums[n+i];
            k=k+2;
        }
        return a;
    }
}
