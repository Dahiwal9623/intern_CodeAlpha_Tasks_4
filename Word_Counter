package CodeAlpha_Task;

import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

public class Word_Counter{
	
	    public static void main(String[] args) {
	        JFrame frame = new JFrame("Word Counter");
	        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
	        frame.setSize(496, 365);

	        JLabel titleLabel = new JLabel("Word Counter");
	        titleLabel.setBounds(150, 10, 100, 20);

	        final JTextArea textArea = new JTextArea(); // Declare textArea as final
	        textArea.setBounds(50, 40, 300, 60);

	        JButton countButton = new JButton("Count Words");
	        countButton.setBounds(150, 120, 100, 30);

	        final JLabel resultLabel = new JLabel(); // Declare resultLabel as final
	        resultLabel.setBounds(150, 160, 100, 20);

	        countButton.addActionListener(new ActionListener() {
	 
	            public void actionPerformed(ActionEvent e) {
	                String text = textArea.getText();
	                int wordCount = countWords(text);
	                resultLabel.setText("Word Count: " + wordCount);
	            }
	        });

	        frame.add(titleLabel);
	        frame.add(textArea);
	        frame.add(countButton);
	        frame.add(resultLabel);
	        frame.setLayout(null);
	        frame.setVisible(true);
	    }

	    public static int countWords(String text) {
	        String[] words = text.split("\\s+");
	        return words.length;
	    }
	}
