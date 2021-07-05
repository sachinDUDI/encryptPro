
#for encrpt and decrypt

def encrypt (code,enkey):

    return enkey.join(code)

def decrypt (code,enkey):

    return code.split(enkey)

#

maincode=input("enter your message code")

encode=input("enter encryption key :")

secretPass=input("enter secret password only alphabet form:")

enStr=encrypt(maincode,encode)

#converting delStr from lidt to string

print("The encrypted code is", enStr)

passwrd=input("enter passwrd to see decrypted massage")

if passwrd==secretPass:

    delStr=decrypt(enStr,encode)

    deStr="".join(delStr)

    print("code after decryption is :",deStr)

else :

    print("you insert the wrong passwrd")
