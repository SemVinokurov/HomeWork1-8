//Задача 1.
/*
Console.Write("Input a first number: ");
int n1 = Convert.ToInt32(Console.ReadLine());
Console.Write("Input a second number: ");
int n2 = Convert.ToInt32(Console.ReadLine());
if(n1 > n2)
{
    Console.WriteLine($"Maximum number: {n1}, Minimum number: {n2}");
}
else
{
    Console.WriteLine($"Maximum number: {n2}, Minimum number: {n1}");
}
*/

//Задача 2.
/*
Console.Write("Input a first number: ");
int n1 = Convert.ToInt32(Console.ReadLine());
Console.Write("Input a second number: ");
int n2 = Convert.ToInt32(Console.ReadLine());
Console.Write("Input a third number: ");
int n3 = Convert.ToInt32(Console.ReadLine());
if(n1 > n2)
  if(n1>n3)
  {
   Console.WriteLine($"Maximum number: {n1}");
  }
  else
  {
    Console.WriteLine($"Maximum is number: {n3}");
  }
else
 if(n2 > n3)
 {
    Console.WriteLine($"Maximum is number: {n2}");
 }
 else
 {
    Console.WriteLine($"Maximum is number: {n3}");
 }
*/
//Задача 3
/*
Console.Write("Input a number: ");
int n1 = Convert.ToInt32(Console.ReadLine());
if(n1 % 2 == 0)
{
    Console.WriteLine($"Even number: {n1}");
}
else
{
    Console.WriteLine("No!");
}
*/
//Задача 4.
/*Console.Write("Input a number: ");
int n = Convert.ToInt32(Console.ReadLine());
int current = 2;

while (current <= n)
{
    Console.Write(current + " ");
    current += 2;
}
*/
//Домашнее Задание №2;
//Задача 1;
/*
int Cnumber(int number)
{
    number = number % 100 /10;
    return number;
}
int num = new Random().Next(100, 1000);
int result = Cnumber(num);
Console.WriteLine($"New version of a number {num} is {result}");
*/
//Задача 2;
/*
int Thirdnumber(int number)
{
    int a = number / 100;
    if (a > 0)
    {
       if (number > 999) 
       {
        if (number >9999)
        {
            number = number%1000/100;
            return number;
        }
        else
        {
           number = number%100/10;
           return number;
        }
       }
       else
       {
        number = number%10;
        return number;
       }
       
    }
    else
    {
        number = -1;
        return number;
    }
}
Console.WriteLine("Input a number: ");
int n1 = Convert.ToInt32(Console.ReadLine());
int result = Thirdnumber(n1);
if(n1>0)
{
    Console.WriteLine($"Third number of a number {n1} is {result}");
}
else
{
    Console.WriteLine("Wrong number");
}

*/
//Задача 3.
/*
bool Relax(int a)
{
  if(a < 6)
  { 
    return false;
   }
 else
{
return true;
}
}
Console.WriteLine("Input a day of the week (1-7): ");
int n1 = Convert.ToInt32(Console.ReadLine());
bool result = Relax(n1);
Console.WriteLine(result);
*/


//Семинар 4 
//Задача 25.
/*
int Exponent(int number1, int number2)
{
  int product = 1;
  for(int current =1; current<=number2; current++)
      product=product*number1;
  return product;

}
Console.Write("Input a number 1: ");
int n1 = Convert.ToInt32(Console.ReadLine());
Console.Write("Input a number 2: ");
int n2 = Convert.ToInt32(Console.ReadLine());
Console.WriteLine($"Product of exponentiation number {n1} in {n2} is {Exponent(n1, n2)}");
*/
//Задача 27
/*
int SumNum(int n)
{
    int sum = 0;
    while(n>0)
    {
        int des = n%10;
        sum = sum + des;
        n = n / 10;
    }
    return sum;
}

Console.Write("Input a number: ");
int n1 = Convert.ToInt32(Console.ReadLine());

Console.WriteLine($"Sum numbers of gidits {n1} is {SumNum(n1)} ");
*/

//Задача 29
/*
Console.WriteLine("Будет создан массив длиной A в диапвзоне 0-A");
 Console.Write("Введите любое число (A): ");
 int enterNumber = Convert.ToInt32(Console.ReadLine());
 int[] array = new int [enterNumber];

for (int i = 0; i<enterNumber; i++)
{
    array [i]=new Random().Next(enterNumber);
    Console.Write(array[i]+"; ");
}
Console.WriteLine();
*/
//Задача 34
/*
Console.WriteLine("Введите размер массива");
int size = Convert.ToInt32(Console.ReadLine());
int[] numbers = new int[size];
FillArrayRandomNumbers(numbers);
Console.WriteLine("Вот наш массив: ");
PrintArray(numbers);
int count = 0;

for (int z = 0; z < numbers.Length; z++)
if (numbers[z] % 2 == 0)
count++;

Console.WriteLine($"всего {numbers.Length} чисел, {count} из них чётные");

void FillArrayRandomNumbers(int[] numbers)
{
    for(int i = 0; i < numbers.Length; i++)
    {
        numbers[i] = new Random().Next(100,1000);
    }
}
void PrintArray(int[] numbers)
{
    Console.Write("[ ");
    for(int i = 0; i < numbers.Length; i++)
    {
        Console.Write(numbers[i] + " ");
    }
    Console.Write("]");
    Console.WriteLine();
}
*/
//задача 36
/*Console.WriteLine("Введите размер массива  ");
int size = Convert.ToInt32(Console.ReadLine());
int[] numbers = new int[size];
FillArrayRandomNumbers(numbers);
Console.WriteLine("массив: ");
PrintArray(numbers);
int sum = 0;

for (int z = 0; z < numbers.Length; z+=2)
    sum = sum + numbers[z];

    Console.WriteLine($"всего {numbers.Length} чисел, сумма элементов cтоящих на нечётных позициях = {sum}");

void FillArrayRandomNumbers(int[] numbers)
{
    for(int i = 0; i < numbers.Length; i++)
        {
            numbers[i] = new Random().Next(1,10);
        }
}
void PrintArray(int[] numbers)
{
    Console.Write("[ ");
    for(int i = 0; i < numbers.Length; i++)
        {
            Console.Write(numbers[i] + " ");
        }
    Console.Write("]");
    Console.WriteLine();
}
*/
//Задача 38
/*
Console.WriteLine("Введите размер массива  ");
int size = Convert.ToInt32(Console.ReadLine());
double[] numbers = new double[size];
FillArrayRandomNumbers(numbers);
Console.WriteLine("массив: ");
PrintArray(numbers);
double min = Int32.MaxValue;
double max = Int32.MinValue;

for (int z = 0; z < numbers.Length; z++)
{
    if (numbers[z] > max)
        {
            max = numbers[z];
        }
    if (numbers[z] < min)
        {
            min = numbers[z];
        }
}

Console.WriteLine($"всего {numbers.Length} чисел. Максимальное значение = {max}, минимальное значение = {min}");
Console.WriteLine($"Разница между максимальным и минимальным значением = {max - min}");

void FillArrayRandomNumbers(double[] numbers)
{
    for(int i = 0; i < numbers.Length; i++)
        {
            numbers[i] = Convert.ToDouble(new Random().Next(100,1000)) / 100;
        }
}
void PrintArray(double[] numbers)
{
    Console.Write("[ ");
    for(int i = 0; i < numbers.Length; i++)
        {
            Console.Write(numbers[i] + " ");
        }
    Console.Write("]");
    Console.WriteLine();
}
*/
//Семинар 6. Домашнее Задание.
//Задача 41.
//Пользователь вводит с клавиатуры M чисел. Посчитайте, сколько чисел больше 0 ввёл пользователь.
/*Console.Write("Введите элементы(через пробел): ");
int[] arr = Array.ConvertAll(Console.ReadLine().Split(), int.Parse);
int count = 0;
 
for (int i = 0; i < arr.Length; i++)
{
    if (arr[i] > 0)
    {
        count++;
    }
}
 
Console.WriteLine($"Кол-во элементов > 0: {count}");
*/
//Задача 43
/*Console.Write("Введите k1: ");
var k1 = Convert.ToDouble(Console.ReadLine());
Console.Write("Введите b1: ");
var b1 = Convert.ToDouble(Console.ReadLine());
Console.Write("Введите k2: ");
var k2 = Convert.ToDouble(Console.ReadLine());
Console.Write("Введите b2: ");
var b2 = Convert.ToDouble(Console.ReadLine());
 
 
var x = -(b1 - b2) / (k1 - k2);
var y = k1 * x + b1;
 
x = Math.Round(x, 3);
y = Math.Round(y, 3);
 
Console.WriteLine($"Пересечение в точке: ({x};{y})");
*/
//Задача 47. Задайте двумерный массив размером m×n, заполненный случайными вещественными числами.
/*Console.WriteLine($"Input a number of rows: ");
int m = Convert.ToInt32(Console.ReadLine());
Console.WriteLine($"Input a number of colums: ");
int n = Convert.ToInt32(Console.ReadLine());
Console.WriteLine($"Input a min number : ");
int min = Convert.ToInt32(Console.ReadLine());
Console.WriteLine($"Input a max number: ");
int max = Convert.ToInt32(Console.ReadLine());
int minValue=min;
int maxValue=max;
void FindRandomNumbers(double[,]array)
{

for(int i=0; i<array.GetLength(0); i++)
{
    for(int j=0; j<array.GetLength(1); j++)
    {
        array[i,j] = Convert.ToDouble(new Random().Next(minValue, maxValue))/10;
    }
}
}


 void Show2dArray(double[,] array)
    {
        for(int i=0; i<array.GetLength(0); i++ )
        {
            for(int j=0; j<array.GetLength(1); j++)
            {
            Console.Write(array[i,j] + " ");
            }
            
            Console.WriteLine();
        }
    }




double[,] myArray = new double[m,n];
FindRandomNumbers(myArray);
Show2dArray(myArray);
Console.WriteLine();

*/

//Задача 50. Напишите программу, которая на вход принимает позиции элемента в двумерном массиве, и возвращает значение этого элемента или же указание, что такого элемента нет.
/*
int[,] CreateRandomArray(int rows, int colums, int minValue, int maxValue)
{
    int[,]array= new int[rows, colums];
    for(int i = 0; i<rows; i++)
    {
       for(int j = 0; j<colums; j++)
       {
        array[i,j] = new Random().Next(minValue, maxValue+1);
       }
    }
    return array;
}

void Show2dArray(int[,] array)

    {
        for(int i=0; i<array.GetLength(0); i++ )
        {
            for(int j=0; j<array.GetLength(1); j++)
            {
            Console.Write(array[i,j] + " ");
            }
            
            Console.WriteLine();
        }
    }



    
    

Console.Write("Input a number of rows: ");
int m = Convert.ToInt32(Console.ReadLine());
Console.Write($"Input a number of colums: ");
int n = Convert.ToInt32(Console.ReadLine());
Console.Write($"Input a min number : ");
int min = Convert.ToInt32(Console.ReadLine());
Console.Write($"Input a max number: ");
int max = Convert.ToInt32(Console.ReadLine());


int[,] myArray = CreateRandomArray(m,n,min,max);
Show2dArray(myArray);
Console.WriteLine();

Console.WriteLine("Input a index rows: ");
int m1 = Convert.ToInt32(Console.ReadLine());
Console.WriteLine("Input a index colums: ");
int n1 = Convert.ToInt32(Console.ReadLine());

if((m1)<myArray.GetLength(0) && (n1)<myArray.GetLength(1))
    {
        Console.WriteLine($"Number: {myArray[m1-1,n1-1]}");
       
    }
    else
    {
        Console.WriteLine("Index does not exist! ");
    }
    */
//Задача 52. Задайте двумерный массив из целых чисел. Найдите среднее арифметическое элементов в каждом столбце.
/*
int[,] CreateRandomArray(int rows, int colums, int minValue, int maxValue)
{
    int[,]array= new int[rows, colums];
    for(int i = 0; i<rows; i++)
    {
       for(int j = 0; j<colums; j++)
       {
        array[i,j] = new Random().Next(minValue, maxValue+1);
       }
    }
    return array;
}

void Show2dArray(int[,] array)

    {
        for(int i=0; i<array.GetLength(0); i++ )
        {
            for(int j=0; j<array.GetLength(1); j++)
            {
            Console.Write(array[i,j] + " ");
            }
            
            Console.WriteLine();
        }
    }

Console.Write("Input a number of rows: ");
int m = Convert.ToInt32(Console.ReadLine());
Console.Write($"Input a number of colums: ");
int n = Convert.ToInt32(Console.ReadLine());
Console.Write($"Input a min number : ");
int min = Convert.ToInt32(Console.ReadLine());
Console.Write($"Input a max number: ");
int max = Convert.ToInt32(Console.ReadLine());


int[,] myArray = CreateRandomArray(m,n,min,max);
Show2dArray(myArray);
Console.WriteLine();


   
    for(int j=0; j<myArray.GetLength(1); j++)
    {
         double sum=0;
        for(int i=0; i<myArray.GetLength(0); i++)
        {
            sum+=myArray[i,j];
        }
        Console.Write(sum/myArray.GetLength(0));
    }
    Console.ReadLine();

  */
//Задача 54. Задайте двумерный массив. 
//Напишите программу, которая упорядочит по убыванию элементы каждой строки двумерного массива.

int [,] CreateRandomArray(int rows, int colums, int minValue, int maxValue)
{
    int [,] array = new int [rows, colums];
    for(int i =0; i<rows; i++)
        for(int j =0; j<colums; j++) 
        {
            array[i,j]= new Random().Next(minValue, maxValue+1);
        }
        return array;
}
void Show2dArray(int [,] array)
{
    for(int i=0; i<array.GetLength(0); i++)
        for(int j=0; j<array.GetLength(1); j++)
        {
            Console.Write(array[i,j] + " ");
            Console.WriteLine();
        }
}

Console.Write("Input a number of rows: ");
int m = Convert.ToInt32(Console.ReadLine());
Console.Write($"Input a number of colums: ");
int n = Convert.ToInt32(Console.ReadLine());
Console.Write($"Input a min number : ");
int min = Convert.ToInt32(Console.ReadLine());
Console.Write($"Input a max number: ");
int max = Convert.ToInt32(Console.ReadLine());


int[,] myArray = CreateRandomArray(m,n,min,max);
Show2dArray(myArray);
Console.WriteLine("-----------------------");

void RegulatArray(int[,] array)
{
     for(int i=0; i<array.GetLength(0); i++)
        for(int j=0; j<array.GetLength(1); j++)
            for(int k = 0; k<array.GetLength(1)-1; k++)
                if(array[i,k]<array[i,k+1])
                {
                    int temp = array[i,k];
                    array[i,k]=array[i,k+1];
                    array[i,k+1]=temp;
                }
            

        
} 

RegulatArray(myArray);
Show2dArray(myArray);
