C# Program to Print a Binary Triangle
using System;<br>
namespace Exercises<br>
{
    class BinaryTriangle
    {
        static void Main(string[] args)
        {
            int number, digit = 1;
            Console.Write("\nEnter the number of lines:\n ");
            number = Convert.ToInt32(Console.ReadLine());
            for (int i = 1; i <= number; i++)
            {
                for (int space = number - i; space > 0; space--)
                {
                    Console.Write(" ");
                }
                for (int j = 0; j < i; j++)
                {
                    Console.Write(digit + " ");
                    digit = (digit == 1) ? 0 : 1;
                }
                Console.Write("\n");
            }
        }
    }
}
![Screenshot 2022-01-21 065121](https://user-images.githubusercontent.com/98145297/150480363-f56d5081-6686-4ae9-b130-f55b78ec572b.png)
