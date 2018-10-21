# BondU1.Ch.2.1.2ArraysTasks
BondU1.Ch.2.1.2 Arrays Tasks 01 - 11
echo "# BondU1.Ch.2.1.2ArraysTasks" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/johnburnham/BondU1.Ch.2.1.2ArraysTasks.git
git push -u origin master
//================================================================================================
// Bond U1; Ch. 2.1.2 p.204; Task 03; Enter Six values into an Array and then display the values.
// John Fones; 181020;
//================================================================================================
using System;

namespace Ch2_1_2_P204_Task03
{
    class Program
    {
        static void Main(string[] args)
        {
            int[] SixValues = new int[6];

            for (int i = 0; i < 6; i++)
            {
                Console.WriteLine("Please enter an integer value.");
                SixValues[i] = System.Convert.ToInt32(Console.ReadLine());
                Console.WriteLine("You have just entered {0} as value No.{1}.", SixValues[i], i+1);
            }
            Console.Write("Your six values are: ");
            for (int i = 0; i < 5; i++)
            {
                Console.Write("{0}, ", SixValues[i]);
            }
            Console.Write("and {0}.", SixValues[5]);
            Console.ReadLine();
        }
    }
}
