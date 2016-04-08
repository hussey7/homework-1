# homework-1
#Playing Over The Wire Bandit

The goal of playing this game was to learn Linux commands. Cygwin Terminal was used to play this game as since I was using a Windows OS. 

#Level 0

To start the game, I logged into the game using this command.
>$ ssh bandit0@bandit.labs.overthewire.org

![image](https://cloud.githubusercontent.com/assets/12781941/14386150/3d9fcd9a-fdc1-11e5-89dd-15bbd177bf1c.png)

#Level 0 -> Level 1

The below command was used to find the password to access Level 1.

> cat readme 

![image](https://cloud.githubusercontent.com/assets/12781941/14386175/61ddc2a2-fdc1-11e5-8eae-00bc1e119545.png)

#Level 1 -> Level 2

The below command was used to find the password to access Level 2 as it was in a file called -.

> cat ./-

![image](https://cloud.githubusercontent.com/assets/12781941/14386190/6e34444a-fdc1-11e5-8c23-4dc6d75afc7c.png)

#Level 2 -> Level 3

The below command was used to find the password to access Level 3 as it was in a file called spaces in this filename.

> cat spaces\ in\ this\ filename

![image](https://cloud.githubusercontent.com/assets/12781941/14386196/72455394-fdc1-11e5-82cc-4c28410a314d.png)

#Level 3 -> Level 4

The command **ls** was used to list the directory since the password was in a hidden file called inhere.

![image](https://cloud.githubusercontent.com/assets/12781941/14386200/767a29b2-fdc1-11e5-8014-88d0a976289f.png)

#Level 4 -> Level 5

The command **cd** was used to access the directory inhere since the password was in a hidden file inside the directory.

![image](https://cloud.githubusercontent.com/assets/12781941/14386201/7abddc9e-fdc1-11e5-8887-8af08caad7e1.png)

#Level 5 -> Level 6

The command **find** was used to find the file the password stored in based on the given properties.

![image](https://cloud.githubusercontent.com/assets/12781941/14386207/7f1405c0-fdc1-11e5-96ab-1a4f643b2cdd.png)

#Level 6 -> Level 7

The command **find** was used to find the file the password stored in based on the given properties.

![image](https://cloud.githubusercontent.com/assets/12781941/14386213/83c61c0c-fdc1-11e5-855e-0833f496729b.png)

#Level 7 -> Level 8

The command **grep** was used to match the word "millionth" as file the password stored in was next to it.

![image](https://cloud.githubusercontent.com/assets/12781941/14386216/8794a7b8-fdc1-11e5-9219-3a9c15c140d6.png)

#Level 8 -> Level 9

The command **sort** was used to sort the file the password stored in and **uniq** was used to specify the unique file under that name.

![image](https://cloud.githubusercontent.com/assets/12781941/14386220/8c52cd52-fdc1-11e5-9fd8-76b48685e505.png)

#Level 9 -> Level 10

The command **grep** and **strings** were used to figure out the password.

![image](https://cloud.githubusercontent.com/assets/12781941/14386225/90025f26-fdc1-11e5-97a3-d60157ee662e.png)

#Level 10 -> Level 11

The command **base64** was used to access the base64 encoded data file.

![image](https://cloud.githubusercontent.com/assets/12781941/14386228/95260322-fdc1-11e5-9d71-a41191f77f0b.png)

#Level 11 -> Level 12

The command **tr** was used to translate in order to figure out the password.

![image](https://cloud.githubusercontent.com/assets/12781941/14386232/9928deb8-fdc1-11e5-89a2-748bfd0181e0.png)

#Level 12 -> Level 13

This level was difficult compared to previous ones. The command **mkdir** was used to make a temporary directory. It was necessaary to do this step as the password file was compressed. Issues were occured during the process of making a directory as the name we give cannot exist already. Also **zcat** was used to expand the compressed files.

![image](https://cloud.githubusercontent.com/assets/12781941/14386236/9cf68374-fdc1-11e5-87d1-daabaabecf25.png)
![image](https://cloud.githubusercontent.com/assets/12781941/14386243/a0c375e8-fdc1-11e5-8e3c-55fd6c50e4f1.png)

#Level 13 -> Level 14

In this level a private SSH key was used to get the access to the next level.

![image](https://cloud.githubusercontent.com/assets/12781941/14386250/a51c3cba-fdc1-11e5-8432-16cad80a6170.png)
![image](https://cloud.githubusercontent.com/assets/12781941/14386257/a9f8f96c-fdc1-11e5-86a3-1ced72213d75.png)

#Level 14 -> Level 15

Using **telnet** command, port 30000 on localhost was accessed in order to get the password for next level. Password for Level 14 had to be re submitted in this process.

![image](https://cloud.githubusercontent.com/assets/12781941/14386266/af361a04-fdc1-11e5-86de-151b379db1d5.png)

#Level 15 -> Level 16

Using **openssl s_client** command, port 30001 on localhost using SSL was accessed in order to get the password for next level. Password for Level 15 had to be re submitted in this process.

![image](https://cloud.githubusercontent.com/assets/12781941/14386269/b1726e4e-fdc1-11e5-9fae-037c99c8a573.png)
![image](https://cloud.githubusercontent.com/assets/12781941/14386275/b4d5f236-fdc1-11e5-9d43-12a03277bc38.png)

#Level 16 -> Level 17

This was another difficult level compared to previous levels. The command **nmap** was used to determine the available hosts within the range 31000 to 32000. Instead of a password, an RSA private key is given out at the end of the process. To access the next level this RSA key has to be stored in a temporary directory and pass it. But that was failed after numerous attempts.

![image](https://cloud.githubusercontent.com/assets/12781941/14386278/b796ee30-fdc1-11e5-8e3a-a2409aee17cd.png)
