C# Program to Print a Binary Triangle
using System;<br>
namespace Exercises<br>
{<br>
    class BinaryTriangle<br>
    {<br>
        static void Main(string[] args)<br><
        {<br>
            int number, digit = 1;<br>
            Console.Write("\nEnter the number of lines:\n ");<br>
            number = Convert.ToInt32(Console.ReadLine());<br>
            for (int i = 1; i <= number; i++)<br>
            {<br>
                for (int space = number - i; space > 0; space--)<br>
                {<br>
                    Console.Write(" ");<br>
              
                for (int j = 0; j < i; j++)<br>
                {<br>
                    Console.Write(digit + " ");<br>
                    digit = (digit == 1) ? 0 : 1;<br>
                }<br>
                Console.Write("\n");<br>
            }<br>
        }<br>
    }<br>
}<br>
![Screenshot 2022-01-21 065121](https://user-images.githubusercontent.com/98145297/150480363-f56d5081-6686-4ae9-b130-f55b78ec572b.png)
