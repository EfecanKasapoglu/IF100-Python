year=int(input("Enter the year: "))
while year!= 2018 and year!= 2017:
  year=int(input("Enter the year: "))
month=int(input("Enter the month: "))
if year==2017 or year==2018:
  if year==2017 and not 1<=month<=12:
    while not 1<=month<=12:
      month=int(input("Enter the month: "))
  elif year==2018 and month!=1:
    while month!=1:
      month=int(input("Enter the month: "))
if month<10:
  month="0"+str(month)
sarki={}
sarkici={}
dictson={}
dictsondan2={}
spotifydata=open("turkiye_spotify_data.txt", "r")

spotifydata12=spotifydata.readlines()
for i in spotifydata12[1:]:
  i=i.strip()
  database=i.split("\t")
  tarih = database[5]
  tarih = tarih.split("-")
  yıl = tarih[0]
  ay = tarih[1]
  sarkici[database[2]]=database[4]
  dictson[database[1]]=database[2]
  dictsondan2[database[1]]=database[4]
  if str(year) == str(yıl) and str(month)==str(ay):
    if database[1] in sarki.keys():
      sarki[database[1]]=int(sarki[database[1]])+int(database[3])
    else:
      sarki[database[1]]=database[3]

A=True
maksimum=0
kontrol = 0
C=True
def sayı(sarki):
  while A: 
    for a,b in sarki.items():
      if kontrol<int(b):
        kontrol=int(b)
        maksimum=a
      else:
        A=False
  return maksimum

  print("NEW SUGGESTION: ",maksimum,", ", dictson[maksimum], " (Total stream number in this month: " ,kontrol,")",sep="")
B = True
while B == True:
  answer=input("Do you want to listen this song (enter either yes or no): " ).lower()
  if answer != "yes" and answer != "no":
    B = True

  elif answer == "yes":
    print("Enjoy ", maksimum,", ", dictson[maksimum],". Here is the url for you: ", dictsondan2[maksimum],sep="")
    B = False
    break

  elif answer == "no":
    sarki.pop(maksimum)
    kontrol=0
    print(sarki)
    sayi(maksimum)

    print("NEW SUGGESTION: ",maksimum,", ", dictson[maksimum], " (Total stream number in this month: " ,kontrol,")",sep="")
    
    print(sarki)
    B = True
