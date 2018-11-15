mydictionary = {}
with open("doc.csv","r") as csv_file:
    reader = csv.reader(csv_file)
    for row in reader:
        mydictionary[row[0]] = row[1]
    for row in reader:
        if mydictionary[row[0]][0] == 'a' or mydictionary[row[0]][0] == 'A' :
            print(mydictionary[row[1]])
       
