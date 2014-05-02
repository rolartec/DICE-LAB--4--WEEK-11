DICE-LAB--4--WEEK-11
====================

"DICE"  LAB # 4 WEEK 11

//  BY REINA OLARTE

//  "DICE"  LAB #4  WEEK  11
public class Dice 
{
	static int CompNumber;
	
	// VARIABLES:
	
	int ADDNumbers;
	
	int GENNumber;
	
	int NUMBbounces;
	
	int AVENumber;
	
	int i=1;
		static int oneThrow()
		{
			int compNumber;
			
			CompNumber = (1	 + (int)(Math.random() * 6));
			
			CompNumber = CompNumber;


			return CompNumber;
		}
		public Dice(int bounces)
		{
			while(i <= bounces)
			{
				ADDNumbers += Throw();
				i++;
			}
			CompNumber = ADDNumbers / bounces;		
		}
		public int Throw()
		{
			CompNumber = (1	 + (int)(Math.random() * 6));
				//System.out.printf("The number that the computer generated was %d\n", computerNumber);
				return CompNumber;
		}
		public int Throw(int bounces)
		{

			NUMBbounces = bounces;
			
			while(i <= bounces)
			{
				GENNumber = (1+(int)(Math.random() *6));
				
				System.out.printf(""
						+ " Generated number is: %d\n", GENNumber);
				ADDNumbers += GENNumber;
				
				System.out.printf("The Sum of the Number: %d\n\n", ADDNumbers);
				
				i++;
			}
			CompNumber = ADDNumbers / NUMBbounces;
			
			return CompNumber;
		}
		public int Value()
		{
			return CompNumber;
		}
}
