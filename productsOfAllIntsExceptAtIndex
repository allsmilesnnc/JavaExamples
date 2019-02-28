/* package whatever; // don't place package name! */

import java.util.*;
import java.lang.*;
import java.io.*;

class myCode
{
    public static void main (String[] args) throws java.lang.Exception
    {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        String input = br.readLine();
        int[] intArray = Arrays.stream(input.substring(1, input.length()-1).split(",")).map(String::trim).mapToInt(Integer::parseInt).toArray();
    
        getProductsOfAllIntsExceptAtIndex(intArray);
    }
    
    public static void getProductsOfAllIntsExceptAtIndex(int[] intArray) {
        int[] productsOfAllIntsExceptAtIndex = new int[intArray.length];
        
        // Add your code here...
        int productSoFar = 1;
        for (int i=0; i < intArray.length; i++) {
            productsOfAllIntsExceptAtIndex[i] = productSoFar;
            productSoFar *= intArray[i];
        }

        productSoFar = 1;
        for (int i = intArray.length - 1; i>=0; i--) {
            productsOfAllIntsExceptAtIndex[i] *= productSoFar;
            productSoFar *= intArray[i];
        }
        
        for (int i=0; i<productsOfAllIntsExceptAtIndex.length; i++) {
        System.out.println(productsOfAllIntsExceptAtIndex[i]);
        }
    }
}
