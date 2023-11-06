# Create-Target-Array-in-the-Given-Array-using-Java-Leetcode

    class Solution {
        public int[] createTargetArray(int[] nums, int[] index) {
            ArrayList<Integer> target = new ArrayList<Integer>();
            int ans[] = new int[nums.length];
            for(int i =0; i<nums.length;i++){
                target.add(index[i],nums[i]);
    
            }
            for(int j =0;j<nums.length;j++){
                ans[j]= target.get(j);
            }
            return ans;
        }
    }
