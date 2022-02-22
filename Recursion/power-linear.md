https://nados.io/question/power-linear?zen=true


```
public class Main {

  public static void main(String[] args) throws Exception {
    Scanner scn = new Scanner(System.in);
    int x = scn.nextInt();
    int n = scn.nextInt();
    int p = power(x, n);
    System.out.println(p);
  }

  public static int power(int x, int n) {
    if(n == 0){
      return 1;
    }
    int x_power = x*power(x, n - 1);
    return x_power;
  }

}
```

Logic-

![image](https://user-images.githubusercontent.com/53649320/155152244-ad1a4b70-e35c-4a2a-83f3-b1d9f7165e37.png)
