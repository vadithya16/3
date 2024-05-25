3a:
class Parent
{
int x;
Parent(int a)
{
x=a;
}
void displayx()
{
System.out.println("\n Value of i : " +x);
}
}
class Child extends Parent
{
int y;
Child(int a,int b)
{
super(a);
y=b;
}
void displayxy()
{
System.out.println("\n Value of a : " +x);
System.out.println("\n Value of b : " +y);
}
}
class Inheritance
{
public static void main(String args[])
{
Parent ob1=new Parent(10);
Child ob2=new Child(20,30);
System.out.println("\n Contents of Parent or Super Class Object : ");
ob1.displayx();
System.out.println("\n Contents of Child Class Object : ");
ob2.displayxy();
}
}

3b:
interface Shape{
void area();
} // end of interface
class Rectangle implements Shape{
double l,b;
Rectangle(double length, double breadth){
l=length;
b=breadth;
}
public void area(){
System.out.println("Area of Rectangle is : " + l*b);
}
}
class Triangle implements Shape{
double b,h;
Triangle (double base, double height){
b= base;
h= height;
}
public void area(){
System.out.println("Area of Triangle is : " + (b*h/2));
}
}
public class InterfaceDemo {
public static void main(String args[]){
Rectangle rect=new Rectangle(10,05);
rect.area();
Triangle tri=new Triangle(10,20);
tri.area();
}// end of main
} //end of InterfaceDemo
