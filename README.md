# my-stuff
Format a string of names like 'Bart, Lisa & Maggie'.
def namelist(names):
    if(len(names) == 0):
        return ''
        
    if(len(names) == 1):
        return names[0]['name']
    elif(len(names) == 2):
        return (names[0]['name'] + ' & ' + names[1]['name'])
    elif(len(names) > 2):
        sentence = ''
        stophere = len(names) - 2
        for words in range(stophere):
            sentence += names[words]['name'] + ', '
        sentence += (names[len(names) - 2]['name'] + ' & ' + names[len(names) - 1]['name'])
        return sentence
