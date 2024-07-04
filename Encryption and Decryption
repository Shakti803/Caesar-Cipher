# This is a Caesar Cipher program

def encrypt(text, shift):
  result = ""
  for char in text:
    if char.isalpha():
      if char.isupper():
        result += chr((ord(char) - 65 + shift) % 26 + 65)
      else:
        result += chr((ord(char) - 97 + shift) % 26 + 97)
    else:
      result += char
  return result

def decrypt(text, shift):
  result = ""
  for char in text:
    if char.isalpha():
      if char.isupper():
        result += chr((ord(char) - 65 - shift) % 26 + 65)
      else:
        result += chr((ord(char) - 97 - shift) % 26 + 97)
    else:
      result += char
  return result

text = input("Enter your message: ")
shift = int(input("Enter the shift value: "))

print("Do you want to (E)ncrypt or (D)ecrypt?")
choice = input().upper()

if choice == 'E':
  print("Encrypted message: " + encrypt(text, shift))
elif choice == 'D':
  print("Decrypted message: " + decrypt(text, shift))
else:
  print("Invalid choice. Please enter E or D.")
