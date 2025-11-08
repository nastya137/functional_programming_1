class Solution {
public:
    int maxProfit(vector<int>& prices) {
        return findMaxProfit(prices, 0, prices[0], prices[0], 0);
    }
    int findMaxProfit(vector<int>& prices, int i, int max, int min, int sum) {
        if(i>=prices.size()) return sum+(max-min);
        if(prices[i]<max){
            sum+=max-min;
            min = prices[i];
        }
        max = prices[i];
        return findMaxProfit(prices, i+1, max, min, sum);
    }
};
