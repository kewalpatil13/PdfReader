# PdfReader
It's can analyze the result pdf(unipune) 
package javaapplication6;


import java.io.File;
import javax.swing.JFileChooser;
import javax.swing.JOptionPane;
import org.apache.pdfbox.pdmodel.PDDocument;
import org.apache.pdfbox.text.PDFTextStripper;
import org.apache.pdfbox.text.PDFTextStripperByArea;
import java.util.*;
import java.io.*;
import java.text.MessageFormat;
import java.util.logging.Level;
import java.util.logging.Logger;
import javax.swing.*;
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author user
 */
public class Result extends javax.swing.JFrame {

    /**
     * Creates new form Result
     */
    File f=null;
    String filename=null;
    public Result() {
        initComponents();
        jTextArea2.setVisible(false);
        jLabel3.setVisible(false);
        jLabel4.setVisible(false);
        jTextField1.setVisible(false);
        jTextField2.setVisible(false);
        search.setVisible(false);
        jButton2.setVisible(false);
        jButton3.setVisible(false);
        jButton4.setVisible(false);
    }

    /**
     * This method is called from within the constructor to initialize the form.
     * WARNING: Do NOT modify this code. The content of this method is always
     * regenerated by the Form Editor.
     */
    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">//GEN-BEGIN:initComponents
    private void initComponents() {

        jLabel2 = new javax.swing.JLabel();
        jScrollPane1 = new javax.swing.JScrollPane();
        jTextArea1 = new javax.swing.JTextArea();
        jPanel1 = new javax.swing.JPanel();
        jLabel3 = new javax.swing.JLabel();
        view = new javax.swing.JButton();
        jTextField2 = new javax.swing.JTextField();
        jLabel4 = new javax.swing.JLabel();
        Choose = new javax.swing.JButton();
        jButton1 = new javax.swing.JButton();
        file = new javax.swing.JTextField();
        jButton2 = new javax.swing.JButton();
        search = new javax.swing.JButton();
        jButton3 = new javax.swing.JButton();
        jScrollPane2 = new javax.swing.JScrollPane();
        jTextArea2 = new javax.swing.JTextArea();
        jTextField1 = new javax.swing.JTextField();
        jLabel1 = new javax.swing.JLabel();
        jButton5 = new javax.swing.JButton();
        jButton4 = new javax.swing.JButton();

        jLabel2.setText("jLabel2");

        jTextArea1.setColumns(20);
        jTextArea1.setRows(5);
        jScrollPane1.setViewportView(jTextArea1);

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);
        setTitle("Result Analysis");
        setResizable(false);

        jPanel1.setBorder(javax.swing.BorderFactory.createEmptyBorder(1, 1, 1, 1));

        jLabel3.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N
        jLabel3.setText("Enter Seat No");

        view.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N
        view.setText("View PDF");
        view.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                viewActionPerformed(evt);
            }
        });

        jTextField2.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N

        jLabel4.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N
        jLabel4.setText("Search By Subject Code");

        Choose.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N
        Choose.setText("Choose");
        Choose.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                ChooseActionPerformed(evt);
            }
        });

        jButton1.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N
        jButton1.setText("Analyse");
        jButton1.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton1ActionPerformed(evt);
            }
        });

        file.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N

        jButton2.setText("Check Result");
        jButton2.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton2ActionPerformed(evt);
            }
        });

        search.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N
        search.setText("Search Seat");
        search.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                searchActionPerformed(evt);
            }
        });

        jButton3.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N
        jButton3.setText("Clear");
        jButton3.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton3ActionPerformed(evt);
            }
        });

        jTextArea2.setColumns(20);
        jTextArea2.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N
        jTextArea2.setRows(5);
        jScrollPane2.setViewportView(jTextArea2);

        jTextField1.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N

        jLabel1.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N
        jLabel1.setText("Choose PDF File");

        jButton5.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N
        jButton5.setText("Result Status");
        jButton5.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton5ActionPerformed(evt);
            }
        });

        javax.swing.GroupLayout jPanel1Layout = new javax.swing.GroupLayout(jPanel1);
        jPanel1.setLayout(jPanel1Layout);
        jPanel1Layout.setHorizontalGroup(
            jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(jPanel1Layout.createSequentialGroup()
                .addContainerGap()
                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addGroup(jPanel1Layout.createSequentialGroup()
                        .addComponent(jLabel4)
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                        .addComponent(jTextField2, javax.swing.GroupLayout.PREFERRED_SIZE, 189, javax.swing.GroupLayout.PREFERRED_SIZE))
                    .addGroup(jPanel1Layout.createSequentialGroup()
                        .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                            .addComponent(jLabel1)
                            .addComponent(jLabel3)
                            .addComponent(jButton5, javax.swing.GroupLayout.Alignment.TRAILING))
                        .addGap(18, 18, 18)
                        .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                            .addGroup(jPanel1Layout.createSequentialGroup()
                                .addComponent(file, javax.swing.GroupLayout.PREFERRED_SIZE, 237, javax.swing.GroupLayout.PREFERRED_SIZE)
                                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                                .addComponent(Choose, javax.swing.GroupLayout.PREFERRED_SIZE, 95, javax.swing.GroupLayout.PREFERRED_SIZE))
                            .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, jPanel1Layout.createSequentialGroup()
                                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                                    .addGroup(jPanel1Layout.createSequentialGroup()
                                        .addComponent(view)
                                        .addGap(56, 56, 56)
                                        .addComponent(jButton1))
                                    .addComponent(jTextField1, javax.swing.GroupLayout.PREFERRED_SIZE, 224, javax.swing.GroupLayout.PREFERRED_SIZE))
                                .addGap(15, 15, 15)
                                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                                    .addComponent(jButton2)
                                    .addComponent(search)))))
                    .addComponent(jButton3))
                .addGap(73, 73, 73)
                .addComponent(jScrollPane2, javax.swing.GroupLayout.DEFAULT_SIZE, 426, Short.MAX_VALUE)
                .addContainerGap())
        );
        jPanel1Layout.setVerticalGroup(
            jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(jPanel1Layout.createSequentialGroup()
                .addContainerGap()
                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addGroup(jPanel1Layout.createSequentialGroup()
                        .addGap(21, 21, 21)
                        .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                            .addComponent(jLabel1)
                            .addComponent(file, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addComponent(Choose))
                        .addGap(31, 31, 31)
                        .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                            .addComponent(view)
                            .addComponent(jButton1)
                            .addComponent(jButton5))
                        .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                            .addGroup(jPanel1Layout.createSequentialGroup()
                                .addGap(27, 27, 27)
                                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                                    .addComponent(jTextField1, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                                    .addComponent(search)))
                            .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, jPanel1Layout.createSequentialGroup()
                                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                                .addComponent(jLabel3)))
                        .addGap(37, 37, 37)
                        .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                            .addComponent(jLabel4)
                            .addComponent(jTextField2, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addComponent(jButton2))
                        .addGap(40, 40, 40)
                        .addComponent(jButton3)
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED, 255, javax.swing.GroupLayout.PREFERRED_SIZE))
                    .addComponent(jScrollPane2))
                .addContainerGap())
        );

        jButton4.setFont(new java.awt.Font("Times New Roman", 0, 14)); // NOI18N
        jButton4.setText("Print");
        jButton4.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButton4ActionPerformed(evt);
            }
        });

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, layout.createSequentialGroup()
                .addGap(27, 27, 27)
                .addComponent(jPanel1, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                .addContainerGap())
            .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, layout.createSequentialGroup()
                .addContainerGap(javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                .addComponent(jButton4)
                .addGap(33, 33, 33))
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addContainerGap()
                .addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                .addComponent(jButton4))
        );

        pack();
    }// </editor-fold>//GEN-END:initComponents

    private void ChooseActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_ChooseActionPerformed
    
    file.setText("");
    JFileChooser ch=new JFileChooser();
    ch.showOpenDialog(null);
    f=ch.getSelectedFile();
    filename=f.getAbsolutePath();
    file.setText(filename);
    if(filename.equals("")){
        JOptionPane.showMessageDialog(this,"Please Select Proper Path of File");
        file.setText("");
        }
    if(filename.matches("(.*).pdf")==false||filename.matches("(.*).pdf")==false){
        JOptionPane.showMessageDialog(this,"Please select PDF file only");
        file.setText("");
    }
    }//GEN-LAST:event_ChooseActionPerformed

    private void viewActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_viewActionPerformed
        if(file.getText().equals("")==false){
        jTextArea2.setVisible(true);
        jButton4.setVisible(true);
        try {
            PDDocument document = PDDocument.load(new File(filename));
            document.getClass();
            if (!document.isEncrypted())
            {
                PDFTextStripperByArea stripper = new PDFTextStripperByArea();
                stripper.setSortByPosition(true);
                PDFTextStripper Tstripper = new PDFTextStripper();
                String str = Tstripper.getText(document);
                Scanner scn = null;
                scn = new Scanner(str);
                String line="";
                jTextArea2.setText(line);
                while(scn.hasNextLine()){
                    line = scn.nextLine();
                    String s="\n"+line;
                    jTextArea2.append(s);
                }
            }
        } catch (IOException ex) {
            Logger.getLogger(Result.class.getName()).log(Level.SEVERE, null, ex);
        }
        }
        else
          JOptionPane.showMessageDialog(this,"Please select proper path");
    }//GEN-LAST:event_viewActionPerformed

    private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton1ActionPerformed
        if(file.getText().equals("")==false){
        jLabel3.setVisible(true);
        jLabel4.setVisible(true);
        jTextField1.setVisible(true);
        jTextField2.setVisible(true);
        search.setVisible(true);
        jButton2.setVisible(true);
        jButton3.setVisible(true);
        jButton4.setVisible(true);
        }
        else{
        JOptionPane.showMessageDialog(this,"Please select proper path");
        }
    }//GEN-LAST:event_jButton1ActionPerformed

    private void searchActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_searchActionPerformed
     if(file.getText().equals("")==false){
         jTextArea2.removeAll();
         if(jTextField1.getText().equals("")==true||jTextField1.getText().length()!=10){
             JOptionPane.showMessageDialog(this,"Please Enter proper seat no...");
             jTextField1.setText("");
         }
         else{
             jTextArea2.setVisible(true);
             jButton4.setVisible(true);
        try {
            PDDocument document = PDDocument.load(new File(filename));
            document.getClass();
            if (!document.isEncrypted())
            {
                PDFTextStripperByArea stripper = new PDFTextStripperByArea();
                stripper.setSortByPosition(true);
                PDFTextStripper Tstripper = new PDFTextStripper();
                String str = Tstripper.getText(document);
                Scanner scn = null;
                scn = new Scanner(str);
                String line="";
                jTextArea2.setText(line);
                int f=0,t=1;
                while(scn.hasNextLine()){
                    line = scn.nextLine();
                    if(line.startsWith(jTextField1.getText())==true&&f==0&&t<33){
                    String s="\n"+line;
                    jTextArea2.append(s);
                    f=1;
                    t++;
                    }
                    if((line.startsWith(" ")==true||line.endsWith(" ")==true)&&f==1&&t<33){
                    String s="\n"+line;
                    jTextArea2.append(s);
                    t++;
                    }
                    if(line.matches("(.*)SGPA(.*)")==true&&f==1&&t<33){
                    String s="\n"+line;
                    jTextArea2.append(s);
                    t++;                    
                    }
                }
            }
        } catch (IOException ex) {
            Logger.getLogger(Result.class.getName()).log(Level.SEVERE, null, ex);
        }
         }
     }
    
    }//GEN-LAST:event_searchActionPerformed

    private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton2ActionPerformed
      if(jTextField2.getText().equals("")==false){
          jTextArea2.setText("");
          jButton4.setVisible(true);
          try {
              PDDocument document = PDDocument.load(new File(filename));
              document.getClass();
              if (!document.isEncrypted()){
                  PDFTextStripperByArea stripper = new PDFTextStripperByArea();
                  stripper.setSortByPosition(true);
                  PDFTextStripper Tstripper = new PDFTextStripper();
                  String str = Tstripper.getText(document);
                  Scanner scn = null;
                  scn = new Scanner(str);
                  String line="";
                  jTextArea2.append(line);
                  int n=0,m=0,o=0;
                  while (scn.hasNextLine()){
                      line = scn.nextLine();
                      if(line.startsWith("   "+jTextField2.getText())==true&&line.matches("(.*)FF(.*)")==true){
                          n++;
                          m++;
                      }
                      else if(line.startsWith("   "+jTextField2.getText())==true){
                          m++;
                      }
                      if(line.matches("(.*)SGPA : --")==true){
                      o++;
                      }
                  }
                  String s="The No. of Student who give exam of subject code = "+jTextField2.getText()+" is "+m;
                  String f="The No. of Student who fails exam of Subject code = "+jTextField2.getText()+" is "+n;
                  String p="The No. of Student who Pass exam of Subject code = "+jTextField2.getText()+" is "+(m-n);
                  //String q="The No. of Student who clear Subject code = "+jTextField2.getText()+" is "+;
                  //String u="The No. of Student who has backlog for Subject code = "+jTextField2.getText()+" is "+o;
                  jTextArea2.append("\n"+s+"\n"+f+"\n"+p);
              }
          } catch (IOException ex) {
              Logger.getLogger(Result.class.getName()).log(Level.SEVERE, null, ex);
          }
         
      }
      else{
          JOptionPane.showMessageDialog(this,"Please enter subject code properly!");
      }
    }//GEN-LAST:event_jButton2ActionPerformed

    private void jButton3ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton3ActionPerformed
      jTextField1.setText("");
        jTextField2.setText("");  // TODO add your handling code here:
    }//GEN-LAST:event_jButton3ActionPerformed

    private void jButton4ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton4ActionPerformed
      MessageFormat header= new MessageFormat("Result");
        MessageFormat footer= new MessageFormat(" Page{0,number,integer} ");
        try{

            //jTextArea2.print(jTextArea2.PrintMode.FIT_WIDTH,header,footer);
              jTextArea2.print(header, footer);

        }catch(Exception e){
            JOptionPane.showMessageDialog(null, e);
        }

    }//GEN-LAST:event_jButton4ActionPerformed

    private void jButton5ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_jButton5ActionPerformed
        if(file.getText().equals("")==false){
           jTextArea2.setVisible(true);
        try{
            PDDocument document = PDDocument.load(new File(filename));
            document.getClass();
            int m=0,n=0;
            if (!document.isEncrypted()){
                  PDFTextStripperByArea stripper = new PDFTextStripperByArea();
                  stripper.setSortByPosition(true);
                  PDFTextStripper Tstripper = new PDFTextStripper();
                  String str = Tstripper.getText(document);
                  Scanner scn = null;
                  scn = new Scanner(str);
                  String line="";
                  jTextArea2.setText(line);
                  while(scn.hasNextLine()){
                      line=scn.nextLine();
                      if(line.matches("(.*)SGPA : --(.*)")==true)
                          m++;
                      if(line.matches("(.*)SGPA(.*)")==true)
                      n++;
                  }
            }
            String l="The no of student are All clear are = "+(n-m);
            String k="The no of students who has backlog are = "+m;
            jTextArea2.append("\n"+l+"\n"+k);
        } catch (IOException ex) {
            Logger.getLogger(Result.class.getName()).log(Level.SEVERE, null, ex);
        }
        }
        else{
            JOptionPane.showMessageDialog(this,"Please select proper file");
        }
    }//GEN-LAST:event_jButton5ActionPerformed

    /**
     * @param args the command line arguments
     */
    public static void main(String args[]) {
        /* Set the Nimbus look and feel */
        //<editor-fold defaultstate="collapsed" desc=" Look and feel setting code (optional) ">
        /* If Nimbus (introduced in Java SE 6) is not available, stay with the default look and feel.
         * For details see http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html 
         */
        try {
            for (javax.swing.UIManager.LookAndFeelInfo info : javax.swing.UIManager.getInstalledLookAndFeels()) {
                if ("Nimbus".equals(info.getName())) {
                    javax.swing.UIManager.setLookAndFeel(info.getClassName());
                    break;
                }
            }
        } catch (ClassNotFoundException ex) {
            java.util.logging.Logger.getLogger(Result.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(Result.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(Result.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(Result.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        //</editor-fold>

        /* Create and display the form */
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new Result().setVisible(true);
            }
        });
    }

    // Variables declaration - do not modify//GEN-BEGIN:variables
    private javax.swing.JButton Choose;
    private javax.swing.JTextField file;
    private javax.swing.JButton jButton1;
    private javax.swing.JButton jButton2;
    private javax.swing.JButton jButton3;
    private javax.swing.JButton jButton4;
    private javax.swing.JButton jButton5;
    private javax.swing.JLabel jLabel1;
    private javax.swing.JLabel jLabel2;
    private javax.swing.JLabel jLabel3;
    private javax.swing.JLabel jLabel4;
    private javax.swing.JPanel jPanel1;
    private javax.swing.JScrollPane jScrollPane1;
    private javax.swing.JScrollPane jScrollPane2;
    private javax.swing.JTextArea jTextArea1;
    private javax.swing.JTextArea jTextArea2;
    private javax.swing.JTextField jTextField1;
    private javax.swing.JTextField jTextField2;
    private javax.swing.JButton search;
    private javax.swing.JButton view;
    // End of variables declaration//GEN-END:variables
}
