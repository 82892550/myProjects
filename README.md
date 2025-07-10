class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        vector<int> resultArray(2);
        for (int i = 0; i < nums.size(); i++) {
            for (int k = i + 1; k < nums.size(); k++) {
                if (nums.at(i) + nums.at(k) == target) {

                    resultArray[0] = i;
                    resultArray[1] = k;
                    return resultArray;
                }
            }
        }
        return resultArray;
    }
};
