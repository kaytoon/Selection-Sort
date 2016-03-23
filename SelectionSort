/**
* Author: Mohamed Dahir
* This is a insertion sorting algortihm
**/
using System;

namespace SelectionSort
{
	class MainClass
	{
		static int[] array;
		public static void Main (string[] args)
		{
			//console out instructions for the user.
			Console.WriteLine("please input the size of your array and press ENTER");

			//b stores the user input as an integer
			int b = Convert.ToInt32(Console.ReadLine ());

			//the user input b, is used to initialize as the size of the array.
				array = new int[b];

			//Used for generating random integers for the array.
				Random ran = new Random();

			//assigns each index of the array a random integer
				for(int i = 0; i<array.Length;i++){
				array [i] = ran.Next(0,101);
				}
			//console outputs the original array for visual.
			Console.WriteLine("This is the original array That was generated");
			for(int i = 0; i<array.Length;i++){

				Console.Write(array[i]+" ");
			}
			Console.WriteLine(" ");
			//a method call to sort the array.
			sort();

			//console out put of the sorted array.
			Console.WriteLine("This is the sorted array");
			for(int i = 0; i<array.Length;i++){

				Console.Write(array[i]+" ");
			}
		}
		/**
		* This method does the insertion sorting algortihm. 
		* it picks an index and figures it out where it belongs in 
		* the array by doing n comparison. 
		**/
		private static void sort() {
			for(int i=0;i<array.Length;i++){
				int firstIndex = array[i];
				for(int k=i+1;k<array.Length;k++){
					if(firstIndex > array[k]){
						firstIndex = array[k];
						swap(i,k);
					}
				}

			}

		}
		/**
		* This method takes two integer parameters.
		* The two integers represent index in an array that needs
		* to be swapped.
		**/
		private static void swap(int i, int k) {
			int temp = array[i];
			array[i] = array[k];
			array[k] = temp;

		}
	}
}

