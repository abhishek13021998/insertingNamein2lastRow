# insertingNamein2lastRow
In this programme we insert name in box in last 2nd row leaving last 2 column space
first we take name of 
String name=sc.next();
now we take now of rows 
int r=sc.nextInt();
now we take no of column
int cc=sc.nextInt();
here column number   must be greater length of name
here are the logic using for loop we can make box and insert name
for(int i=0;i<r;i++)
		{
			for(int j=0;j<c;j++)
			{
				if((i==0&&j==0)||(i==0&&j==c-1)||(i==r-1&&j==0)||(i==r-1&&j==c-1))
				System.out.print("+");
				else if(i==0||i==r-1)
				System.out.print("-");
				else if(j==0||j==c-1)
				System.out.print("|");
				else if(i==r-3&&j==c-(name.length()+2))
				{
					for(int k=0;k<name.length();k++)
					System.out.print(name.charAt(k));
					j=j+name.length()-1;
				}
				else
				System.out.print(" ");
			}
			System.out.println();
		}![Screenshot (991)](https://user-images.githubusercontent.com/84003456/118531378-67707280-b763-11eb-9936-50efac46a9aa.png)
