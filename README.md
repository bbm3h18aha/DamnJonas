# DamnJonas
package ubung37;

import java.awt.BorderLayout;
import java.awt.Container;
import java.awt.Dimension;
import java.awt.FlowLayout;
import java.awt.GridLayout;

import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JPanel;
import javax.swing.JTextField;
import javax.swing.text.JTextComponent;


public class English extends JFrame {
	
	Container nihaoma;
	
	public English() {
		
	nihaoma = getContentPane();
	
	JLabel lenglisch = new JLabel ("Englisch :");
	JLabel ldeutsch = new JLabel ("Deutsch :");
	
	JPanel panel = new JPanel();
	JPanel penglisch = new JPanel();
	JPanel pdeutsch = new JPanel();
	JPanel pgo = new JPanel();
	
	JTextField tenglisch = new JTextField(15);
	JTextField tdeutsch = new JTextField(15);
	
	JButton bgo = new JButton ("GO");
	
	penglisch.setLayout(new GridLayout(0,1,30,10));
	penglisch.add(lenglisch);
	penglisch.add(ldeutsch);
	
	pdeutsch.setLayout(new GridLayout(0,1,30,10));
	pdeutsch.add(tenglisch);
	pdeutsch.add(tdeutsch);
	
	pgo.setLayout(new GridLayout(0,1,30,10));
	pgo.add(bgo);
	
	
	panel.setLayout(new FlowLayout());
	panel.add(penglisch);
	panel.add(pdeutsch);
	panel.add(pgo);
	nihaoma.add(panel,BorderLayout.NORTH);
	
	setTitle("Wörterbuch");
	setDefaultCloseOperation(EXIT_ON_CLOSE);
	setSize(new Dimension(380,110));
	setMinimumSize(new Dimension(380,110));

	setVisible(true);
	}
	
	
	
}
