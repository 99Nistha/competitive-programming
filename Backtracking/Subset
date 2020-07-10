void solve(vector<vector<int>> &ans, vector<int> &A, vector<int> prev, int pos)
{
    if (pos >= A.size())
    {
        return;
    }

    vector<int> tprev(prev.begin(), prev.end());
    prev.push_back(A[pos]);
    ans.push_back(prev);
    solve(ans, A, prev, pos + 1);
    solve(ans, A, tprev, pos + 1);
}
vector<vector<int>> Solution::subsets(vector<int> &A)
{
    vector<vector<int>> ans;
    ans.push_back(vector<int>());
    sort(A.begin(), A.end());
    solve(ans, A, vector<int>(), 0);
    return ans;
}
