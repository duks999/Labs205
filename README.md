# Labs205
Labs205
Form1.cs
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Coronovirus
{
    public partial class Form1 : Form
    {
        double bufer;
        double bufer1;
        bool plus = false;
        bool minuse = false;
        bool del = false;
        bool umnoj = false;
        double pasent;
        string TexBox;
        bool Zap = true;
        bool noll = true;
        double bufer3;
        bool TTT = true; 
        
        public Form1()
        {
            InitializeComponent();
        }

        private void button18_Click(object sender, EventArgs e)
        {
            if (noll == true)
            {
                textBox1.Text = null;
                textBox1.Text += "5";
                noll = false;
            }
            else
                textBox1.Text += "5";
        }

        private void button1_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0")
            {
                
                textBox1.Text = "0";
                
            }
            else
                textBox1.Text += "0";



        }

        private void button5_Click(object sender, EventArgs e)
        {
            if (noll == true)
            {
                textBox1.Text = null;
                textBox1.Text += "1";
                noll = false;
            }
            else
            textBox1.Text += "1";
        }

        private void button8_Click(object sender, EventArgs e)
        {
            if (noll == true)
            {
                textBox1.Text = null;
                textBox1.Text += "2";
                noll = false;
            }
            else
                textBox1.Text += "2";
        }

        private void Form1_Load(object sender, EventArgs e)
        {

        }

        private void button7_Click(object sender, EventArgs e)
        {
            if (noll == true)
            {
                textBox1.Text = null;
                textBox1.Text += "3";
                noll = false;
            }
            else
                textBox1.Text += "3";
        }

        private void button10_Click(object sender, EventArgs e)
        {
            if (noll == true)
            {
                textBox1.Text = null;
                textBox1.Text += "4";
                noll = false;
            }
            else
                textBox1.Text += "4";
        }

        private void button17_Click(object sender, EventArgs e)
        {
            if (noll == true)
            {
                textBox1.Text = null;
                textBox1.Text += "6";
                noll = false;
            }
            else
                textBox1.Text += "6";
        }

        private void button9_Click(object sender, EventArgs e)
        {
            if (noll == true)
            {
                textBox1.Text = null;
                textBox1.Text += "7";
                noll = false;
            }
            else
                textBox1.Text += "7";
        }

        private void button15_Click(object sender, EventArgs e)
        {
            if (noll == true)
            {
                textBox1.Text = null;
                textBox1.Text += "8";
                noll = false;
            }
            else
                textBox1.Text += "8";
        }

        private void button14_Click(object sender, EventArgs e)
        {
            if (noll == true)
            {
                textBox1.Text = null;
                textBox1.Text += "9";
                noll = false;
            }
            else
                textBox1.Text += "9";
        }

        private void button2_Click(object sender, EventArgs e)
        {
            textBox1.Text = null;
            textBox1.Text = "0";
            Zap = true;
            noll = true;
             plus = false;
             minuse = false;
             del = false;
             umnoj = false;
        }

        private void button6_Click(object sender, EventArgs e)
        {
            bufer = double.Parse(textBox1.Text);
            textBox1.Text = null;
            plus = true;

        }

        private void button4_Click(object sender, EventArgs e)
        {
           if (plus == true)
           {
                
                bufer1 = double.Parse(textBox1.Text);
                bufer1 = bufer1 + bufer;
                textBox1.Text = bufer1.ToString();
           }

            if (minuse == true)
            {
                if (TTT == true)
                bufer1 = double.Parse(textBox1.Text);
                bufer3 = bufer1;
                bufer = bufer - bufer3;
                textBox1.Text = bufer.ToString();
            }

            if (umnoj == true)
            {
                bufer1 = double.Parse(textBox1.Text);
                bufer1 = bufer1 * bufer;
                textBox1.Text = bufer1.ToString();
            }

            if (del == true)
            {
                bufer1 = double.Parse(textBox1.Text);
                bufer3 = bufer1;
                bufer = bufer / bufer3;
                textBox1.Text = bufer.ToString();
            }
        }

        private void button16_Click(object sender, EventArgs e)
        {
            bufer = double.Parse(textBox1.Text);
            textBox1.Text = null;
            minuse = true;
        }

        private void button13_Click(object sender, EventArgs e)
        {
            bufer = double.Parse(textBox1.Text);
            textBox1.Text = null;
            umnoj = true;
        }

        private void button19_Click(object sender, EventArgs e)
        {
            bufer = double.Parse(textBox1.Text);
            textBox1.Text = null;
            del = true;
        }

        private void button3_Click(object sender, EventArgs e)
        {
            if (Zap == true)
            {
                textBox1.Text += ",";
                Zap = false;
            }
            
            
 
        }

        private void button12_Click(object sender, EventArgs e)
        {
            pasent = double.Parse(textBox1.Text) / 100;
            textBox1.Text = pasent.ToString();
        }

        private void button1_MouseMove(object sender, MouseEventArgs e)
        {
            button1.BackColor = System.Drawing.Color.Brown;
        }

        private void button1_MouseLeave(object sender, EventArgs e)
        {
            button1.BackColor = System.Drawing.Color.Black;
        }

        private void button3_MouseMove(object sender, MouseEventArgs e)
        {
            button3.BackColor = System.Drawing.Color.Brown;
        }

        private void button3_MouseLeave(object sender, EventArgs e)
        {
            button3.BackColor = System.Drawing.Color.Black;
        }

        private void button4_MouseMove(object sender, MouseEventArgs e)
        {
            button4.BackColor = System.Drawing.Color.Brown;
        }

        private void button6_MouseMove(object sender, MouseEventArgs e)
        {
            button6.BackColor = System.Drawing.Color.Brown;
        }

        private void button7_MouseMove(object sender, MouseEventArgs e)
        {
            button7.BackColor = System.Drawing.Color.Brown;
        }

        private void button8_MouseMove(object sender, MouseEventArgs e)
        {
            button8.BackColor = System.Drawing.Color.Brown;
        }

        private void button5_MouseMove(object sender, MouseEventArgs e)
        {
            button5.BackColor = System.Drawing.Color.Brown;
        }

        private void button10_MouseMove(object sender, MouseEventArgs e)
        {
            button10.BackColor = System.Drawing.Color.Brown;
        }

        private void button18_MouseMove(object sender, MouseEventArgs e)
        {
            button18.BackColor = System.Drawing.Color.Brown;
        }

        private void button17_MouseMove(object sender, MouseEventArgs e)
        {
            button17.BackColor = System.Drawing.Color.Brown;
        }

        private void button16_MouseMove(object sender, MouseEventArgs e)
        {
            button16.BackColor = System.Drawing.Color.Brown;
        }

        private void button9_MouseMove(object sender, MouseEventArgs e)
        {
            button9.BackColor = System.Drawing.Color.Brown;
        }

        private void button15_MouseMove(object sender, MouseEventArgs e)
        {
            button15.BackColor = System.Drawing.Color.Brown;
        }

        private void button14_MouseMove(object sender, MouseEventArgs e)
        {
            button14.BackColor = System.Drawing.Color.Brown;
        }

        private void button13_MouseMove(object sender, MouseEventArgs e)
        {
            button13.BackColor = System.Drawing.Color.Brown;
        }

        private void button2_MouseMove(object sender, MouseEventArgs e)
        {
            button2.BackColor = System.Drawing.Color.Brown;
        }

        private void button11_MouseMove(object sender, MouseEventArgs e)
        {
            button11.BackColor = System.Drawing.Color.Brown;
        }

        private void button12_MouseMove(object sender, MouseEventArgs e)
        {
            button12.BackColor = System.Drawing.Color.Brown;
        }

        private void button19_MouseMove(object sender, MouseEventArgs e)
        {
            button19.BackColor = System.Drawing.Color.Brown;
        }

        private void button4_MouseLeave(object sender, EventArgs e)
        {
            button4.BackColor = System.Drawing.Color.Black;
        }

        private void button6_MouseLeave(object sender, EventArgs e)
        {
            button6.BackColor = System.Drawing.Color.Black;
        }

        private void button7_MouseLeave(object sender, EventArgs e)
        {
            button7.BackColor = System.Drawing.Color.Black;
        }

        private void button8_MouseLeave(object sender, EventArgs e)
        {
            button8.BackColor = System.Drawing.Color.Black;
        }

        private void button5_MouseLeave(object sender, EventArgs e)
        {
            button5.BackColor = System.Drawing.Color.Black;
        }

        private void button16_MouseLeave(object sender, EventArgs e)
        {
            button16.BackColor = System.Drawing.Color.Black;
        }

        private void button17_MouseLeave(object sender, EventArgs e)
        {
            button17.BackColor = System.Drawing.Color.Black;
        }

        private void button18_MouseLeave(object sender, EventArgs e)
        {
            button18.BackColor = System.Drawing.Color.Black;
        }

        private void button10_MouseLeave(object sender, EventArgs e)
        {
            button10.BackColor = System.Drawing.Color.Black;
        }

        private void button13_MouseLeave(object sender, EventArgs e)
        {
            button13.BackColor = System.Drawing.Color.Black;
        }

        private void button14_MouseLeave(object sender, EventArgs e)
        {
            button14.BackColor = System.Drawing.Color.Black;
        }

        private void button15_MouseLeave(object sender, EventArgs e)
        {
            button15.BackColor = System.Drawing.Color.Black;
        }

        private void button9_MouseLeave(object sender, EventArgs e)
        {
            button9.BackColor = System.Drawing.Color.Black;
        }

        private void button19_MouseLeave(object sender, EventArgs e)
        {
            button19.BackColor = System.Drawing.Color.Black;
        }

        private void button12_MouseLeave(object sender, EventArgs e)
        {
            button12.BackColor = System.Drawing.Color.Black;
        }

        private void button11_MouseLeave(object sender, EventArgs e)
        {
            button11.BackColor = System.Drawing.Color.Black;
        }

        private void button2_MouseLeave(object sender, EventArgs e)
        {
            button2.BackColor = System.Drawing.Color.Black;
        }

        private void button11_Click(object sender, EventArgs e)
        {
            TexBox = textBox1.Text;
            TexBox = TexBox.Insert(0, "-");
            textBox1.Text = TexBox;
        }
        private void textBox1_TextChanged(object sender, EventArgs e)
        {

        }
    }
}



Form1.Desinger.cs
namespace Coronovirus
{
    partial class Form1
    {
        /// <summary>
        /// Обязательная переменная конструктора.
        /// </summary>
        private System.ComponentModel.IContainer components = null;

        /// <summary>
        /// Освободить все используемые ресурсы.
        /// </summary>
        /// <param name="disposing">истинно, если управляемый ресурс должен быть удален; иначе ложно.</param>
        protected override void Dispose(bool disposing)
        {
            if (disposing && (components != null))
            {
                components.Dispose();
            }
            base.Dispose(disposing);
        }

        #region Код, автоматически созданный конструктором форм Windows

        /// <summary>
        /// Требуемый метод для поддержки конструктора — не изменяйте 
        /// содержимое этого метода с помощью редактора кода.
        /// </summary>
        private void InitializeComponent()
        {
            this.button1 = new System.Windows.Forms.Button();
            this.button3 = new System.Windows.Forms.Button();
            this.button4 = new System.Windows.Forms.Button();
            this.button5 = new System.Windows.Forms.Button();
            this.button6 = new System.Windows.Forms.Button();
            this.button7 = new System.Windows.Forms.Button();
            this.button8 = new System.Windows.Forms.Button();
            this.button2 = new System.Windows.Forms.Button();
            this.button9 = new System.Windows.Forms.Button();
            this.button10 = new System.Windows.Forms.Button();
            this.button11 = new System.Windows.Forms.Button();
            this.button12 = new System.Windows.Forms.Button();
            this.button13 = new System.Windows.Forms.Button();
            this.button14 = new System.Windows.Forms.Button();
            this.button15 = new System.Windows.Forms.Button();
            this.button16 = new System.Windows.Forms.Button();
            this.button17 = new System.Windows.Forms.Button();
            this.button18 = new System.Windows.Forms.Button();
            this.button19 = new System.Windows.Forms.Button();
            this.textBox1 = new System.Windows.Forms.TextBox();
            this.SuspendLayout();
            // 
            // button1
            // 
            this.button1.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button1.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button1.ForeColor = System.Drawing.SystemColors.Control;
            this.button1.ImageAlign = System.Drawing.ContentAlignment.MiddleLeft;
            this.button1.Location = new System.Drawing.Point(12, 500);
            this.button1.Name = "button1";
            this.button1.Size = new System.Drawing.Size(156, 68);
            this.button1.TabIndex = 0;
            this.button1.Text = "0";
            this.button1.TextAlign = System.Drawing.ContentAlignment.MiddleLeft;
            this.button1.UseVisualStyleBackColor = false;
            this.button1.Click += new System.EventHandler(this.button1_Click);
            this.button1.MouseLeave += new System.EventHandler(this.button1_MouseLeave);
            this.button1.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button1_MouseMove);
            // 
            // button3
            // 
            this.button3.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button3.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button3.ForeColor = System.Drawing.SystemColors.Control;
            this.button3.Location = new System.Drawing.Point(204, 500);
            this.button3.Name = "button3";
            this.button3.Size = new System.Drawing.Size(60, 68);
            this.button3.TabIndex = 2;
            this.button3.Text = ",";
            this.button3.UseVisualStyleBackColor = false;
            this.button3.Click += new System.EventHandler(this.button3_Click);
            this.button3.MouseLeave += new System.EventHandler(this.button3_MouseLeave);
            this.button3.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button3_MouseMove);
            // 
            // button4
            // 
            this.button4.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button4.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button4.ForeColor = System.Drawing.SystemColors.Control;
            this.button4.Location = new System.Drawing.Point(300, 500);
            this.button4.Name = "button4";
            this.button4.Size = new System.Drawing.Size(60, 68);
            this.button4.TabIndex = 3;
            this.button4.Text = "=";
            this.button4.UseVisualStyleBackColor = false;
            this.button4.Click += new System.EventHandler(this.button4_Click);
            this.button4.MouseLeave += new System.EventHandler(this.button4_MouseLeave);
            this.button4.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button4_MouseMove);
            // 
            // button5
            // 
            this.button5.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button5.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button5.ForeColor = System.Drawing.SystemColors.Control;
            this.button5.Location = new System.Drawing.Point(12, 414);
            this.button5.Name = "button5";
            this.button5.Size = new System.Drawing.Size(60, 60);
            this.button5.TabIndex = 4;
            this.button5.Text = "1";
            this.button5.UseVisualStyleBackColor = false;
            this.button5.Click += new System.EventHandler(this.button5_Click);
            this.button5.MouseLeave += new System.EventHandler(this.button5_MouseLeave);
            this.button5.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button5_MouseMove);
            // 
            // button6
            // 
            this.button6.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button6.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button6.ForeColor = System.Drawing.SystemColors.Control;
            this.button6.Location = new System.Drawing.Point(300, 414);
            this.button6.Name = "button6";
            this.button6.Size = new System.Drawing.Size(60, 60);
            this.button6.TabIndex = 5;
            this.button6.Text = "+";
            this.button6.UseVisualStyleBackColor = false;
            this.button6.Click += new System.EventHandler(this.button6_Click);
            this.button6.MouseLeave += new System.EventHandler(this.button6_MouseLeave);
            this.button6.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button6_MouseMove);
            // 
            // button7
            // 
            this.button7.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button7.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button7.ForeColor = System.Drawing.SystemColors.Control;
            this.button7.Location = new System.Drawing.Point(204, 414);
            this.button7.Name = "button7";
            this.button7.Size = new System.Drawing.Size(60, 60);
            this.button7.TabIndex = 6;
            this.button7.Text = "3";
            this.button7.UseVisualStyleBackColor = false;
            this.button7.Click += new System.EventHandler(this.button7_Click);
            this.button7.MouseLeave += new System.EventHandler(this.button7_MouseLeave);
            this.button7.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button7_MouseMove);
            // 
            // button8
            // 
            this.button8.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button8.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button8.ForeColor = System.Drawing.SystemColors.Control;
            this.button8.Location = new System.Drawing.Point(108, 414);
            this.button8.Name = "button8";
            this.button8.Size = new System.Drawing.Size(60, 60);
            this.button8.TabIndex = 7;
            this.button8.Text = "2";
            this.button8.UseVisualStyleBackColor = false;
            this.button8.Click += new System.EventHandler(this.button8_Click);
            this.button8.MouseLeave += new System.EventHandler(this.button8_MouseLeave);
            this.button8.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button8_MouseMove);
            // 
            // button2
            // 
            this.button2.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button2.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button2.ForeColor = System.Drawing.SystemColors.Control;
            this.button2.Location = new System.Drawing.Point(12, 156);
            this.button2.Name = "button2";
            this.button2.Size = new System.Drawing.Size(60, 60);
            this.button2.TabIndex = 8;
            this.button2.Text = "C";
            this.button2.UseVisualStyleBackColor = false;
            this.button2.Click += new System.EventHandler(this.button2_Click);
            this.button2.MouseLeave += new System.EventHandler(this.button2_MouseLeave);
            this.button2.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button2_MouseMove);
            // 
            // button9
            // 
            this.button9.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button9.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button9.ForeColor = System.Drawing.SystemColors.Control;
            this.button9.Location = new System.Drawing.Point(12, 242);
            this.button9.Name = "button9";
            this.button9.Size = new System.Drawing.Size(60, 60);
            this.button9.TabIndex = 9;
            this.button9.Text = "7";
            this.button9.UseVisualStyleBackColor = false;
            this.button9.Click += new System.EventHandler(this.button9_Click);
            this.button9.MouseLeave += new System.EventHandler(this.button9_MouseLeave);
            this.button9.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button9_MouseMove);
            // 
            // button10
            // 
            this.button10.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button10.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button10.ForeColor = System.Drawing.SystemColors.Control;
            this.button10.Location = new System.Drawing.Point(12, 328);
            this.button10.Name = "button10";
            this.button10.Size = new System.Drawing.Size(60, 60);
            this.button10.TabIndex = 10;
            this.button10.Text = "4";
            this.button10.UseVisualStyleBackColor = false;
            this.button10.Click += new System.EventHandler(this.button10_Click);
            this.button10.MouseLeave += new System.EventHandler(this.button10_MouseLeave);
            this.button10.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button10_MouseMove);
            // 
            // button11
            // 
            this.button11.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button11.Font = new System.Drawing.Font("Microsoft Sans Serif", 20F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button11.ForeColor = System.Drawing.SystemColors.Control;
            this.button11.Location = new System.Drawing.Point(108, 156);
            this.button11.Name = "button11";
            this.button11.Size = new System.Drawing.Size(60, 60);
            this.button11.TabIndex = 11;
            this.button11.Text = "+/-";
            this.button11.UseVisualStyleBackColor = false;
            this.button11.Click += new System.EventHandler(this.button11_Click);
            this.button11.MouseLeave += new System.EventHandler(this.button11_MouseLeave);
            this.button11.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button11_MouseMove);
            // 
            // button12
            // 
            this.button12.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button12.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button12.ForeColor = System.Drawing.SystemColors.Control;
            this.button12.Location = new System.Drawing.Point(204, 156);
            this.button12.Name = "button12";
            this.button12.Size = new System.Drawing.Size(60, 60);
            this.button12.TabIndex = 12;
            this.button12.Text = "%";
            this.button12.UseVisualStyleBackColor = false;
            this.button12.Click += new System.EventHandler(this.button12_Click);
            this.button12.MouseLeave += new System.EventHandler(this.button12_MouseLeave);
            this.button12.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button12_MouseMove);
            // 
            // button13
            // 
            this.button13.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button13.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button13.ForeColor = System.Drawing.SystemColors.Control;
            this.button13.Location = new System.Drawing.Point(300, 242);
            this.button13.Name = "button13";
            this.button13.Size = new System.Drawing.Size(60, 60);
            this.button13.TabIndex = 13;
            this.button13.Text = "X";
            this.button13.UseVisualStyleBackColor = false;
            this.button13.Click += new System.EventHandler(this.button13_Click);
            this.button13.MouseLeave += new System.EventHandler(this.button13_MouseLeave);
            this.button13.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button13_MouseMove);
            // 
            // button14
            // 
            this.button14.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button14.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button14.ForeColor = System.Drawing.SystemColors.Control;
            this.button14.Location = new System.Drawing.Point(204, 242);
            this.button14.Name = "button14";
            this.button14.Size = new System.Drawing.Size(60, 60);
            this.button14.TabIndex = 14;
            this.button14.Text = "9";
            this.button14.UseVisualStyleBackColor = false;
            this.button14.Click += new System.EventHandler(this.button14_Click);
            this.button14.MouseLeave += new System.EventHandler(this.button14_MouseLeave);
            this.button14.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button14_MouseMove);
            // 
            // button15
            // 
            this.button15.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button15.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button15.ForeColor = System.Drawing.SystemColors.Control;
            this.button15.Location = new System.Drawing.Point(108, 242);
            this.button15.Name = "button15";
            this.button15.Size = new System.Drawing.Size(60, 60);
            this.button15.TabIndex = 15;
            this.button15.Text = "8";
            this.button15.UseVisualStyleBackColor = false;
            this.button15.Click += new System.EventHandler(this.button15_Click);
            this.button15.MouseLeave += new System.EventHandler(this.button15_MouseLeave);
            this.button15.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button15_MouseMove);
            // 
            // button16
            // 
            this.button16.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button16.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button16.ForeColor = System.Drawing.SystemColors.Control;
            this.button16.Location = new System.Drawing.Point(300, 328);
            this.button16.Name = "button16";
            this.button16.Size = new System.Drawing.Size(60, 60);
            this.button16.TabIndex = 16;
            this.button16.Text = "-";
            this.button16.UseVisualStyleBackColor = false;
            this.button16.Click += new System.EventHandler(this.button16_Click);
            this.button16.MouseLeave += new System.EventHandler(this.button16_MouseLeave);
            this.button16.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button16_MouseMove);
            // 
            // button17
            // 
            this.button17.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button17.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button17.ForeColor = System.Drawing.SystemColors.Control;
            this.button17.Location = new System.Drawing.Point(204, 328);
            this.button17.Name = "button17";
            this.button17.Size = new System.Drawing.Size(60, 60);
            this.button17.TabIndex = 17;
            this.button17.Text = "6";
            this.button17.UseVisualStyleBackColor = false;
            this.button17.Click += new System.EventHandler(this.button17_Click);
            this.button17.MouseLeave += new System.EventHandler(this.button17_MouseLeave);
            this.button17.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button17_MouseMove);
            // 
            // button18
            // 
            this.button18.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button18.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button18.ForeColor = System.Drawing.SystemColors.Control;
            this.button18.Location = new System.Drawing.Point(108, 328);
            this.button18.Name = "button18";
            this.button18.Size = new System.Drawing.Size(60, 60);
            this.button18.TabIndex = 18;
            this.button18.Text = "5";
            this.button18.UseVisualStyleBackColor = false;
            this.button18.Click += new System.EventHandler(this.button18_Click);
            this.button18.MouseLeave += new System.EventHandler(this.button18_MouseLeave);
            this.button18.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button18_MouseMove);
            // 
            // button19
            // 
            this.button19.BackColor = System.Drawing.SystemColors.ActiveCaptionText;
            this.button19.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.button19.ForeColor = System.Drawing.SystemColors.Control;
            this.button19.Location = new System.Drawing.Point(300, 156);
            this.button19.Name = "button19";
            this.button19.Size = new System.Drawing.Size(60, 60);
            this.button19.TabIndex = 19;
            this.button19.Text = "/";
            this.button19.UseVisualStyleBackColor = false;
            this.button19.Click += new System.EventHandler(this.button19_Click);
            this.button19.MouseLeave += new System.EventHandler(this.button19_MouseLeave);
            this.button19.MouseMove += new System.Windows.Forms.MouseEventHandler(this.button19_MouseMove);
            // 
            // textBox1
            // 
            this.textBox1.Enabled = false;
            this.textBox1.Font = new System.Drawing.Font("Microsoft Sans Serif", 40F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(204)));
            this.textBox1.Location = new System.Drawing.Point(12, 54);
            this.textBox1.Multiline = true;
            this.textBox1.Name = "textBox1";
            this.textBox1.Size = new System.Drawing.Size(348, 76);
            this.textBox1.TabIndex = 20;
            this.textBox1.Text = "0";
            this.textBox1.TextAlign = System.Windows.Forms.HorizontalAlignment.Right;
            this.textBox1.TextChanged += new System.EventHandler(this.textBox1_TextChanged);
            // 
            // Form1
            // 
            this.AutoScaleDimensions = new System.Drawing.SizeF(6F, 13F);
            this.AutoScaleMode = System.Windows.Forms.AutoScaleMode.Font;
            this.ClientSize = new System.Drawing.Size(372, 572);
            this.Controls.Add(this.textBox1);
            this.Controls.Add(this.button19);
            this.Controls.Add(this.button18);
            this.Controls.Add(this.button17);
            this.Controls.Add(this.button16);
            this.Controls.Add(this.button15);
            this.Controls.Add(this.button14);
            this.Controls.Add(this.button13);
            this.Controls.Add(this.button12);
            this.Controls.Add(this.button11);
            this.Controls.Add(this.button10);
            this.Controls.Add(this.button9);
            this.Controls.Add(this.button2);
            this.Controls.Add(this.button8);
            this.Controls.Add(this.button7);
            this.Controls.Add(this.button6);
            this.Controls.Add(this.button5);
            this.Controls.Add(this.button4);
            this.Controls.Add(this.button3);
            this.Controls.Add(this.button1);
            this.Name = "Form1";
            this.Text = "Form1";
            this.Load += new System.EventHandler(this.Form1_Load);
            this.ResumeLayout(false);
            this.PerformLayout();

        }

        #endregion

        private System.Windows.Forms.Button button1;
        private System.Windows.Forms.Button button3;
        private System.Windows.Forms.Button button4;
        private System.Windows.Forms.Button button5;
        private System.Windows.Forms.Button button6;
        private System.Windows.Forms.Button button7;
        private System.Windows.Forms.Button button8;
        private System.Windows.Forms.Button button2;
        private System.Windows.Forms.Button button9;
        private System.Windows.Forms.Button button10;
        private System.Windows.Forms.Button button11;
        private System.Windows.Forms.Button button12;
        private System.Windows.Forms.Button button13;
        private System.Windows.Forms.Button button14;
        private System.Windows.Forms.Button button15;
        private System.Windows.Forms.Button button16;
        private System.Windows.Forms.Button button17;
        private System.Windows.Forms.Button button18;
        private System.Windows.Forms.Button button19;
        private System.Windows.Forms.TextBox textBox1;
    }
}

