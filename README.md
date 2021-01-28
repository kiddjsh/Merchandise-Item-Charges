# Merchandise-Item-Charges
An application, using a solution algorithm that uses logical and relational expressions, that determines the total purchases and sales tax of merchandise purchased. The application prompts for the name of the purchaser, the item being purchased, and  the price of the item, then determines the subtotal, the sales tax, and the total purchase amount.

# Variables & IPO Model
![Variables & IPO Model](https://raw.githubusercontent.com/kiddjsh/Merchandise-Item-Charges/main/images/Items_Variable%20%26%20IPO%20Model.PNG)

# My C# Solution
```C#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ExcerciseW2
{
    class Program
    {
        static void Main(string[] args)
        {
            //variable declaration
            string customer = "josh";
            double itemPrice1 = 0;
            double itemPrice2 = 0;
            double itemPrice3 = 0;
            double itemPrice4 = 0;
            double totalSales = 0;
            double subTotal = 0;
            double totalPurchase = 0;
            const double salesTax = .07;


            //output greeting
            Console.ForegroundColor = ConsoleColor.Green;
            Console.WriteLine("Hi! Welcome to the Online Antique Shop.");
            Console.ForegroundColor = ConsoleColor.Green;

            //input inputs from the user
            customer = Console.ReadLine();
            Console.Write("Please enter the name of purchase: ");
            customer = Console.ReadLine();
            Console.Write("You will be asked to enter your Items Purchased and Price. Thank You!");
            customer = Console.ReadLine();
            Console.Write("_____________________________________________________");
            customer = Console.ReadLine();
            Console.ForegroundColor = ConsoleColor.Green;

            //enter the items purchases & sales amount
            customer = Console.ReadLine();
            Console.Write("---------Item 1---------");
            customer = Console.ReadLine();
            Console.Write("Enter Item Purchased: ");
            customer = Console.ReadLine();
            Console.Write("Enter Item Price: $");
            itemPrice1 = Convert.ToDouble(Console.ReadLine());
            totalSales = totalSales + itemPrice1;
            customer = Console.ReadLine();
            Console.Write("---------Item 2---------");
            customer = Console.ReadLine();
            Console.Write("Enter Item Purchased: ");
            customer = Console.ReadLine();
            Console.Write("Enter Item Price: $");
            itemPrice2 = Convert.ToDouble(Console.ReadLine());
            totalSales = totalSales + itemPrice2;
            customer = Console.ReadLine();
            Console.Write("---------Item 3---------");
            customer = Console.ReadLine();
            Console.Write("Enter Item Purchased: ");
            customer = Console.ReadLine();
            Console.Write("Enter Item Price: $");
            itemPrice3 = Convert.ToDouble(Console.ReadLine());
            totalSales = totalSales + itemPrice3;
            customer = Console.ReadLine();
            Console.Write("---------Item 4---------");
            customer = Console.ReadLine();
            Console.Write("Enter Item Purchased: ");
            customer = Console.ReadLine();
            Console.Write("Enter Item Price: $");
            itemPrice4 = Convert.ToDouble(Console.ReadLine());
            totalSales = totalSales + itemPrice4;
            customer = Console.ReadLine();
            Console.ForegroundColor = ConsoleColor.Green;

            //do calculations
            totalSales = itemPrice1 + itemPrice2 + itemPrice3 + itemPrice4;
            subTotal = totalSales * salesTax;
            totalPurchase = totalSales + subTotal;
            Console.ForegroundColor = ConsoleColor.Green;

            //output outputs
            Console.Write("_______________________________________________________________________");
            customer = Console.ReadLine();
            Console.Write("Sub Total: $" + totalSales);
            customer = Console.ReadLine();
            Console.Write("Sales Tax @ 7%: $" + subTotal);
            customer = Console.ReadLine();
            Console.Write("Total Purchase: $" + totalPurchase);
            customer = Console.ReadLine();
            Console.Write("_______________________________________________________________________");
            customer = Console.ReadLine();
            Console.Write("Thank you for shopping at the Online Antique Shop.");
            customer = Console.ReadLine();
            Console.ReadLine();  //keep window open
        }
    }
}
```

# Complete Working Program
![Complete Working Program](https://raw.githubusercontent.com/kiddjsh/Merchandise-Item-Charges/main/images/Items_Complete%20Working%20Program.PNG)

# Desk Check
![Desk Check](https://raw.githubusercontent.com/kiddjsh/Merchandise-Item-Charges/main/images/Items_Desk%20Check.PNG)
