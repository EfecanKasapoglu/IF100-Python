hori_knight=input("Please enter horizontal position of the knight (a,b,c,d,e,f,g,h): ")
h = "a,b,c,d,e,f,g,h"
v = "1,2,3,4,5,6,7,8"
if hori_knight.lower() in h:
  vert_knight=input("Please enter vertical position of the knight (1,2,3,4,5,6,7,8): ")
  if vert_knight in v:
    hori_bis=input("Please enter horizontal position of the bishop (a,b,c,d,e,f,g,h): ")
    if hori_bis.lower() in h:
      vert_bis=input("Please enter vertical position of the bishop (1,2,3,4,5,6,7,8): ")
      if vert_bis in v:
        if hori_knight.lower()==hori_bis.lower() and vert_bis==vert_knight:
          print("They can't be in the same square")
        elif (int(vert_bis) - int(vert_knight) == 2 or int(vert_bis) - int(vert_knight) == -2) and (ord(hori_knight.lower())-ord(hori_bis.lower()) == 1 or ord(hori_knight.lower())-ord(hori_bis.lower()) == -1):
          print("Knight can attack bishop")
        elif (int(vert_bis) - int(vert_knight) == 1 or int(vert_knight) - int(vert_knight)) == -1 and (ord(hori_knight.lower()) - ord(hori_bis.lower()) ==2 or ord(hori_knight.lower())- ord(hori_bis.lower()) ==-2):
          print("Knight can attack bishop")
        elif int(vert_bis) - int(vert_knight) == ord(hori_bis.lower()) - ord(hori_knight.lower()):
          print("Bishop can attack knight")
        else:
          print("Neither of them can attack each other")
      elif (vert_bis).isalpha():
        print("Vertical input for bishop is not a number") 
      elif (vert_bis).isdigit() and 'vert_bis' not in v:
        print("Vertical input for bishop is not a proper number")
      elif not (vert_bis).isdigit():
        print("Vertical input for bishop is not a number")
    elif not (hori_bis).isalpha:
      print("Horizontal input for bishop is not a letter")
    elif len(hori_bis)>=2:
      print("Horizontal input for bishop is not a letter")
    elif len(hori_bis)<2 and hori_bis.lower() not in h:
      print("Horizontal input for bishop is not a proper letter")
  elif not vert_knight.isdigit():
    print("Vertical input for knight is not a number")
  elif vert_knight.isalpha():
    print("Vertical input for knight is not a number")
  elif vert_knight not in v and vert_knight.isdigit():
    print("Vertical input for knight is not a proper number")
elif not (hori_knight).isalpha():
  print("Horizontal input for knight is not a letter")
elif len(hori_knight)>=2:
  print("Horizontal input for knight is not a letter")
elif len(hori_knight)<2 and hori_knight.lower() not in h:
  print("Horizontal input for knight is not a proper letter")
