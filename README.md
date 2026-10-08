Jag har utgått från en lärares exempel kod och gjort några ändringar för att testa olika exceptions.

Ändringar:
Lade till en kontroll för division med 0 och kastar DivideByZeroException.
Kommenterade bort den generella catch (Exception) i ProcessFile så att specifika exceptions kan skickas vidare till Main.
Behöll finally för att säkerställa att StreamReader stängs.
Testade exceptions

Jag har testat:

FileNotFoundException – genom att ta bort/döpa om numbers.txt.
FormatException – genom att skriva hej i filen.
DivideByZeroException – genom att skriva 0 i filen.
Exception – genom att testa en tom fil och en felaktig sökväg.
Normalt flöde – genom att skriva 10 i filen.

Allt fungerade som förväntat.
