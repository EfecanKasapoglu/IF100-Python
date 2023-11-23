database=input("Please enter the database: ")
movement=input("Please enter the movement name that you want to purchase: ")
newdatabase=database.split(",")
movementlist=[]
moneylist=[]
paintlist=[]
for x in newdatabase:
      all=x.split(":") 
      all2=x.split(";")
      paintlist.append(all[0])
      moneylist.append(all2[-1])
      movementlist.append((all2[0]).split(":")[1])
if movement not in movementlist:
  print("There are no paintings belonging to ",movement,".", sep="")
else:
  money=float(input("Please enter the amount of money you have (in million): "))
  painting=input("Please enter the name of the painting that you want to buy: ")
  painting=painting.split(",")
  for i in painting:
    if i not in paintlist:
      print(i, "is not in the database.")        
    else:
      if len(painting)==1:
        idx=paintlist.index(i)
        idx2=movementlist.index(movement)
        if  idx==idx2:
          if float(money)>=float(moneylist[idx][0:3]):
            print("You have successfully purchased ", i,".",sep="")                      
          else:
            print("Willing painting(s) value(s) are higher than your current budget.")       
           
        elif idx!=idx2:
          print(i,"does not belong to", movement, "movement.")              
     
      elif len(painting)!=1:
        price=0 
        c=0
        for a in painting:        
          idx=paintlist.index(a)  
          while c<=len(painting):                 
            if movementlist[idx]!=movement:
              print(a,"does not belong to", movement, "movement.")
              c+=1              
            elif movementlist[idx]==movement:
              price=price+float(moneylist[idx][0:3])
              c+=1
              
        if money>=price:        
          print("You have successfully purchased ",painting[0],",",painting[-1], ".", sep="")
          break
        elif money<price:
          print("Willing painting(s) value(s) are higher than your current budget.")
          break
