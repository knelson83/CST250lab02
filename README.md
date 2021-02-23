# public class TwoDimensionalArrays {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
      
     int[][] myGrid = { {1,2,3,4}, {5,6,7,8}, {9,10,11,12} };
     
     int[][] myGrid2 = { {-26,-13,-17,-16,37}, {-83,-3,-25,-1,-100} };
     printMaxOfEachRow(myGrid2);
        
    }
    public static void printMaxOfEachRow(int[][] inputArray){
        
        int maxOfEachRow;
        for (int row = 0; row < inputArray.length; row++){
            
            
            maxOfEachRow = inputArray[row][0];
            for(int col = 0; col < inputArray[row].length; col++){
               if(inputArray[row][col]> maxOfEachRow){
                   maxOfEachRow = inputArray[row][col];
               }
             
            }
        System.out.println("The Max value at row " + row + " is : " + maxOfEachRow);
        
        }
    }
