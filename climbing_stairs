class Solution {
public:
    int climbStairs(int n) {
        if(n<3) return n;
        return count_ways(n, 2, 1, 3);
    }
    int count_ways(int n, int first, int second, int i){
        if(i>n) return first;
        int x = first;
        first+=second;
        second = x;
        return count_ways(n, first, second, i+1);
    }
};
