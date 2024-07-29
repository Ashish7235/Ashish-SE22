import java.util.Scanner;
public class complex {
        int real1;
        int real2;
        int img1;
        int img2;
        complex()
        {
                System.out.println("Addition of two complex numumbers:");
        }
        complex(int r1,int r2,int i1,int i2)
        {
                this.real1=r1;
                this.real2=r2;
                this.img1=i1;
                this.img2=i2;
        }
     void accept()
     {
             Scanner sc=new Scanner(System.in);
             System.out.println("Enter real part 1:");
             this.real1=sc.nextInt();
             System.out.println("Enter real part 2:");
             this.real2=sc.nextInt();
             System.out.println("Enter img part 1:");
             this.img1=sc.nextInt();
             System.out.println("Enter img part 2:");
             this.img2=sc.nextInt();
     }
     void display()
     {
             int sum=this.real1+this.real2;
             System.out.println("sum of two complex no is:"+(sum)+"+"+(this.img1+this.img2)+"i");
             int sub=this.real1-this.real2;
             System.out.println("sum of two complex no is:"+(sub)+"+"+(this.img1-this.img2)+"i");
             int mul=this.real1*this.real2;
             System.out.println("sum of two complex no is:"+(mul)+"+"+(this.img1*this.img2)+"i");
             int div=this.real1/this.real2;
             System.out.println("sum of two complex no is:"+(div)+"+"+(this.img1/this.img2)+"i");
     }
        public static void main(String[] args) {
                complex c = new complex();
                c.accept();
                c.display();                
        }

}