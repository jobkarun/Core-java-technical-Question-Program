# Core-java-technical-Question-Program
                             
                             Core java technical Question Program
                        
                              
 ## String only program
1.     How do you count the number of occurrences of each character in a string?
        
          val str="karun kumar"
          val ch=str.toCharArray()
          val map=HashMap<Char,Int>()

          for(i in ch){
             if(map.containsKey(i)){
             map.put(i, map[i]!! +1)
            }else map.put(i,1)
           }
          map.forEach { k, v -> println(" Key: $k --  Values: $v")}

2.	   How do you remove all white spaces from a string in java?
       
        val str="karun kumar Singh"
         for(i in 0..str.length-1){
          if(str[i] !=' '){
             print(str[i])
          }
        }


3.	   How do you covert to string to array? 
      
         * val str="This is Ram"
          val sb=str.split(" ")
          for (i in 0..sb.size-1){
          println(sb[i])
          }

4.     Write a java program to reverse a string and without using reverse()?
            
        * val str="karun"
          for(i in str.length-1 downTo 0){
          print(str[i])
          }
        * val sb=StringBuilder(str)
          print(sb.reverse())

5.	   Write a java program to count word a string?  

       var count=1
       val str="This is Mohan"
       for (i in 0.. str.length-1) {
         if(str[i]==' ')
          count++
        }
       println("Total Words:"+ count)


6.	   Write a Java program to find the length of a String without using inbuilt functions.
        var count=0
        val str="This is Ram"
        for (i in str.toCharArray()) {
          count++
        } 
        println(count)

7.	    Write a java program to reverse each word of a given string?
         val str="This is Mohan"
         val s=str.split(' ')
         for (i in s.size-1 downTo 0) {
           print(" " +s[i])
         }   
         
         output-> Mohan is This
         

8.	    Write a program to check if a String is a palindrome in Java? 
      
        val str="madam"
        var rev=""
         for (i in str.length-1 downTo 0) {
            rev+=str[i]
         }
         if(str==rev){
             println("this is a palindrome : "+str)
         } else  println("this is Not palindrome :"+str)

9.	     How do you convert string to integer and integer to string in java?
       
        * val str:String="12"
          val a:Int=34
          val c:Int=a+Integer.parseInt(str)
          print(c)
          
10.	    Write a java program to check whether two strings are anagram or not?
      
         val str1="karun"
         val str2="arun"

         val s1 = str1.replace("\\s", "");
         val s2 = str2.replace("\\s", "");

         var status = true;
             if(s1.length != s2.length)
                 status = false;
             else
             {
                 val arr1 = s1.toLowerCase().toCharArray();
                 val arr2 = s2.toLowerCase().toCharArray();
                 Arrays.sort(arr1);
                 Arrays.sort(arr2);
                 status = Arrays.equals(arr1, arr1);
             }

          if(status)
                 System.out.println(s1+" and "+s2+" are anagrams");
             else
                 System.out.println(s1+" and "+s2+" are not anagrams");



12.     Write a Java program to find first non repeated character in a string.
   
13.     Write a Java program to check  if given strings are Isomorphic.
