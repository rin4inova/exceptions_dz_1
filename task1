package DZ1;

/*Задание 1. Преобразование строки в число.
Реализуйте метод covertAndSum, который принимает массив строк, каждая
из которых должна быть преобразована в целое число. Метод возвращает
сумму всех чисел. Если хотя бы одна строка не может быть преобразована
в число, метод должен выбросить исключение NumberFormatException.
Дополнительно, если сумма чисел превышает 100, выбрасывайте
ArithmeticException с сообщением "Превышен лимит суммы".
 */

public class Dz1_1 {
    public static void main(String[] args) {
        try {
            String[] strings = {"50", "60"};
            System.out.println(convertAndSum(strings));
        }
        catch (NumberFormatException e) {
            System.out.println("Ошибка преобразования строки в число");
        }
        catch (ArithmeticException e) {
            System.out.println(e.getMessage());
        }
    }

    public static int convertAndSum(String[] strings) {
        int sum = 0;
        for (String s : strings){
            try {
                int number = Integer.parseInt(s);
                sum += number;
            } catch (NumberFormatException e){
                throw new NumberFormatException("Ошибка преобразования строки в число: " + s);
            }
        }
        if(sum > 100){
            throw new ArithmeticException("Превышен лимит суммы");
        }
        return sum;
    }
}
