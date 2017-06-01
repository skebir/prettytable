# prettytable

PrettyTable is a simple Java library designed to make it quick and easy to represent tabular data in visually appealing ASCII tables, like this:

```
+-----------+----------+---------------------+-------------+
| Firstname | Lastname |        Email        |    Phone    |
+-----------+----------+---------------------+-------------+
|   John    |   Doe    | johndoe@nothing.com | +2137999999 |
|   Jane    |   Doe    | janedoe@nothin.com  | +2137999999 |
+-----------+----------+---------------------+-------------+
```

The preceding output can be produced using the following code :

```java
public static void main(String[] args) {
        PrettyTable table = new PrettyTable("Firstname", "Lastname", "Email", "Phone");
        table.addRow("John", "Doe", "johndoe@nothing.com", "+2137999999");
        table.addRow("Jane", "Doe", "janedoe@nothin.com", "+2137999999");
        System.out.println(table);
}
```
