  global mydb
  mydb = mysql.connector.connect(
  host="localhost",
  user="myusername",
  password="mypassword")
  Create database mysql;Create table ujjwal(username varchar(19),passw varchar (14));Create table member( ad varchar(55),name varchar(50),addr varchar(90),phone varchar(10),email varchar(60),Age int);Create table vaccination (ad varchar(12), name varchar(50),dt date, d varchar(10));
def showusers():
  c1=db1.cursor()
  c1.execute("select * from ujjwal")
  res = c1.fetchall()
  print("List of Ujjwal ")
  for val in res:
    print("UserName = "+val[0] + " Password =" + val[1])
def login():
  print("-" * 50)
  print("\t COVID VACCINATION RECORD")
  print("-" * 50)
  print("\t LOGIN")
  un = input("Enter User Name: ")elect * from ujjwal")
  res = c1.fetchall()
  print("List of Ujjwal ")
  for val in res:
    print("UserName = "+val[0] + " Password =" + val[1])
def login():
  print("-" * 50)
  print("\t COVID VACCINATION RECORD")
  print("-" * 50)
  print("\t LOGIN")
  un = input("Enter User Name: ")
  pw= input("Enter Password: ")
  q= "select * from ujjwal where username=%s and passw=%s"
  val = (un,pw)
  c2= db1.cursor()
  c2.execute(q,val)
  res = c2.fetchall() 
