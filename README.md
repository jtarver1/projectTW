# projectTW

ProjectTW is a group project that I did last year in Dr. Arup Ghosh's CS232 class. The course material for the class was the fundamentals of Java.
In the group project, the goal was to create a graphical user interface that would educate students about safety whilst gaming online.

The first file we had to make was a tester file. The file was titled G3Tester. The package folder that it and Section3.java would be in is Group3Project.
The actual code for this file is small and only includes a main function, an implimentation of the Section3 file, and a Menu() call.

Sectiion3 is where the bulk of our code is at. At the very top after the package, all of our libraries are added. 
They include: java.util.Scanner, java.io.File, java.io.FileNotFoundException, java.util.Arrays, and java.util.Random.
As a warning, some of the comments in this project were tests at one point, and should not be taken too seriously.

Our first implimentation of the aforementioned libraries is Scanner. It will be used to read the user's inputs while they are using the GUI.
The prompt when the GUI starts says "What topic on Online Gaming Safety would you like to access? 1)Introduction 2)Risks 3)Prevention 4)Quiz 5)Resources 0)Exit Module".
Once a number is selected, the program will tell the user their choice unless they put in an invalid input. In this case, it will prompt the user "Please enter a single digit that corresponds to one of the choices...", and then redirect back to the start of the program. 
All of this is encoded in a switch, with each section corresponding to all of the cases in the switch.

The next section is for the quiz. NumQ is a placeholder for the number of questions which is 10. Score is a variable that keeps track of how many questions the user gets correct.
The user is prompted with "Welcome to the quiz! Please answer 10 questions on Online Gaming Safety...". A for loop is printing the questions until the number of questions reaches 10.
Once the quiz is finished, the score that the user made is printed for them to see.

If INTRO is selected by the user they are givent the following message. 
INTRODUCTION TO ONLINE GAMING SAFETY
        "In this project we will be discussing the importance of safe online gaming.
        What is online gaming? Online gaming describes any video game that offers online interactions with other players.
        Although, online gaming may be enjoyable. There are potential risk factors that you should be aware of.
       To learn more about these risk and how to prevent them.
       Continue with this program that was specifally designed to inform you on how to safely online game."
       
If RISK is selected then they are given the following message.
 "While online gaming can be a fun way to have fun and pass time for the casual user, what most people new to the scene wouldn't expect is losing their data. Your personal information could be at risk, credit cards, personal info, location and potentially more.
      "There are many different risks related to the online gaming scene, these risks will be refered to as 'attacks' due to their malicious nature to the user. Today we will cover 4, Phishing, Doxxing, DDosing, and cyber bullying.
      There are many different types of attacks but these are some of the main types:
      The first and simplest methods is the 'phishing' method, and the reason it's called that is due to the nature of the attack. The attack is conducted through social engineering and the effectiveness of the attack is determined by the victims awareness.
      The attack could range from forward asking for information or 'baiting' the user into giving them a back door to access their information, whether it be through links or social engineering.
    The next attack is more identity risk focused, this attack is called doxxing. If a hacker manages to infiltrate your account, whether it be from a hack or a phishing scam, they can gain access to your information such as name, location, birth date, passwords, payment info, and much more.
      Doxxing attacks will usually involve spreading this information to either more hackers, or people willing to buy information to commit identity theft or online robbery.
      The method used to directly take you out of the equation is the DDosing attack. This attack involves a user obtaining your IP or net address to attack your internet router. This can cause outages to your internet system, often for long periods of time.
      These attacks can be automated or done manually if the proper safety methods aren't incorporated properly.
      For the last attack, we'll be disscussing one that requires no code what so ever, cyberbullying. While it may require no coding it is still a malicious attack in the online gaming world. Cyber bullying hurts the user more than any digital data, leading to depression, anxiety and more".

If RESOURCES is selected then the user gets the following links.
        "https://www.kaspersky.com/resource-center/threats/top-10-online-gaming-risks"
        "https://www.ncsc.gov.uk/guidance/phishing"
        "https://www.cloudflare.com/learning/ddos/what-is-a-ddos-attack/"
       "https://www.kaspersky.com/resource-center/definitions/what-is-doxing"
        "https://www.unicef.org/end-violence/how-to-stop-cyberbullying"

If PREVENTION is selecting they are given the following message.
"While there are some dangers in online gaming, there are many ways to stay safe!
        Use strong passwords, alternative usernames, and a seperate email to prevent your other accounts from being hacked in the event of a breach. 
        Be cautious when browsing gaming websites and be careful when downloading content, be sure to use only official webpages and use an antivirus when possible. Be sure to avoid pirating or torrenting games, as these websites are often used to hack and phish for information as well.
        When chat is available in a multiplayer game, exercise your internet safety. Be sure to NEVER reveal any personal information, no matter what.
        Use your payment information only on secure interfaces, or attempt to use a throw away prepaid card when possible to avoid your banking information from getting stolen.
        If you ever feel uncomfortable with another player online, block them! Also remember to report any players who might be hacking or phishing for information int he game. 

The remainder of the class is the coding for randomized quiz.
An array of strings is created, followed by a try-catch. In the try-catch it reads the G3Questions file line by line and stops reading if there are any errors.
  The next lines of code finish the creations of the arrays for the randomizer to use.
The randomizer reads the arrays that were generated and works with the quiz coding back toward the beginning of the class to print the questions that it chooses.
It also eliminates the possibility of generating a duplicate question in the quiz.
The quizify method at the end of the class determines the correct answer for the question that the answer corresponds to and prints the reult to the user. The correct answer for each question is listed at the beginning of each question in the G3Questions file but is invisible to the user. Quizify reads that first character in each line as the correct answer to the question.
