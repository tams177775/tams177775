 👋 Hi, I’m @tams177775
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
tams177775/tams177775 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import randomimport math print("THIS IS YOUR FAKE PASSPORT GENERATOR \n")print("Follow the operations you need to do \n")print( "I Input Your details In the following fashion\n1. Select Your first names and last names\n2. Input your Two DOB in ages\n3.Enter Your age currently in The Passport\nII You can print out the details in encrypted form or a normal form") print("\nOptions available\n1.Enter the details/n2.Print in encrypteed form\n3.Print in normal form") while (True): print("\nenter the selection\n") opt = int(input()) if (opt == 1): p = 0 # Inputs for the names def name(first1, first2): global p length1 = len(first1) / 2 length2 = len(first2) / 2 if ((length1 - (0.5)) % 2 == 0): half1 = first1[:(round(length1)) + 1] else: half1 = first1[:round(length1)] half2 = first2[round(length2):] p = (half1 + half2) first1 = input("enter first name for first input\n") first2 = input("enter first name for second input\n") second1 = input("enter second name for first input\n") second2 = input("enter second name for second input\n") #Encryption logic with a function def encrypnum(num1): z=num1[:][::-1] return z key = random.randint(0, 26) def encryp(msg, key): encrypted = '' for charac in msg: if charac.isalpha(): n = ord(charac) n += key if charac.isupper(): if n > ord('Z'): n -= 26 elif n < ord('A'): n += 26 elif charac.islower(): if n > ord('z'): n -= 26 elif n < ord('a'): n += 26 encrypted += chr(n) else: encrypted += charac return encrypted # 2nd Part creating a new age age11 = int(input("enter age1 \n")) age22 = int(input("enter age2\n")) curryr = int(input("enter current year\n")) sum11 = 0 sum22 = 0 while (age11 or age22): y11 = age11 % 10 sum11 = sum11 + (y11) age11 = age11 // 10 y22 = age22 % 10 sum22 = sum22 + (y22) age22 = age22 // 10 year = curryr - (sum11 + sum22) day = random.randint(1, 31) month = random.randint(1, 12) # display=print("The New Date of Birth is "+ str(day) + "/" + str(month) + "/" + str(year) ) if (month == 2): day = random.randint(1, 28) elif (month == 1 or 3 or 5 or 7 or 8 or 10 or 12): day = random.randint(1, 31) elif (month == 4 or 6 or 9 or 11): day = random.randint(1, 30) age1 = int(input("enter correct age1 \n")) strage = str(age1) if (len(strage) == 3): countfor = 7 elif(len(strage) == 2):
