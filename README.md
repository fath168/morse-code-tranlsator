# morse-code-tranlsator
name = input("Please enter your name: ")
print(f'welcome {name} to a morse code translator!')
reason = input('Why do you want to learn morse code?')
print('ahhhh, i see:D')
print(f'good luck on your journey {name} !')
print('')
print('')
print('')
print('')
print('                welcome')
print('               _-------_')

morse_dict = {'a': '.-', 'b': '-...', 'c': '-.-.', 'd': '-..', 'e': '.', 
    'f': '..-.', 'g': '--.', 'h': '....', 'i': '..', 'j': '.---', 
    'k': '-.-', 'l': '.-..', 'm': '--', 'n': '-.', 'o': '---', 
    'p': '.--.', 'q': '--.-', 'r': '.-.', 's': '...', 't': '-', 
    'u': '..-', 'v': '...-', 'w': '.--', 'x': '-..-', 'y': '-.--', 
    'z': '--..', ' ': ' '}

while True:
 text_to_translate = input('Enter words please!: ').lower()
 translated_message = []
 for char in text_to_translate:
  if char in morse_dict:
        translated_message.append(morse_dict[char])   
  else:
   translated_message.append(char)

 print('MORSE CODE: ')
 print(' '.join(translated_message))
 print('')