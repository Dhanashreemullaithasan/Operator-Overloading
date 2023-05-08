# Operator-Overloading

## Aim:
 To write a C# program to pass values through constructors(default and parameterized) and also overload equal operators by checking whether objects are equal using operator overloading. 
 
 ## Algorithm:
 
1. Create a class for operator overloading.

2..Get inputs for length,breadthandheight of the box fromthe user and then calculate the volume in overloading function.

3.After that return a new object for the calculated volume.

4.Then create a new object to store the return object.

5.After that print the calculated volume.
 
 ## Program:
 ```
 using System.Runtime.CompilerServices;
using System.Security.Cryptography;
using System.Security.Cryptography.X509Certificates;

class  program
{
    public program()
    {
        Console.WriteLine("Default constructor");

    }
    public program(int number)
    {
        Console.WriteLine("22");
    }
    public static bool operator == (program p1,program p2)
    {
        return p1.Equals(p2);
    }
    public static bool operator != (program p1,program p2)
    {
        return !p1.Equals(p2);
    }
}
class Example
{
    public static void Main()
    {
        program p1 = new program();
        program p2 = new program(10);
        if(p1==p2)
        {
            Console.WriteLine("objects are equal");
        }
        else
        {
            Console.WriteLine("objects are not equal");
        }
    }
}
 ```
 ## Output:
 ![ex6 c#](https://user-images.githubusercontent.com/94165415/236787566-2e969a03-2e80-4c28-9383-c6c4e53bc00c.png)

 ## Result:
 
Thus the C# program to find the volume of a box using operator overloading is implemented successfully.
