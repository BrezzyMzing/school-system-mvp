import java.io.FileWriter;
import java.io.IOException;

public class SchoolPage {
    public static void main(String[] args) {
        try {
            FileWriter myWriter = new FileWriter("school.html");
            myWriter.write("<html><head><title>School Page</title></head><body>");
            myWriter.write("<h1>Welcome to our School</h1>");
            myWriter.write("<p>We offer a wide range of courses and programs to help you achieve your academic and career goals.</p>");
            myWriter.write("<h2>Programs</h2>");
            myWriter.write("<ul><li>Bachelor's Degree</li><li>Master's Degree</li><li>Doctorate Degree</li></ul>");
            myWriter.write("</body></html>");
            myWriter.close();
            System.out.println("School page created successfully.");
        } catch (IOException e) {
            System.out.println("An error occurred while creating the school page.");
            e.printStackTrace();
        }
    }
}# school-system-mvp
