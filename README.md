# java_Strings

package koppula;
import java.util.*;
public class Strings
{
	public static void main(String args[])
	{
		/*String s=new String("Aditya");// String 
		s=s.concat(" engineering");
		System.out.println(s);*/
		
		/*StringBuffer sb=new StringBuffer("Aditya");// mutability
		sb.append("College");
		System.out.println(sb);*/
		
		/*String s1=new String("Aditya College of Engineering");
		System.out.println(s1.charAt(9));*/
		
		/*String s1=new String("i am learning java Programming");
		String s2=new String("i am learning java Programming");
		//System.out.println(s1==s2);*/
		
		// returns boolean Value,, here it is false because of "==" the memory reference will be compared.from the above s1 and s2 the content is same 
		// but reference is different(both are declared using two different new's)
		
		//System.out.println(s1.equals(s2));
		
		// returns True because here content comparison will be done, Even though there are declared using diff new's but content is same so Return TRUE
		
		//String s1=new String("I love Farming ");
		//System.out.println(s1.indexOf("l"));
		// returns the indexof the particular character
		
		/*String s2=new String("I love Farming very much");
		System.out.println(s2.lastIndexOf("v"));*/
		
		// returns the last index of repeated character
	     
		/*String a=new String("AdityA");
		String b=new String("aditya");
		//System.out.println(a.equals(b));*/
		
		// returns false because case sensitive
		
		/*String a1=new String("AdityA");
		String b1=new String("aditya");
		System.out.println(a1.equalsIgnoreCase(b1));*/
		
		// this function avoids the case sensitive and Returns True
		
		/*String a2=new String("Aditya College of Engineering is the best eng college in EG");
		System.out.println(a2.replace("e", "E"));*/
		
		// here all 'e' are replaced with 'E'
		
		/*String a3=new String("Aditya college of Engineering is the best eng college in EG");
		System.out.println(a3.replaceFirst("college","COLLEGE"));*/
		
		// first occurenced of college is replaced with "COLLEGE"
		
		//String a3=new String("Aditya college of Engineering is the best eng college in EG");
		//System.out.println(a3.replaceAll("college","COLLEGE"));
		
		// all college occurences are replaced with COLLEGE
		
		
		// program to find the no of vowels and consonants in a given word
		
	}
	
}

public class Vowel_word {
	public static void main(String args[])throws Exception
	{
		InputStreamReader isr=new InputStreamReader(System.in);
		BufferedReader br=new BufferedReader(isr);
		String ip; 
		int v=0,c=0;
		ip=br.readLine();
		char x[]=ip.toCharArray(); // convert string to char array
		for(int i=0;i<x.length;i++)// 
		{
			if (x[i]=='a' || x[i]=='e' || x[i]=='i' || x[i]=='o' || x[i]=='u')
				v++;
			else	
			c++;
		}
		System.out.println(v+" vowels  and  "+c+" consonants  ");
}
}

/*InputStreamReader isr=new InputStreamReader(System.in);
		BufferedReader br=new BufferedReader(isr);
		String str1;
		int i,l=0,u=0,d=0,s=0;
		str1=br.readLine();
		char ch[]=str1.toCharArray();
		for(i=0;i<ch.length;i++)
	if(Character.isLowerCase(ch[i]))
	{
		l++;
	}
	else if (Character.isUpperCase(ch[i]))
			{
				u++;
			}
	else if (Character.isDigit(ch[i]))
		{
		d++;
		}
	else
	{
		s++;
	}
		System.out.println(l+" "+u+" "+d+" "+s);
		}
		}*/
		
		/*InputStreamReader isr=new InputStreamReader(System.in);
		BufferedReader br=new BufferedReader(isr);
		String a;
		int sum=0;
		a=br.readLine();
		char c[]=a.toCharArray();
		for (int i=0;i<c.length;i++)
		{
			if (Character.isDigit(c[i]))
				sum+=Integer.parseInt(c[i]+"");// another approach by using c[i]-48// here 48 means its a unicode of zero
		}
		System.out.println(sum);
	}
		
}*/
		
		InputStreamReader isr=new InputStreamReader(System.in);
		BufferedReader br=new BufferedReader(isr);
		String s1;
		StringBuffer sb1;
		s1=br.readLine();
		String words[]=s1.split(" ");
			for(int i=0;i<words.length;i++)		
		{
			sb1=new StringBuffer(words[i]);
			System.out.print(sb1.reverse()+" ");
		}
		/*sb.setCharAt(0,'r'); // setting the 'r' at index 0
		sb.deleteCharAt(5);// deleting the char at index 5*/
		// sb.reverse();
		//sb.delete(5,8);
		//sb.append('reddy');
		//sb.insert(4,'e'); // (index, character)
		// length and capacity sb func can be executed within the System.out statement 
		
		
	}
}
		
		
	
