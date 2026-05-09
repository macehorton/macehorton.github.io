# macehorton.github.io
public class Swimwear {
    private String id;
    private String name;
    private String size; // e.g., XS, S, M, L, XL
    private double price;
    private String color;

    public Swimwear(String id, String name, String size, double price, String color) {
        this.id = id;
        this.name = name;
        this.size = size;
        this.price = price;
        this.color = color;
    }

    // Getters
    public String getName() { return name; }
    public double getPrice() { return price; }
    public String getSize() { return size; }

    @Override
    public String toString() {
        return String.format("%s (%s) - %s: $%.2f", name, color, size, price);
    }
}
import java.util.ArrayList;
import java.util.List;

public class ShoppingCart {
    private List<Swimwear> items;

    public ShoppingCart() {
        this.items = new ArrayList<>();
    }

    public void addItem(Swimwear item) {
        items.add(item);
        System.out.println("Added to cart: " + item.getName());
    }

    public double calculateTotal() {
        return items.stream().mapToDouble(Swimwear::getPrice).sum();
    }

    public void displayCart() {
        System.out.println("\n--- Your Shopping Cart ---");
        for (Swimwear item : items) {
            System.out.println("- " + item);
        }
        System.out.printf("Total: $%.2f\n", calculateTotal());
    }
}
public class SwimwearStore {
    public static void main(String[] args) {
        // 1. Initialize some inventory
        Swimwear bikini = new Swimwear("S001", "Tropical Floral Bikini", "M", 45.99, "Ocean Blue");
        Swimwear onePiece = new Swimwear("S002", "Classic High-Neck One-Piece", "S", 59.50, "Midnight Black");
        Swimwear sarong = new Swimwear("S003", "Sheer Beach Wrap", "One Size", 25.00, "Sunset Orange");

        // 2. User starts shopping
        ShoppingCart myCart = new ShoppingCart();
        
        System.out.println("Welcome to the Azure Tide Swimwear Store!\n");
        
        myCart.addItem(bikini);
        myCart.addItem(sarong);

        // 3. Review and Checkout
        myCart.displayCart();
        
        System.out.println("\nProceeding to secure payment...");
    }
}
