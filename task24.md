using System; 

namespace SimpleDllTest 
{
    public class MySimpleLibrary
    {
    
        public void SayHello()
        {
            Console.WriteLine("Привет! Я void-метод 1.");
        }
        public void SayBye()
        {
            Console.WriteLine("Пока! Я void-метод 2.");
        }
        public int AddTwoNumbers(int x, int y)
        {
            return x + y;
        }
        public string MakeName(string first)
        {
            return "Имя: " + first;
        }
        public double Multiply(double a, double b)
        {
            return a * b;
        }
    }
    class Program
    {
        static void Main(string[] args)
        {
            MySimpleLibrary lib = new MySimpleLibrary();

            lib.SayHello();
            lib.SayBye();
            int sum = lib.AddTwoNumbers(4, 6);
            Console.WriteLine("Сумма: " + sum);  

            string name = lib.MakeName("Вася");
            Console.WriteLine(name);  

            double product = lib.Multiply(2.5, 3);
            Console.WriteLine("Произведение: " + product);  

            Console.ReadLine();  
        }
    }
}
