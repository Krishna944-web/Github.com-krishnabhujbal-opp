# Github.com-krishnabhujbal-opp
import java.util.Scanner; 
abstract class Shape 
{ 
double l, h; 
abstract void get_data(); 
abstract void compute_area(); 
} 
class triangle extends Shape 
{ 
void get_data() 
{ 
Scanner sc = new Scanner(System.in); 
System.out.print("Enter the base of triangle : "); 
l = sc.nextDouble(); 
 
System.out.print("Enter the Height of triangle : "); 
h = sc.nextDouble(); 
} 
 
void compute_area() 
{ 
double area; 
area = (l*h)/2; 
System.out.print("Area of the trangle is "+area); 
} 
} 
class rectangle extends Shape 
{ 
void get_data() 
{ 
Scanner sc = new Scanner(System.in); 
System.out.print("\nEnter the Length of rectangle : "); 
l = sc.nextDouble(); 
 
System.out.print("Enter the Height of rectangle : "); 
h = sc.nextDouble(); 
} 
 
void compute_area() 
{ 
double area; 
area = l*h; 
System.out.print("Area of the rectangle is "+area); 
}
} 
class shape1 
{ 
public static void main(String args[]) 
{ 
triangle t = new triangle(); 
t.get_data(); 
t.compute_area(); 
 
rectangle r = new rectangle(); 
r.get_data(); 
r.compute_area(); 
} 
}
