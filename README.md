# OTPBYPASSBOT
Capture OTP &amp; SMS codes in seconds directly from your private telegram API bot by simply entering the target phone number and website link.

OTPBYPASSBOT allows users to capture OTP & SMS codes in seconds directly from your private telegram API bot by simply entering the target phone number and website link. Sim swaps are no longer necessary due to our technology.

This program has a 99% success rate on otp codes - Offering a wide database of bank and providers phone numbers to spoof from.
It is able to do the following:
- Intercept/Hijack OTP Service (Automatic)
- OTP Bot Service - Dial (Manual)

# API
The API requests availables & working :

- /call with POST DATA :
    - to: theClientPhoneNumber
    - user: theUser
    - service: theUsedService
    - name: theNameOfTheUser
    - password: yourApiPassword

- /get with POST DATA :
    - callSid: theCallSid
    - password: yourApiPassword

- /stream/service with GET DATA :
    - service: theServiceNameYouWannaUse

- /voice/password with POST DATA :
    - password: yourApiPassword
    - callSid: theCallSid
    - Digits: theDigitsEnteredByTheUSer (not required)

# BOT COMMANDS
All the Admin commands :

- !user add @user : allow someone to use the bot & the calls
- !user delete @user : remove someone or an admin from the bot
- !user info @user : get infos from a user
- !user setadmin @user : set a user to admin

All the Users commands :

- !secret yoursecretpassword @user : set a user to admin without been admin
- !call phonenumber service or for example !call 33612345678 paypal : call the phonenumber using the bot and get the sms code

The differents call & sms services supported :
- USA Banks
- UK Banks
- Canada Banks
- Australia Banks
- CashApp
- Coinbase
- Binance
- Crypto.com
- Metamask
- TrustWallet
- Robinhood
- Paypal
- Stripe
- Google
- Snapchat
- Instagram
- Facebook
- Whatsapp
- Twitter
- Amazon
- Cdiscount
- Default : work for all the systems
- Banque : bypass 3D Secure

# HOW IT WORKS
- When you do a !call (3312345678) Citibank, the OTPBYPASS Bot sends a post request to the api, which will save the call into a sqlite DB and send the call to the custom twilio API.
- The Twilio API use our /status route to know what to do in the call, the status route returns TwiML code to Twilio.
- The /status route returns the self hosted service song using the /stream/service route.
- If the user enter the digit code using the numpad, the song stops, it thanks him for the code, and end the call.
- The /status route send the code to your discord channel using a webhook.

# SCREENSHOT SAMPLES
![image](https://user-images.githubusercontent.com/106332046/170526825-23a0ef54-ed1a-4b52-b142-5fb43fddc8b2.png)
![image](https://user-images.githubusercontent.com/106332046/170527290-701222fd-6e26-4f75-9a98-a9c8b3abb6a4.png)
![image](https://user-images.githubusercontent.com/106332046/170527310-f75a51a0-51f8-43ba-b974-44694bae1fbd.png)
![image](https://user-images.githubusercontent.com/106332046/170527350-02896020-6074-4668-a645-a86982d13b67.png)
![image](https://user-images.githubusercontent.com/106332046/170527403-fadde93a-1fd6-4c58-afc2-80e88548d106.png)
![image](https://user-images.githubusercontent.com/106332046/170527418-fafcc684-df0d-4b4f-bcfd-0eb5b9c92f97.png)
![image](https://user-images.githubusercontent.com/106332046/170527462-45be52f3-c3d1-4cc2-a261-3757ae0dcb3c.png)
![image](https://user-images.githubusercontent.com/106332046/170527484-69ac5886-53aa-4e30-9176-435525b16260.png)
![image](https://user-images.githubusercontent.com/106332046/170527507-1e8ac337-8f5f-4eee-ae7d-84b4220abff3.png)
![image](https://user-images.githubusercontent.com/106332046/170527527-5da1dbe6-c6cc-40cc-88f4-238e4805a944.png)

# ADDITIONAL FEATURES
- Custom Caller ID (can use any company or bank)
- Unique text-to-speech for each call
- Human like voice
- Multiple modes to choose from
- Multiple languages supported
- Multiple countries supported


# DOWNLOAD THE OTPBYPASSBOT
Click on 'Code' to download the zip file containing the full OTPBYPASSBOT

# Disclaimer
This code is only a POC code, do not use it illegally. You could been arrested to use badly this code. Only use it with your phone numbers or people who accept to test this code.
