import qrcode
import random
import string

#Function to define random filename
def fileNameGenerator(length):
    letters = string.ascii_letters
    resultString = ''.join(random.choice(letters) for i in range(length))
    return resultString

#User defines how many to create
amountOfFiles = int(input('How many QR codes would you like to generate? '))

#Generates QRcodes
for i in range(amountOfFiles):
    genFileName = fileNameGenerator(15)
    data = input('Enter text: ')
    img = qrcode.make(data)
    genFileNameFinal = str(genFileName + '.png')
    img.save(genFileNameFinal)
