# melekabdullaieva1lab


package lab1;

public class Person {

    private String name;
    private int age;

    @Override
    public boolean equals(Object obj) {
        if(obj==null) {
            return false;
        }
        // TODO Auto-generated method stub
        return obj==this||((Person)obj).age==this.age&&((Person)obj).name.equals(this.name);
    }
}
