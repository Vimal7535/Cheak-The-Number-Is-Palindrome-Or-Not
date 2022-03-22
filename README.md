# Cheak-The-Number-Is-Palindrome-Or-Not


using System;

namespace Cheak_Number_Is_Palindrome

{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Cheak the Number is Palindrome or Not\n");
            int rem;
            int result = 0;
            int temp;
            Console.WriteLine("Enter a Number");
            int num = int.Parse(Console.ReadLine());
            temp = num;
            while (num != 0)
            {
                rem = num % 10;
                num = num / 10;
                result = result * 10 + rem;
            }
            if (temp == result)
            {
                Console.WriteLine("Number is Palindrome...");
            }
            else
            {
                Console.WriteLine("Number is Not Palindrome...");
            }
           
        
        }
    }
}
