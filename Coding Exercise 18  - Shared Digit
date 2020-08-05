public class SharedDigit {

    public static boolean hasSharedDigit(int firstNumber, int secondNumber) {
        if (firstNumber < 10 || firstNumber > 99 || secondNumber < 10 || secondNumber > 99) {
            return false;
        } else {
            int firstNumberLast = firstNumber % 10;
            int firstNumberStart = firstNumber / 10;
            int secondNumberLast = secondNumber % 10;
            int secondNumberStart = secondNumber / 10;
            if (firstNumberStart == secondNumberStart || firstNumberStart == secondNumberLast || firstNumberLast == secondNumberStart
                           || firstNumberLast == secondNumberLast) {
                return true;
            } else {
                return false;
            }
        }

    }
}
