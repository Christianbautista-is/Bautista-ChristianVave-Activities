class Box<T> {
    private T value;

    public void setValue(T value) {
        this.value = value;
    }

    public T getValue() {
        return value;
    }
}

public class Generics{
    public static void main(String[] args) {

        Box<String> stringBox = new Box<>();
        stringBox.setValue("Hello, BSIS!");
        System.out.println("String Value: " + stringBox.getValue());

        Box<Integer> intBox = new Box<>();
        intBox.setValue(100);
        System.out.println("Integer Value: " + intBox.getValue());
    }
}
