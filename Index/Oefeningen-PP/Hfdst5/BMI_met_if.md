# Oplossing 1

```csharp
            Console.Write("Gewicht (kg): ");
            double gewicht = double.Parse(Console.ReadLine());

            Console.Write("Lengte (m): ");
            double lengte = double.Parse(Console.ReadLine());

            double BMI = Math.Round(gewicht / (Math.Pow(lengte, 2)), 2);

            Console.WriteLine($"Je BMI is {BMI}");

            if (BMI < 18.5)
            {
                Console.ForegroundColor = ConsoleColor.Red;
                Console.WriteLine("Ondergewicht");
                Console.ResetColor();
            }

            else if (18.5 <= BMI && BMI <= 24.9)
            {
                Console.ForegroundColor = ConsoleColor.Green;
                Console.WriteLine("Normaal gewicht");
                Console.ResetColor();
            }

            else if (25 <= BMI && BMI <= 29.9)
            {
                Console.ForegroundColor = ConsoleColor.DarkYellow;
                Console.WriteLine("Overgewicht, je loopt niet echt een risico, maar je mag niet dikker worden.");
                Console.ResetColor();
            }

            else if (30 <= BMI && BMI <= 39.9)
            {
                Console.ForegroundColor = ConsoleColor.Red;
                Console.WriteLine(" Zwaarlijvigheid (obesitas). Verhoogde kans op allerlei aandoeningen zoals diabetes,\r\n hartaandoeningen en rugklachten. Je zou 5 tot 10 kg moeten vermageren.");
                Console.ResetColor();
            }

            else if (40 <= BMI)
            {
                Console.ForegroundColor = ConsoleColor.Magenta;
                Console.WriteLine("Ernstige zwaarlijvigheid. Je moet dringend vermageren want je gezondheid is in gevaar \r\n (of je hebt je lengte of gewicht in verkeerde eenheid ingevoerd).");
                Console.ResetColor();
            }

            else {
                Console.WriteLine("Rust in vrede.");
            }
```

[Terug](../Hfdst5.md)