# AppSigProdutos
sis de gerenciamento de cadastro

import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JTabbedPane;
import javax.swing.JTextField;
import javax.swing.JPanel;

public class AppSigCad extends JFrame {

    // Construtor da Classe
    public AppSigCad() {
        super();
        setTitle("Sistema de Gerenciamento De Clientes, Produtos e Fornecedores");
        setSize(800, 600);
        setLocationRelativeTo(null);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLayout(null);

        JTabbedPane tbmat = new JTabbedPane();
        tbmat.setSize(510, 130);
        tbmat.setLocation(40, 210);
        add(tbmat);

        JLabel mat = new JLabel();      
        mat.setText("Matricula: ");
        mat.setBounds(70, 230, 100, 30);       
        mat.setLocation(70, 230);       
        add(mat);

        JLabel tel = new JLabel();      
        tel.setText("Telefone: ");
        tel.setBounds(70, 290, 100, 30);       
        tel.setLocation(70, 290);       
        add(tel);

        JTextField Mmat = new JTextField();
        Mmat.setBounds(140, 230, 400, 30);
        add(Mmat);

        JTextField Tmat = new JTextField();
        Tmat.setBounds(140, 290, 400, 30);
        add(Tmat);


        JTabbedPane tbPanel = new JTabbedPane();
        tbPanel.setSize(545, 350);
        tbPanel.setLocation(20, 10);
        add(tbPanel);

        JPanel pnlCliente = new JPanel();
        pnlCliente.setLayout(null);
        tbPanel.addTab("Cliente", pnlCliente);
        

        
        
        
        

        setVisible(true);
    }

    public static void main(String[] args) throws Exception {
        new AppSigCad();
    }
}

