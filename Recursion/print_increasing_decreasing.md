https://nados.io/question/print-increasing-decreasing?zen=true

```
    public static void main(String[] args) throws Exception {
        // write your code here
        Scanner scn = new Scanner(System.in);
        int n = scn.nextInt();
        pdi(n);
    }

    public static void pdi(int n){

        //base case
        if(n==0){
            return;
        }else{
            
        System.out.println(n);
        pdi(n-1);
        System.out.println(n);

        }
        
    }
```    
    ![image](https://user-images.githubusercontent.com/53649320/154636372-132a9ecf-abb3-4203-b041-f88ae4c8adec.png)

