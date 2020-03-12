# anagram
to find two words are anagram or not
          
              import java.util.*;
              public class Main
              {
                public static void main(String[] args) {
                Scanner sc = new Scanner(System.in);
                System.out.println("ENTER THE STRING1: ");
                String str1 = sc.nextLine();
                System.out.println("ENTER THE STRING2: ");
                String str2 = sc.nextLine();
                char arr1[] = str1.toLowerCase().toCharArray();
                char arr2[] = str2.toLowerCase().toCharArray();
                Arrays.sort(arr1);
                Arrays.sort(arr2);
                if(str1.length() != str2.length())
                {
                    System.out.println("NOT AN ANAGRAM");
                }
                else
                {
                    if(Arrays.equals(arr1,arr2))
                    {
                       System.out.println("ANAGRAM"); 
                    }
                    else
                    {
                       System.out.println("NOT AN ANAGRAM");  
                    }
                }
              }
            }
  
