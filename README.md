[1,2,3]
//[4,5,6]
//[7,8,9]
let arr = [[1,2,3],[4,5,6],[7,8,9]];
let n = arr.length;
let result = "";
//(2,0),(1,0),(0,0)
for(i=n-1;i>=0;i--){
    result = result+arr[i][0];
}
//(0,1),(0,2)
for(i=1;i<n;i++){
    result = result+arr[0][i];
}
//(1,2),(2,2)
for(i=1;i<n;i++){
    result=result+arr[i][n-1];
}
for(i=n-1;i<=n-1;i++){
    result=result+arr[i][n-2];
}
console.log(result);
