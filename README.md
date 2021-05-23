import java.io.FileWriter;
import java.io.IOException;
import java.io.BufferedWriter;
import java.io.File;

public class Jala {
	public static void main(String[] args) throws IOException 
  {
		File file = new File("myfile.txt");
		BufferedWriter bw = new BufferedWriter(new FileWriter(file));
		try
        {
            bw.write("Hello I'm sai!!");
        }
         catch (IOException e) {
            System.out.println("Sorry!!! can't read the file");;
        }
        bw.close();
   }
}
