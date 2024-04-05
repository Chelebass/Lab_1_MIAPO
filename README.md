# Lab_1_MIAPO
using System;

namespace MyNamespace
{
    public class main
    {
        static void Main()
        {
            int count = 0;
            while (true)
            {
                Console.Clear();
                int a = findPashaGender();
                count++;
                if (a == 52)
                {
                    Console.WriteLine(count);
                    return;
                }
            }
        }
        public static int findPashaGender()
        {
            Random rnd = new Random();
            Console.WriteLine("Паша?");
            int rndRes = rnd.Next(0, 100);
            

            if (rndRes > 50)
            {
                Console.WriteLine(rndRes);
                Console.WriteLine("Да, паша");
            }
            else
            {
                Console.WriteLine(rndRes);
                Console.WriteLine("Нет, не паша");
            }

            return rndRes;
        }
    }
}

