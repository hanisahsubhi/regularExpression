class RegexEg {
  public static void main(String[] args) {

    //two methods (matches() and pattern.matches() ) will print the same results:
    //matches() will compare input with regex and will return a boolean
    System.out.println(input.matches(regex));

    System.out.println(Pattern.matches(regex,input));

    //String input = "This is a string";
    //String regex = "This is a string";

    //hence output will be true.

    //split() method split the given string into an Array of String based on the regular expression in the method argument:
    
//sample string   
String chainedString = "Lets-break-this-chain-!";
//Creating Regex for splitting the String
String regex = "-";
//Splitting the String using split() method
//split()divides the String and stores them in a Array of String
String[] freeString = chainedString.split(regex);
/**
 *  freeString = ("Lets", "break", "this", "chain", "!")
 */
  }
 
 
//Regex pattern
  // To search the pattern having two characters in between A and l in the given string "A%(lication".
String searchStr = "A%(lication";
String regexStr = "A..lication";
System.out.println(searchStr.matches(regexStr)); 

//To check if a number is found 0 or n times after X in the given string.
String searchStr = "X4756Y";
String regexStr = "X\\d*Y";
System.out.println(searchStr.matches(regexStr));    
}
