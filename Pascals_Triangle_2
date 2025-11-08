class Solution {
public:
    vector<int> getRow(int rowIndex) {
        vector<int> row(1, 1);
        return createRow(rowIndex, row);
    }
    vector<int> createRow(int rowIndex, vector<int>& row){
        if(row.size()==rowIndex+1) return row;
        int a = 1;
        for(int i = 0; i<row.size()-1; i++){
            int b = row[i+1];
            row[i+1]=a+b;
            a=b;
        }
        row.push_back(1);
        return createRow(rowIndex, row);
    }
};
