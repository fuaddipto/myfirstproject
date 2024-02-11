def add(x,y):
  return x+y
def sub(x,y):
  return x-y
def mul(x,y):
  return x*y
def divide(x,y):
  return x/y
  

print("Select operation.")
print("1.Add")
print("2.Subtract")
print("3.Multiply")
print("4.Divide")
while True:
  choice =input("enter a choice :")
  if choice in ('1','2','3','4'):
    try:
       num1=float(input("enter first num :"))
       num2=float(input("enter second num :"))
    except ValueError:
       print("invalid input.Please enter a num")
       continue
    if choice =='1':
      print(num1 ,"+",num2,"=",add(num1,num2))
    elif choice =='2':
        print(num1 ,"2",num2,"=",sub(num1,num2))
    elif choice =='3':
      print(num1 ,"*",num2,"=",mul(num1,num2))
    elif choice =='4':
      print(num1 ,"/",num2,"=",divide(num1,num2))
    next_cal=input("enter new calculation?yes/no\n")
    if next_cal == "no":
      break
      
  else : 
    print("invalid input.pls try again")
