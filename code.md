import java.util.Scanner;
///mine
public class StringUtil{
    public static void main(String[] args){
        System.out.println("??:");
        Scanner inp = new Scanner(System.in);
        String string = inp.nextLine();
        System.out.println("??:");
        String ac = string.replaceAll(" +","");
        System.out.println(ac);
    }
}

//result

import java.util.Scanner;
public class StringUtil {
    public static void main(String[] args) {
        Scanner in =new Scanner(System.in);
        //??String?
        String a=in.nextLine();
        StringBuilder stringBuilder = new StringBuilder(a);
        for (int i = 0; i < stringBuilder.length(); i++) {
            if (stringBuilder.charAt(i)==' ') {
                System.out.println(i);
                stringBuilder.deleteCharAt(i);
                i--;
            }else {
                stringBuilder.charAt(i);
            }
        }
        System.out.println(stringBuilder.toString());
    }
}
