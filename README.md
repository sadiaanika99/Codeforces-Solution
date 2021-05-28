 Codeforces-solution 758A:Holiday of equality
#include <iostream>

using namespace std;

int main()

{
    int n,arr[100],i,j=0,k=0;
    cin>>n;
    for(i=0;i<n;i++)
    {
        cin>>arr[i];
        j=max(arr[i],j);
    }
    for(int i=0;i<n;i++)
    {
        k=k+j-arr[i];
    }

    cout <<k<< endl;
    return 0;
}
