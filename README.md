# Fibonacci-series-c-


using System;


    class Program
    {
        static void Main(string[] args)
        {
            int c_num = 0;
            int o_num = 1;
            int nxt_num = 0;
            Console.WriteLine("enter limit ");
            int starting = int.Parse(Console.ReadLine());

            int finsh = int.Parse(Console.ReadLine());
           
            
            while ( c_num <= finsh)
            {
                
               
                nxt_num = c_num + o_num;
                o_num = c_num;
                c_num = nxt_num;

                while (c_num >= starting && c_num <= finsh)
                {
                    Console.WriteLine(c_num);

                    nxt_num = c_num + o_num;
                    o_num = c_num;
                    c_num = nxt_num;

                }


            }
            Console.ReadLine();
        }
    }

