# NotesBin
Quick Reference sheet for notes and discussion for class.
 class Program
    { 
        static void Main(string[] args)
        {
            
            int n = 100;// <-- Ignore passed by solution
            for (int i = 1; i <= n; i++)
            {
                if (n % 2 == 0 && n % 3 == 0)
                {
                    Console.WriteLine(" Codility Test ");
                }
                else if (n % 3 == 0 && n % 5 == 0)
                {
                    Console.WriteLine("Test Coders");
                }
                else if (n % 2 == 0 && n % 5 == 0)
                {
                    Console.WriteLine("Codility Coders");
                }
                else if (n % 2 == 0 && n % 3 == 0 && n % 5 == 0)
                {
                    Console.WriteLine("Codility Test Coders");
                }
                else if (n % 2 == 0)
                {
                    Console.WriteLine("Codility");
                }
                else if (n % 3 == 0)
                {
                    Console.WriteLine("Test");
                }
                else if (n % 5 == 0)
                {
                    Console.WriteLine("Coders");
                }
                else
                {
                    Console.WriteLine(n);
                }

            }

            Console.ReadLine();
        }
    }















 class Program
    {
        static void Main(string[] args)
        {
            int r = Solution.solution(100003, 6230002);
            Console.WriteLine(r);
            Console.ReadLine();
        }
    }

    class Solution
    {
        public static int solution(int A, int B)
        {
            if (A < 0 || A > 100000000) return -1;
            if (B < 0 || B > 100000000) return -1;

            //List of all variables This is the chars array
            char[] firstNumberChars = getChars(A);
            char[] secondNumberChars = getChars(B);

            //Length for comparison 
            int firstNumberLength = firstNumberChars.Length;
            int secondNumberLength = secondNumberChars.Length;

            // utilizes math class to make it easier for you to do comparison
            int highestLength = Math.Max(firstNumberLength, secondNumberLength);

            // If math class not in the code the following code solves that double check the Greater than and less than
            // Greater number get set to the HigestLength
            //if (firstNumberLength < secondNumberLength)
            //{
            //    highestLength = secondNumberLength;
            //}
            //else if (secondNumberLength < firstNumberLength)
            //{
            //    highestLength = firstNumberLength;
            //}
            //else
            //{
            //    highestLength = firstNumberLength;
            //}

            StringBuilder decimalZip = new StringBuilder();

            //does the loop to zipp up the values
            for (int i = 0; i < highestLength; i++)
            {
                if (i < firstNumberLength) decimalZip.Append(firstNumberChars[i]);

                if (i < secondNumberLength) decimalZip.Append(secondNumberChars[i]);
            }

            int maxValue = 100000000;

            Int64 answer = Int64.Parse(decimalZip.ToString());

            if (answer > maxValue)
                return -1;
            return Int32.Parse(decimalZip.ToString());
        }
        private static char[] getChars(int n)
        {
            return n.ToString().ToCharArray();
        }
    }











class Class1
    {
        public int Solution(int S)
        {
            if (S.ToString().Length == 0) return -1; //returns -1 if size is 0

            //foreach (char n in S)
            //{
            //    if ()
            //    {
            //        Console.WriteLine(" ");
            //    }
            //    else if ()
            //    {
            //        Console.WriteLine(" ");
            //    }
            //    else if ()
            //    {
            //        Console.WriteLine(" ");
            //    }
            //    else if ()
            //    {
            //        Console.WriteLine(" ");
            //    }
            //    else
            //    {
            //        Console.WriteLine(" ");
            //    }
            //    Console.ReadLine();
            //}

            return 0;
        }
    }
