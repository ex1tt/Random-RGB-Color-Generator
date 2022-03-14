package colorGenerator;
import java.awt.*;
import java.awt.event.*;
import javax.swing.*;
import java.util.Random;

public class ColorGenerator {

	// generating random RGB values...
	public static int generateRGB() {
		Random random = new Random();
		int RGB = random.nextInt(256);
		return RGB;		
	}
	
	public static void main(String[] args) {
		
		// creating the color square
		JPanel color = new JPanel();
		color.setBackground(new Color(255, 255, 255));
		color.setBounds(175,160,250,250);	
		color.setBorder(BorderFactory.createLineBorder(Color.WHITE));
		
		JLabel label = new JLabel("RGB:" + " (" + 255 + ", " + 255 + ", " + 255 + ")");
		label.setFont(new Font("Serif", Font.PLAIN, 25));
		label.setBounds(185, 60, 1000, 100);
		label.setForeground(Color.WHITE);
		
		// creating button and key listener
		JButton button = new JButton("Click For New Color");
		button.setBounds(200,435,200,50);
		button.setFocusable(false);
		button.addActionListener(new ActionListener() {
						
			public void actionPerformed(ActionEvent e){  // assigning random RGB values to three variables
		        int red = generateRGB();
		        int green = generateRGB();
		        int blue = generateRGB();
		        
		        color.setBackground(new Color(red, green, blue)); // that are then casted onto the label        		        
		        label.setText("RGB:" + " (" + red + ", " + green + ", " + blue + ")");
		        
			}  
		});
		
		// creating frame of the program
		JFrame frame = new JFrame("RGB Color Generator");
		frame.setVisible(true);
		frame.setSize(600, 600);
		frame.setResizable(false);
		frame.getContentPane().setBackground(Color.BLACK);
		frame.setLayout(null);
		frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		frame.add(color);
		frame.add(button);
		frame.add(label);
		
		}
	}
