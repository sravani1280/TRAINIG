class Solution {

public:

    int maxProfit(vector<int>& prices) {
    
        int min_price=INT_MAX;
        
        int profit=0;
        
      int n = prices.size();
      
        int i;
        
        for(i=0;i<n;i++)
        
        {
        
            min_price = min(prices[i],min_price);
            
            profit = max(profit,prices[i]-min_price);
            
        }
        
        return profit;
        
    }
    
};
