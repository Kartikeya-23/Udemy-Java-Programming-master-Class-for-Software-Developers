public class NumberToWords {


    public static int getDigitCount(int number) {
        int count = 0;
        if (number == 0) {
            return 1;
        }
        if (number < 0) {
            return -1;
        }
        while (number > 0) {
            number /= 10;
            count++;;
        }
        return count;
    }

    public static int reverse(int number) {
        int remainder,reverseNumber = 0;
        boolean isNegative = false;
        if (number < 0) {
            number = Math.abs (number);
            isNegative = true;
        }
        while (number > 0) {
            remainder = number % 10;
            reverseNumber = reverseNumber * 10 + remainder;
            number /= 10;
        }
        if (isNegative == true) {
            return -reverseNumber;
        }
        return reverseNumber;
    }

    public static void numberToWords(int number) {

        if (number < 0) {
            System.out.println("Invalid Value");
        } else if (number == 0) {
            System.out.println("Zero");
        } else {
            int reverseNumber = reverse(number);
            int numberDigitCount = getDigitCount(number);
            int reverseNumberDigitCount = getDigitCount(reverseNumber);
            String s = "";
            int remainder = 0;
            while (reverseNumber > 0) {
                remainder = reverseNumber % 10;
                switch(remainder) {
                    case 0:
                        s = s + "Zero ";
                        break;
                    case 1:
                        s = s + "One ";
                        break;
                    case 2:
                        s = s + "Two ";
                        break;
                    case 3:
                        s = s + "Three ";
                        break;
                    case 4:
                        s = s + "Four ";
                        break;
                    case 5:
                        s = s + "Five ";
                        break;
                    case 6:
                        s = s + "Six ";
                        break;
                    case 7:
                        s = s + "Seven ";
                        break;
                    case 8:
                        s = s + "Eight ";
                        break;
                    case 9:
                        s = s + "Nine ";
                        break;
                    default:
                        break;
                }
                reverseNumber /= 10;
            }
            if (numberDigitCount > reverseNumberDigitCount) {
                for(int i = 0; i < (numberDigitCount - reverseNumberDigitCount); i++) {
                    s = s + "Zero ";
                }

            }
            System.out.println(s);
        }


    }
}
