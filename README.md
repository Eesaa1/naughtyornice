namespace WindowsFormsApp1
{
    public partial class Form1 : Form
    {
        int Score = 0;


        public Form1()
        {
            InitializeComponent();

        }

        private void textBox1_TextChanged(object sender, EventArgs e)
        {



        }

        private void label1_Click(object sender, EventArgs e)
        {

        }

        private void label6_Click(object sender, EventArgs e)
        {

        }

        /* Check lists */
        private void checkBox1_CheckedChanged(object sender, EventArgs e)
        {
            if (checkBox1.Checked == true)
            {
                Score++;
            }
        }
        private void checkBox3_CheckedChanged(object sender, EventArgs e)
        {
            if (checkBox3.Checked == true)
            {
                Score++;
            }
        }
        private void checkBox6_CheckedChanged(object sender, EventArgs e)
        {
            if (checkBox6.Checked == true)
            {
                Score++;
            }
        }
        private void checkBox8_CheckedChanged(object sender, EventArgs e)
        {
            if (checkBox8.Checked == true)
            {
                Score++;
            }
        }

        /* Cards */
        private void textBox2_TextChanged(object sender, EventArgs e)
        {
            int i = Convert.ToInt32(textBox2.Text);
            if (i > 1)
            {
                Score = Score + 2;
            }
            else if (i > 0)
            {
                Score++;
            }

        }
        /* Name */
        private void textBox1_TextChanged_1(object sender, EventArgs e)
        {
            string Name = textBox1.Text;
        }
        /* Naughty or nice */
        private void button1_Click(object sender, EventArgs e)

        {
            if (Score > 4)
            {

                MessageBox.Show("Well done {0} you have been a good boy/girl this year!", Name);
                MessageBox.Show(Convert.ToString(Score));
            }
            else
            {
                MessageBox.Show("Unfortunately {0} you have been naughty this year, better luck next year!", Name);
                MessageBox.Show(Convert.ToString(Score));
            }
        }


    }
}
