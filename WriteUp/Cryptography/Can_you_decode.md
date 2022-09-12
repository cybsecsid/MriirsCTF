# Cryptography (Can You Decode?)

We have three files to solve this challenge. The flag was divided into 3 parts in three different files.\
**1. encrypted1 (Audio File)\
2. encrypted2 (PNG File)\
3. encrypted3 (Word File)**

##  Challenge File:

You can download the challenge file from [HERE](https://github.com/ashtrace/MriirsCTF/raw/main/WriteUp/Cryptography/Cryptography.zip)

## Encrypted1 (Audio File):

As soon as we hear the sound, we can understand that it’s encoded in morse code. We can find morse code decoder in the internet. The one I used is: [Here](https://morsecode.world/international/decoder/audio-decoder-adaptive.html)

The decoded string is **‘FLAG’**


## Encrypted2 (PNG File):

This is some kind of cipher code. Now if we google the image, we find some hints about the cipher code. On further inspection, we can understand that its known as **‘Pigpen Cipher’**. The decoder used for this is: [Here](https://planetcalc.com/7842/)

The decoded string is **‘CRYPTGRPHY’**

## Encrypted3 (Word File):

 We have got a hint that the text is rotated, meaning rot cipher is used. But for the actual rot number we need to calculate the sum given.
BOOM! \
**Its rot 13.**\
Website used to decode rot 13 : [CLick Here](https://rot13.com/)


The following was the message we decoded:
“ 
**"aTVfYzAwbH0="** 
you have reached the base! How about moving upward? “

Again, we got the hint that it’s a BASE encoding. And the widely used BASE encoding is BASE64. So, we use a BASE64 decoder to decode the first line, which would ultimately give us the final part of the flag. 
The website used for BASE64 decoding is:
[Here](https://www.base64decode.org/)

The final part is:
‘ **i5_c00l}**‘




## Flag
Now, joining all the three parts, we get the final flag as (within the flag format):
**flag{CRYPTGRPHY_i5_c00l}**




## Author
 [Derick Johnson](https://www.linkedin.com/in/derick-m-johnson/)
