import java.util.Scanner;

public class MaxToys {
    public static int getMaxToys(int prices[],int money) {
        int sum=0;
        int count=0;
        int max=0;
        for(int i=0;i<prices.length;i++) {
            sum=count=0;
            for(int j=i;j<prices.length;j++) {
                if((sum+prices[j])<=money){
                    sum=sum+prices[j];
                    count=count+1;
                    max=Math.max(count,max);
                }
                else
                {
                  count=0;
                  sum=0;
                  break;
                }
            }
        }
        return max;
    }
    public static void main(String[] args) {
        Scanner sc1=new Scanner(System.in);
        Scanner sc2=new Scanner(System.in);
        Scanner sc3=new Scanner(System.in);
        System.out.println("Enter a Number");
        int n = sc1.nextInt();
        int prices[]=new int[n];
        for(int i=0;i<n;i++) {
          prices[i]=sc2.nextInt();
        }
        System.out.println("Enter money");
        int money = sc3.nextInt();
    System.out.println(getMaxToys(prices,money));
    }
}
