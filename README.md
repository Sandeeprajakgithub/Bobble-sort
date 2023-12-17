class A{
    public static void main(String args[]){
        //bobble sort
        int arr[]  = {10,50,20,40,80,90};
        for(int i = 0 ; i < arr.length-1 ; i++){
            for(int j = 0 ; j < arr.length-1-i; j++){
                if(arr[j]>arr[j+1]){
                    int x = arr[j];
                    arr[j] = arr[j+1];
                    arr[j+1] = x;
                }
            }
        }
        for(int val : arr){
            System.out.print(val+" ");
        }
    }
}
