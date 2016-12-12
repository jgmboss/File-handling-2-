import java.io.FileWriter;
import java.io.BufferedWriter;
import java.io.IOException;
public class Qtwo
{
    public static void main (String args []) throws IOException
    {
        String[][] namesNclass = {{"Sophie", " Stanfield", " Class 5"}, {" James", " Kitson", " Class 5"}, {" Zoe", " Gaskill", " Class 1"},{" Paul", " Johns", " Class 1"}, {" Freya", " Moore", " Class 5"}};


        FileWriter fw = new FileWriter("Macintosh HD \\ Users \\ rexpon \\ Documents.txt", true);
        BufferedWriter bw = new BufferedWriter(fw);


        for (int r = 0; r < namesNclass.length; r++){
            for (int c = 0; c < namesNclass[r].length; c++){
                fw.write (namesNclass[r][c] + "\t");


            }
            fw.write ("\n");
        }
        fw.close();
    }
}
