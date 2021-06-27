# Exception-handling
using System;

namespace ExceptionHandling
{
    class Program
    {
        static void Main(string[] args)
        {
            try
            {
                Console.WriteLine("Enter the First Number:");
                int i = int.Parse(Console.ReadLine());
                Console.WriteLine("Enter the Second Number:");
                int j = int.Parse(Console.ReadLine());
                int k = i / j; Console.WriteLine("The value is:" + k);
            }
            catch(FormatException ex1)
            {
                Console.WriteLine(ex1.Message);
            }
            catch (DivideByZeroException ex2) { Console.WriteLine(ex2.Message); }
            catch (Exception ex) { Console.WriteLine(ex.Message); }
           
            Console.WriteLine("End of the program");

        }
    }
}
