import java.util.Scanner;

class Cylinder {
    private double radius;
    private double height;
    private double area;

    public Cylinder(double radius, double height) {
        this.radius = radius;
        this.height = height;
        this.area = calculateArea();
    }

    public double getRadius() {
        return radius;
    }

    public double getHeight() {
        return height;
    }

    public double getArea() {
        return area;
    }

    private double calculateArea() {
        return 2 * Math.PI * Math.pow(radius, 2) + 2 * Math.PI * radius * height;
    }
}

class CylinderVol extends Cylinder {
    private double volume;

    public CylinderVol(double radius, double height) {
        super(radius, height);
        this.volume = calculateVolume();
    }

    public double getVolume() {
        return volume;
    }

    private double calculateVolume() {
        return Math.PI * Math.pow(getRadius(), 2) * getHeight();
    }
}

public class CylinderMain {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the radius of the cylinder: ");
        double radius = scanner.nextDouble();

        System.out.print("Enter the height of the cylinder: ");
        double height = scanner.nextDouble();

        CylinderVol cylinder = new CylinderVol(radius, height);

        System.out.println("Area of the cylinder: " + cylinder.getArea());
        System.out.println("Volume of the cylinder: " + cylinder.getVolume());
    }
}
