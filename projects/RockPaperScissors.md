---
layout: project
type: project
title: "RockPaperScissors"
date: 2021
published: true
labels:
  - Game
  - Quick
  - C#
summary: "I developed a quick RockPaperScissors game based on instructions from a tecxt box for my class."
---
namespace Rock_Paper_Scissors
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }
        class program
        {
            static void Main(string[] args)
            {
                int a;
                string player;
                string CPU;
                Random Num = new Random();
                a = Num.Next(1,4);
                switch (a)
                {
                    case 1:
                    CPU = "ROCK";
                    break;
                    case 2:
                    CPU = "PAPER";
                    break;
                    case 3:
                    CPU = "SCISSORS";
                    break;
                    default:
                    CPU = "MR";
                    break;
                }
                Console.WriteLine("Enter your Input");
                player = Console.ReadLine();
                string player01 = player.ToUpper();
                Console.WriteLine("The computer chose " + CPU);
                Console.WriteLine("The player chose " +player01);
               
                if (player01 == "Rock")
                    if (CPU == "Rock") 
                Console.WriteLine("TIE");

                if (CPU == "Paper")
                    Console.WriteLine("You Lose");

                if (CPU == "Scissors")
                    Console.WriteLine("You Win");

                if (player01 == "Scissors")
                    if (CPU == "Rock")
                        Console.WriteLine("You Lose");

                if (CPU == "Paper")
                    Console.WriteLine("You Win");

                if (CPU == "Scissors")
                    Console.WriteLine("You Tie");

                if (player01 == "Paper")
                    if (CPU == "Rock")
                        Console.WriteLine("You Win");

                if (CPU == "Paper")
                    Console.WriteLine("Tie");

                if (CPU == "Scissors")
                    Console.WriteLine("You Lose");
            }
        }
    }
}
