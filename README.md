import java.util.ArrayList;

class DataStore<T> {
    private ArrayList<T> list = new ArrayList<>();

    public void addData(T data) {
        list.add(data);
    }

    public void displayData() {
        for (T item : list) {
            System.out.println(item);
        }
    }
}

public class GenericsArrayList{
    public static void main(String[] args) {

        DataStore<String> names = new DataStore<>();
        names.addData("Jastin");
        names.addData("Alexus");
        names.addData("James");

        System.out.println("Names:");
        names.displayData();

        DataStore<Integer> numbers = new DataStore<>();
        numbers.addData(10);
        numbers.addData(20);
        numbers.addData(30);

        System.out.println("\nNumbers:");
        numbers.displayData();
    }
}
