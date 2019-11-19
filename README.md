# pleasework
#Sarah Mewhinney
#CSCI 102- Section B
#Utility
def PrintOutput(word):
    print("OUTPUT>", word)
def UpdateString(string1, string2, j):
    list1 = list(string1)
    list1[j] = string2
    newstring = ""
    newstring = newstring.join(list1)
    PrintOutput(newstring)
def FindWordCount(a, str1):
    countofstr1 = a.count(str1)
    PrintOutput(countofstr1)
def ScoreFinder(players, scores, name):
    newindex = players.index(name)
    finalscore = scores[newindex]
    print(name, "got a score of", finalscore)
def Union(list1, list2):
    list3 = []
    list3 = list1 + list2
    newlist = []
    for i in list3:
        if i not in newlist:
            newlist.append(i)
    PrintOutput(newlist)
def Intersection(list1, list2):
    list3 = []
    list3 = list1 + list2
    newlist = []
    for i in list3:
        if FindWordCount(list3, i) > 1:
            newlist.append(i)