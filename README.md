# Sequence-equation in cpp
#include <bits/stdc++.h>

using namespace std;
int main()
{

    int n,i,j;
    cin >> n;
    int arr[n],temp;


    

    for (int i = 0; i < n; i++) {
        cin >> arr[i];
    }

    vector<int> result;

    for (i = 0; i <n; i++) {
        for(j=0;j<n;j++)
        {
            if(arr[j]==i+1)
            {
                temp=j+1;
                break;
            }

        }
        for(j=0;j<n;j++)
        {
            if(arr[j]==temp){
                result.push_back(j+1);
                break;
            }
        }

    }
    for(i=0;i<n;i++)
    {
        cout<<result[i]<<endl;
    }
}

    
