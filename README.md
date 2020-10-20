print("Title of program: Basketball formations bot")
print()
while True:
  description = input("What Basketball formations would you like to know?")

  list_of_words = description.split()

  Basketballformations_list = []
  information_list = []
  counter = 0
  
  for each_word in list_of_words:
    
    if each_word == "fiveout":
      Basketballformations_list.append("fiveout")
      information_list.append("all players on the offense spreads out and stands at each of the five spots of the three point line")
      counter += 1
    if each_word == "122":
      Basketballformations_list.append("122")
      information_list.append("that there is 3 lines of defense in 122 form which is a very good formation")
      counter += 1
    if each_word == "131X":
      Basketballformations_list.append("131X")
      information_list.append("This use in offense when the opponent is having a full court press and one person screens for one player and another person  runs down the court")
      counter += 1
 
  if counter == 0:
    
      output = "Sorry I don't understand. Please use different words."

  elif counter == 1:
    
      output = Basketballformations_list[0] + " means that "+ information_list[0] + ". Hope you understand it now."  

  else:

    feelings = ""    
    for i in range(len(feelings_list)-1):
      feelings += feelings_list[i] + ", "
    feelings += "and " + feelings_list[-1]
    
    encouragement = ""    
    for j in range(len(encouragement_list)-1):
      encouragement += encouragement_list[i] + ", "
    encouragement += "and " + encouragement_list[-1]

    output = "It seems that you are feeling quite " + feelings + ". Please always remember "+ encouragement + "! Hope you feel better :)"

  print()
  print(output)
  print()
