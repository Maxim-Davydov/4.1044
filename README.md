# 4.1044
Код программы
![изображение](https://user-images.githubusercontent.com/116034877/220600183-ddd5e6b1-600f-4438-9a3d-da6c734b85bc.png)
Скриншот выполнения программы
![изображение](https://user-images.githubusercontent.com/116034877/220600291-c92081ce-67da-4842-b287-411a7ab17739.png)

using System;
using System.Collections.Generic;
using System.IO;
using System.Linq;
using System.Net;
using System.Text;
using System.Text.RegularExpressions;
using System.Threading.Tasks;


namespace ConsoleApplication7
{
    public enum Week
    {
        Понедельник = 0,
        Вторник = 1,
        Среда = 2,
        Четверг = 3,
        Пятница = 4,
        Суббота = 5,
        Воскресенье = 6
    }
    class Program
    {
        public static void Main(string[] args)
        {
            Console.Write("Введите номер дня недели=");
            var n = int.Parse(Console.ReadLine());
            Console.WriteLine((Week)((n - 1) % Enum.GetValues(typeof(Week)).Length));
        }
    }
}
