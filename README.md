# House-Builder
Just another repository
using System;
namespace _08.House_Builder
{
    class Program
    {
        static void Main(string[] args)
        {
            long firstMaterials = long.Parse(Console.ReadLine());
            long secondMaterials = long.Parse(Console.ReadLine());

            long fMaterial = 0;
            long sMaterial = 0;

            if (firstMaterials < 128)
            {
                fMaterial = firstMaterials * 4;
                sMaterial = secondMaterials * 10;
            }
            else
            {
                fMaterial = secondMaterials * 4;
                sMaterial = firstMaterials * 10;
            }

            Console.WriteLine(fMaterial + sMaterial);
        }
    }
}
