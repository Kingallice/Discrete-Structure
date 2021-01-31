package largest.palindromic.product;

public class LargestPalindromicProduct {

    public static void main(String[] args) {
        System.out.println("Largest Palindromic Product: " + LargestPalindromicProduct(100,1000));
    }
    public static int LargestPalindromicProduct(int low, int high)
    {
        int Product = 0;
        for(int i = low; i < high; i++)
        {
            for(int j = low; j < high; j++)
            {
                if(isPalindrome((i*j) + ""))
                {
                    if(Product < i*j)
                        Product = i*j;
                }
            }
        }
        return Product;
    }
    public static boolean isPalindrome(String text) {
        boolean out = false;
        int i = text.length() - 1;

        if (text.charAt(0) == text.charAt(i) && i - 1 <= 1) 
        {
            out = true;
        } 
        else if (text.charAt(0) == text.charAt(i)) 
        {
            text = text.substring(1, i);
            out = isPalindrome(text);
        } 
        return out;
    }
}
