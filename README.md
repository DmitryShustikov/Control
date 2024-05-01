
Console.Write("Введите элементы массива через пробел: ");
string[] inputArray = Console.ReadLine().Split(' ');

string[] resultArray = FilterArray(inputArray);

    
Console.WriteLine("Новый массив строк:");

Console.WriteLine(string.Join("  ", resultArray));

string[] FilterArray(string[] inputArray)

    {
       return Array.FindAll(inputArray, str => str.Length <= 3);
    }
