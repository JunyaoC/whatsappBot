# WhatsApp Bot
Sometimes we need to send large batch of messages in WhatsApp, but the contacts aren't saved as a contact in our phone. This code aims to solve this problem, where messages can be sent to recipients without saving. The message can also take in variables, which can be very useful for customized messages and logic proccessing.

##Features
1. Send WhatsApp messages directly to phone numbers without saving.
2. Messages can take in variables which can be substitute while sending.
4. Use of Excel spreadsheet as input.
3. GUI interface

##Instruction
1. Load an excel file containing data and contact numbers you like to message.
    **Do not include any title!**:
    >Only include data and start on first cell (Row1 Column1). Do not include title (eg: Name, Contact Number) in Excel speadsheet!
2. After including the spreadsheet, values in the spreadsheet are recognized as independent variables. Type your message, and use @var[number] to insert variable.
    Exmaple (assume @var1 has value "John Smith"):
    > Insert: Hi @var1
    >Result : Hi John Smith
3. Preview your message or customize delay. The delay is the delay in seconds between messages are being sent. Depends on your network, a faster network can use a shorter delay for better efficiency.
4. Hit Run.
5. Selenium will launch with preferred web driver. Default is chrome.
6. After scanning the barcode, the bot will start delivering your messages to contact numbers automatically.

#Known Issue
1.Currently only support Text Messages without emoji.


##Dependencies
eel
openpyxl
selenium
