# Anagram-Java_interview_practice
package com.anagram;

import java.util.Arrays;

/**
 *
 * @author Dinesh Nanda
 * 
 */

public class Anagram {

    public static void main(String[] args) {
        
        String str1 = "Brag";
        String str2 = "Grab";
        
        str1 = str1.toLowerCase();
        str2 = str2.toLowerCase();
        
        if (str1.length() != str2.length()) {  
            
            System.out.println("Both the strings are not anagram");
            
        }else{
            
            //Converting both the arrays to character array  
            char[] char1 = str1.toCharArray();
            char[] char2 = str2.toCharArray();
            
            Arrays.sort(char1);
            Arrays.sort(char2);
            
            if(Arrays.equals(char1, char2) == true){
                
                System.out.println("Both the strings are anagram");
            }else{
                
                System.out.println("Both the strings are not anagram");
            }
     
        }   
    }
}
