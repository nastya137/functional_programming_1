class Solution {
public:
    int jump(vector<int>& nums) {
        return count_jumps(nums, 0, 0);
    }
    int count_jumps(vector<int>& nums, int i, int n){
        if (i>=nums.size()-1) return n;
        if(i+nums[i]>=nums.size()-1) {
                return n+1;
                }
            int next_i = i;
            int value = 0;
            for(int j = i+1; j<=i+nums[i]; j++){
                if(nums[j]+j>=value){                   
                    value = nums[j]+j;
                    next_i = j;                    
                }
            }
        return count_jumps(nums, next_i, n+1);
    }
};
