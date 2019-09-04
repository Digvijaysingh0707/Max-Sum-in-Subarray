# Max-Sum-in-Subarray
package com.company;

public class Main {

    public static void main(String[] args) {
int a[]={1,5,9,9,5,22};
int n = a.length;
int max=Integer.MIN_VALUE;
for(int i =0;i<n;i++){
    for(int j =i;j<n;j++){
        int curSum=0;
        for(int k=i;k<=j;k++){
            curSum+=a[i];
        }
        if(curSum>max){
            max=curSum;
        }
    }
        }
        System.out.println(max);
    }
}
