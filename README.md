# Java-Program-to-Check-Whether-Given-String-is-palindrome-or-not
If a string is palindrome, it gives the same string even after reversing it.
import java.io.*;
class Programming9
{
  public static void main (String args[]) throws IOException
//IO Exception will thrown if an I/O errors occur
  {
    BufferedReader br = new BufferedReader (new InputStreamReader (System.in));	//accept String from keyboard
      System.out.println ("enter the String:");
    String str = br.readLine ();	//  read from BufferReader class
    String temp = str;		// converting the string into StringBuffer

    StringBuffer sb = new StringBuffer (str);
      sb.reverse ();		//reverse String into StringBuffer
      str = sb.toString ();	//convert StringBuffer into a String

    if (temp.equalsIgnoreCase (str))	//compare original string available in temp with this reversed String
        System.out.println (temp + " is palindrome");
    else
        System.out.println (temp + " is not palindrome");
  }
}
