using System;

public class ObjectPlacement
{
    public static void Main()
    {
        // Генерация случайных координат объектов
        Random rnd = new Random();
        int numObjects = 5; // Количество объектов
        int[,] objects = new int[numObjects, 2]; // Массив объектов и их координат

        for (int i = 0; i < numObjects; i++)
        {
            // Генерируем случайные координаты объектов в пределах плоскости
            objects[i, 0] = rnd.Next(0, 100); // x-координата
            objects[i, 1] = rnd.Next(0, 100); // y-координата
            
            Console.WriteLine($"Object {i+1} at ({objects[i, 0]}, {objects[i, 1]})");
        }

        // Здесь можно добавить алгоритм оптимизации для минимизации конфликтов или расстояния между объектами
        
    }
}
