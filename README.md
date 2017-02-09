# Divide-and-Conquer-d-vide-et-mpera-
Basic Divide and Conquer algorithm search

public class nameOne {

public static void main (String [] args){

    int myNumber = 6;
    int findNumber= guessNumber(myNumber);
    System.out.println("Your number is: " + findNumber);

}

public static int guessNumber(int n){

    int low = 1;
    int high = n;
    while(low <= high)
    {
        int mid = (low+(high-low)/2);
        if(mid == n)
            return mid;
        else if(n < mid)
            high= mid-1;
        else
            low= mid+1;
    }
    return -1;
    }
}
