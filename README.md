# printing-Arrays-values-in-Reverses
printing Arrays  values  in Reverses
public class GF {
    static void reverseArrays(int arr[],int start,int end){
        int temp;
        while (start<end){
              temp=arr[start];
              arr[start]=arr[end];
              arr[end]=temp;
              start++;
              end--;

        }
    }
        static void printArray(int arr[],int size) {
            for (int i = 0; i < size; i++)
                System.out.print(arr[i] + " ");

                System.out.println();
            }



    public static void main(String[] args) {
        int arr[]={10,20,30,40,50,60,70,80};
        printArray(arr,8);
        reverseArrays(arr,0,7);
        System.out.print("Reverse value of Arrays :\n");
        printArray(arr,8);
    }
}
