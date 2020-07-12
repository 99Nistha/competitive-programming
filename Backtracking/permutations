void helper (vector<int> &A, int i, int j, vector<vector<int> > &out, int n) {
// base case
if (i == n) {
    out.push_back(A);
    return;
}

for (int j = i; j < n; j++) {
    swap (A[i], A[j]);
    helper (A, i + 1, j + 1, out, n);
    swap (A[i], A[j]);
}

return;
}

vector<vector<int> > Solution::permute(vector<int> &A) {
    vector<vector<int> > out;
    helper (A, 0, 0, out, A.size());
    return out;
}
