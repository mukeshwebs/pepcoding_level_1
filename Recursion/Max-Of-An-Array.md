https://nados.io/question/max-of-an-array?zen=true

![image](https://user-images.githubusercontent.com/53649320/155653328-9d6e03f0-dbc0-4185-b50d-845ccaf68692.png)


```

public class Main {

    public static void main(String[] args) throws Exception {
        // write your code here
      Scanner scn = new Scanner(System.in);
      int n = scn.nextInt();
      int[] arr = new int[n];

      for (int i = 0; i < n; i++) {
         arr[i] = scn.nextInt();

      }
         int max =  maxOfArray(arr, 0);
         System.out.println(max);

    }

    public static int maxOfArray(int[] arr, int idx){

        //base case
        if(idx==arr.length){
            return 0;
        }

        //recursive case
        int max_in_smaller = maxOfArray(arr, idx+1);    //faith

        //compare with the idx element
        if(arr[idx]>max_in_smaller){
            return arr[idx];
        }else

        return max_in_smaller;
    }

}
```
