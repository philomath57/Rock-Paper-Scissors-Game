# Rock-Paper-Scissors-Game
import random 
def game(comp,user):
  if comp==user:
    return None
  elif comp=='r' and user=='p':
    return True
  elif comp=='r' and user=='s':
    return False
  elif comp=='p' and user=='s':
    return True
  elif comp=='p' and user=='r':
    return False
  elif comp=='s' and user=='p':
    return False
  elif comp=='s' and user=='r':
    return True
print("comp: rock(r) paper(p), scissor(s)??")
randno=random.randint(1,3)
if randno==1:
  comp='r'
elif randno==2:
  comp='p'
elif randno==3:
  comp='s'
user=input("Your input: \n")
a=game(comp,user)
print(f"Computer chose {comp}")
print(f"User chose {user}")
if a==None:
  print("Tie\n")
elif a:
  print("User Wins\n")
else:
  print("Computer Wins\n")
