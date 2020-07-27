#grep simulator

import re

#get user's need
print('Which file do you want to look into ?')
path = input()
hand = open(path)

print('Enter a regular expression : ')
regex = input()

# get matches
matches = []
for line in hand:
  line = line.rstrip()
  match = re.findall(regex, line)
  if len(match)>0:
    matches.append(match)

# get file name for a nice display
file = re.findall('[ \w-]+?(?=\.)',path)
if len(file) > 0:
  file  = file[0]

print(str(file)+' had '+str(len(matches))+' lines that matched '+regex)
