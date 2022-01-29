        private bool czyjRuch = true;

        private void WstawZnak(object przycisk)
        {

        }

        private void WlaczPrzyciskiIResetuj()
        {
            button1.Enabled = true;
            button2.Enabled = true;
            button3.Enabled = true;
            button4.Enabled = true;
            button5.Enabled = true;
            button6.Enabled = true;
            button7.Enabled = true;
            button8.Enabled = true;
            button9.Enabled = true;
            button1.Text = "";
            button2.Text = "";
            button3.Text = "";
            button4.Text = "";
            button5.Text = "";
            button6.Text = "";
            button7.Text = "";
            button8.Text = "";
            button9.Text = "";
        }

        private void WylaczPrzyciski()
        {
            button1.Enabled = false;
            button2.Enabled = false;
            button3.Enabled = false;
            button4.Enabled = false;
            button5.Enabled = false;
            button6.Enabled = false;
            button7.Enabled = false;
            button8.Enabled = false;
            button9.Enabled = false;
        }

        private bool SprawdzCzyKtosWygral()
        {
            if (button1.Text == button2.Text && button2.Text == button3.Text && button1.Text != "")
                return true;
            else if (button4.Text == button5.Text && button5.Text == button6.Text && button4.Text != "")
                return true;
            else if (button7.Text == button8.Text && button8.Text == button9.Text && button9.Text != "")
                return true;
            else if (button1.Text == button4.Text && button4.Text == button7.Text && button1.Text != "")
                return true;
            else if (button2.Text == button5.Text && button5.Text == button8.Text && button5.Text != "")
                return true;
            else if (button3.Text == button6.Text && button6.Text == button9.Text && button9.Text != "")
                return true;
            else if (button1.Text == button5.Text && button5.Text == button9.Text && button9.Text != "")
                return true;
            else if (button3.Text == button5.Text && button5.Text == button7.Text && button3.Text != "")
                return true;
            else
                return false;
        }
