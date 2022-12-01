# number-is-present-

#include <iostream>
using namespace std;
bool ispresent(int arr[][3],int target , int i ,int j){
    for(int i=0;i<3;i++){
        for(int j=0;j<3;j++){
            if(arr[i][j]==target)
            return 1;
        }
    }
    return 0;
}
int main() {
    
    cout<<"enter elements of array"<<endl;
    int arr[3][3],target;
    for(int i=0;i<3;i++){
        for(int j=0;j<3;j++){
            cin>>arr[i][j];
        }
        cout<<endl;
    }
    cout<<"Array:"<<endl;
     for(int i=0;i<3;i++){
        for(int j=0;j<3;j++){
            cout<<arr[i][j]<<" ";
        }
        cout<<endl;
    }
    cout<<"enter the number ";
    cin>>target;
    
    if(ispresent(arr,target,3,3)){
        cout<<"number is present";
    }
    else{
        cout<<"number is not present";
    }
    

    return 0;
}
