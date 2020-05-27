import java.util.Scanner;
import java.util.Random;
public class Ap {
	public static void main(String[] args)
	{
		int score=0;
		int score1=0;
		Random r=new Random();
		String ENG;
		String IND;
		String a[]= {"even","odd"};
		String Players[]= {"KL Rahul","Shikhar Dhawan","Virat Kohli"};
		String Bowlers[]= {"Ben Stokes","Stuart Broad","James Anderson"};
		String Batsman[]= {"Alastair Cook","Jos Buttler","Joe Root"};
		String Bowler[]= {"Bhuvaneshwar Kumar","Jasprith Bumrah","Ravindra Jadeja"};
		System.out.println("..........ITS TOSS TIME..........");
		System.out.println("IND Choosed Even");
		Scanner sc=new Scanner(System.in);
		int n=sc.nextInt();
		System.out.println("Number Entered by AUS for toss is:");
		int b=r.nextInt(6);
			System.out.println(b);
			int sum=n+b;
			System.out.println("sum is:"+sum);
		if(sum==2||sum==4||sum==6||sum==8||sum==10||sum==12)
		{
			System.out.println("IND Won The Toss And Choosed To Bat");
		}
		else
		{
			System.out.println("ENG Won The Toss And Choosed To Bowl");
		}
		System.out.println("Select Number Of Wickets:");
		int c=sc.nextInt();
		if(sum==2||sum==4||sum==6||sum==8||sum==10||sum==12)
		{
			System.out.println("IND Is batting");
		}
		for(int j=0;j<3;j++)
				{
			 System.out.println(Players[j]+" "+"is batting");
			 System.out.println(Bowlers[j]+" "+"is bowling");
			 for(int k=0;k<=20;k++)
				{
							int d=sc.nextInt();
							System.out.println(d);
							int e=r.nextInt(6);
							System.out.println(e);
							if(d==e)
							{
								System.out.println("out");
								break;
							}
							else if(d!=e)
							{
								score=d+e+score;
								System.out.println("Score is:"+score);
							}
				}
				}
	if(sum==1||sum==3||sum==5||sum==7||sum==9||sum==11)
	{
		System.out.println("ENG Is batting");
	}
	for(int j=0;j<3;j++)
			{
		 System.out.println(Batsman[j]+" "+"is batting");
		 System.out.println(Bowler[j]+" "+"is bowling");
		 for(int k=0;k<=20;k++)
			{
						int f=sc.nextInt();
						System.out.println(f);
						int g=r.nextInt(6);
						System.out.println(g);
						if(f==g)
						{
							System.out.println("out");
							break;
						}
						else
						{
							score1=f+g+score1;
							System.out.println("Score1 is:"+score1);
						}
					}
			}
	if(score>score1)
	{
		System.out.println("IND WINS");
	}
	else
	{
		System.out.println("ENG WINS");
	}
	}
	}



	
	

	

	
