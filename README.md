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