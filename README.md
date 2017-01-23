# InsomnihackTeaser2017-cryptoquizz
Insomnihack Teaser 2017 cryptoquizz Write Up

<b>Cryptoquizz : </b> <br/>
Hello, young hacker. Are you ready to fight rogue machines ? Now, you'll have to prove us that you are a genuine cryptographer.

Running on quizz.teaser.insomnihack.ch:1031

<b>Solution : </b><br/>
When we connect to host this is the sample output : 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
madHatter:Desktop madHatter$ nc quizz.teaser.insomnihack.ch 1031


~~ Hello, young hacker. Are you ready to fight rogue machines ?    ~~
~~ Now, you'll have to prove us that you are a genuine             ~~
~~ cryptographer.                                                  ~~



~~ What is the birth year of Ralph Merkle ?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

It askes us questions about birth year of different cryptographers.

In order to get the flag we wrote a python code which has all of the cryptograpers name and birth year.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
import socket


def netcat(host, port):
    s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
    s.connect((host, int(port)))
    content = None
    while True:
        data = s.recv(4096)
        print(repr(data))
        
        if "Shannon" in repr(data):
            content = "1916\n"
            s.sendall(content.encode())
       

        if "Davies" in repr(data):
            content = "1924\n"
            s.sendall(content.encode())
       

        if "Ferguson" in repr(data):
            content = "1965\n"
            s.sendall(content.encode())
       

        if "Vaudenay" in repr(data):
            content = "1968\n"
            s.sendall(content.encode())
       

        if "Mitsuru Matsui" in repr(data):
            content = "1956\n"
            s.sendall(content.encode())
       

        if "Stinson" in repr(data):
            content = "1956\n"
            s.sendall(content.encode())
     

        if "Brassard" in repr(data):
            content = "1955\n"
            s.sendall(content.encode())
        

        if "Ross Anderson" in repr(data):
            content = "1956\n"
            s.sendall(content.encode())
        

        if "Feistel" in repr(data):
            content = "1915\n"
            s.sendall(content.encode())
        

        if "Bernstein" in repr(data):
            content = "1971\n"
            s.sendall(content.encode())
        

        if "Kocher" in repr(data):
            content = "1973\n"
            s.sendall(content.encode())
        

        if "Coppersmith" in repr(data):
            content = "1950\n"
            s.sendall(content.encode())
        

        if "Lindell" in repr(data):
            content = "1971\n"
            s.sendall(content.encode())
        

        if "Rijmen" in repr(data):
            content = "1970\n"
            s.sendall(content.encode())
        

        if "Shamir" in repr(data):
            content = "1952\n"
            s.sendall(content.encode())
        

        if "Bellare" in repr(data):
            content = "1962\n"
            s.sendall(content.encode())
        

        if "Michael O. Rabin" in repr(data):
            content = "1949\n"
            s.sendall(content.encode())
        

        if "Bleichenbacher" in repr(data):
            content = "1964\n"
            s.sendall(content.encode())
        

        if "Chaum" in repr(data):
            content = "1955\n"
            s.sendall(content.encode())
        

        if "Oorschot" in repr(data):
            content = "1962\n"
            s.sendall(content.encode())

        

        if "Sahai" in repr(data):
            content = "1974\n"
            s.sendall(content.encode())
        

        if "Ferguson" in repr(data):
            content = "1965\n"
            s.sendall(content.encode())
        

        if "Niels" in repr(data):
            content = "1964\n"
            s.sendall(content.encode())


        if "Daemen" in repr(data):
            content = "1965\n"
            s.sendall(content.encode())


        if "Xiaoyun" in repr(data):
            content = "1966\n"
            s.sendall(content.encode())


        if "Micali" in repr(data):
            content = "1954\n"
            s.sendall(content.encode())


        if "Victor S. Miller" in repr(data):
            content = "1947\n"
            s.sendall(content.encode())
            

        if "Patarin" in repr(data):
            content = "1965\n"
            s.sendall(content.encode())
            

        if "Merkle" in repr(data):
            content = "1952\n"
            s.sendall(content.encode())
            

        if "Donald Davies" in repr(data):
            content = "1924\n"
            s.sendall(content.encode())
            

        if "Rogaway" in repr(data):
            content = "1962\n"
            s.sendall(content.encode())
            

        if "Yvo Desmedt" in repr(data):
            content = "1956\n"
            s.sendall(content.encode())
            

        if "Smart" in repr(data):
            content = "1967\n"
            s.sendall(content.encode())
            

        if "Hellman" in repr(data):
            content = "1945\n"
            s.sendall(content.encode())
            

        if "Okamoto" in repr(data):
            content = "1952\n"
            s.sendall(content.encode())
            

        if "Knudsen" in repr(data):
            content = "1962\n"
            s.sendall(content.encode())
            

        if "Schnorr" in repr(data):
            content = "1943\n"
            s.sendall(content.encode())
            

        if "Massey" in repr(data):
            content = "1934\n"
            s.sendall(content.encode())
            

        if "Biryukov" in repr(data):
            content = "1969\n"
            s.sendall(content.encode())
            

        if "Biham" in repr(data):
            content = "1960\n"
            s.sendall(content.encode())
            

        if "Stern" in repr(data):
            content = "1949\n"
            s.sendall(content.encode())
            

        if "Joux" in repr(data):
            content = "1967\n"
            s.sendall(content.encode())
            

        if "Halevi" in repr(data):
            content = "1966\n"
            s.sendall(content.encode())
            

        if "Cramer" in repr(data):
            content = "1968\n"
            s.sendall(content.encode())
            

        if "David Naccache" in repr(data):
            content = "1967\n"
            s.sendall(content.encode())
            

        if "Kaisa Nyberg" in repr(data):
            content = "1967\n"
            s.sendall(content.encode())
            

        if "Whitfield" in repr(data):
            content = "1944\n"
            s.sendall(content.encode())
            

        if "Moni Naor" in repr(data):
            content = "1961\n"
            s.sendall(content.encode())
            

        if "Rafail Ostrovsky" in repr(data):
            content = "1963\n"
            s.sendall(content.encode())

        if not data:
            print(repr(data))
            break



    s.shutdown(socket.SHUT_WR)
    s.close()

netcat("quizz.teaser.insomnihack.ch",1031)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

After responding questions it gives us the flag in this output : 

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
OK, young hacker. You are now considered to be a <b>INS{GENUINE_CRYPTOGRAPHER_BUT_NOT_YET_A_PROVEN_SKILLED_ONE}</b>
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
