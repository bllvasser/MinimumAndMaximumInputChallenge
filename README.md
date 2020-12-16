# MinimumAndMaximumInputChallenge
package academy.learnprogrmming;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner console = new Scanner(System.in);

        int minimumNumber = Integer.MAX_VALUE;
        int maximumNumber = Integer.MIN_VALUE;



        while(true) {

            System.out.println("Enter number");
            boolean isAnInt = console.hasNextInt();

            if(isAnInt){

                int number = console.nextInt();

                if(number > maximumNumber) {
                    maximumNumber = number;
                }
                if(number < minimumNumber) {
                    minimumNumber = number;
                }
            } else {
                break;
            }
            console.nextLine();

        }

        System.out.println("The minimum number is " + minimumNumber + " and the maximum number is " + maximumNumber);
        console.close();
    }
}
"C:\Program Files\Java\jdk-15.0.1\bin\java.exe" "-javaagent:C:\Users\nadiy\OneDrive\Desktop\IntelliJ IDEA Community Edition 2020.2.3\lib\idea_rt.jar=50024:C:\Users\nadiy\OneDrive\Desktop\IntelliJ IDEA Community Edition 2020.2.3\bin" -Dfile.encoding=UTF-8 -classpath C:\Users\nadiy\IdeaProjects\MinAndMaximumChallenge\out\production\MinAndMaximumChallenge academy.learnprogrmming.Main
Enter number
1
Enter number
2
Enter number
3
Enter number
a
The minimum number is 1 and the maximum number is 3

Process finished with exit code 0
