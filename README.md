# findingdistinctnumbers

public class HelloWorld{

     public static void main(String []args){
        
        int[] array = {0,0,1,1,6,6,7,0};
        System.out.println(array);
        boolean alreadyExecuted = false;
        
        for(int i = 0; i<array.length; i++)
        {
            System.out.print(array[i]);
        }
        
        int count;
        
        int[] newarray = new int[50];
        
        for( int i = 0; i< array.length; i++)
        {
            count = 0;
            for( int j = 0; j<array.length; j++)
            {
                if(array[i]==array[j] && i!=j)
                {
                    count++;
                }
            }
                if(count==0)
                {
                     if(!alreadyExecuted) 
                     {
                        array[i]= 0;
                        alreadyExecuted = true;
                    }
                }
        }
        
        System.out.println();
         for(int i = 0; i<array.length; i++)
        {
            System.out.print(array[i]);
        }
     }
}
