# Week8IDReader

## CVVVvalidation
```
 class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Good Morning!");
            Console.WriteLine("Please enter your CVV infromation.");
            string UsersCVV = Console.ReadLine();
            if(Validate(UsersCVV))
            {

            }
        }
        public static bool Validate(string input)
        {
            if(input.Length == 3)
            {
                try
                {
                    long.Parse(input);
                    Console.WriteLine("Thank you for you CVV.");
                    return true;
                }
                catch(Exception error)
                {
                    Console.WriteLine(error);
                    return false;
                }  
            }
            else
            {
                Console.WriteLine("Can you not be stupid.");
                return false;
            }
        }
    }
    
    ```
