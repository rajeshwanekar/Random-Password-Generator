# Random Password Generator


## Import libraries

```python
import string
import random
```


## User input and print menu



```python
length = int(input('Enter password length : '))
print('''choose character set for password from these :
          1. Letters
          2. Digits
          3. Special characters
          4. Exit''')
```

## While Loops and For Loops

```python
characterList = ""
while(True):
    choice = int(input("Pick a number : "))
    if(choice == 1):

     characterList += string.ascii_letters 

    elif(choice == 2):

     characterList += string.digits

    elif(choice == 3):

     characterList += string.punctuation

    elif(choice == 4):
         break

    else:
        print('Please pick a valid option!')

password = []

for i in range(length):
      randomcharacter = random.choice(characterList)
      password.append(randomcharacter)
```
## Print Output

```python
print("The random password is : " + "".join(password))
```

## Contributing

This project is done by Rajesh Wanekar
You can connect with me on [![Linkedin](https://i.sstatic.net/gVE0j.png) LinkedIn](https://www.linkedin.com/in/rajesh-wanekar-342288320/)
