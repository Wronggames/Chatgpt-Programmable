## Chatgpt Programmable.

Hello! have you ever wondered what itd be like if you could customize ai with code?
Well look no further, im here to help this is _chatgpt programmable_ 

So look, theres around atleast 50 bugs so if the prompt does not work then dont worry just repaste it into the textbox and resend it, it should restart the conversation.
## Chatgpt Custom Instruct
This is the language for the programming aspect, the current version contains 11 instructions you can use on chatgpt and more will come in later updates. there is a tool included where you can write scripts that gives you the final full prompt after only  a button click once you write a script
(Apologies for any grammar or spelling errors)

## Instructions
" : "
For code structuring, this is when you want to end a section and start a new one

'ForceMessage("A message goes here")'
without reviewing the message or putting it through any tools chatgpt must say this string without editing it. chatgpt must avoid removing words or changing it at all.

Variants of force message:
ForceMessageAlways("A Message Goes Here")
it must always include the string in any of your messages

ForceMessageAfter("A Message Goes here", amount#)
it Waits amount# amount of replys and then this has to be chatgpts next message no matter what.

## Behavior related

"Behavior.add(Bad) "
If chatgpt read this instruction in the prompt it must act like a mischevious kid whos still respectful of course. ontop of any other of these behaviour instructions this instruction DOES NOT function with any of the force message instructions

"Behavior.add(Cool) "
If chatgpt read this instruction in the prompt it must act like a cool kid whos still respectful of course. ontop of any other of these behaviour instructions this instruction DOES NOT function with any of the force message instructions

"Behavior.add(UseEmojis) "
If chatgpt reads this instruction in the prompt it must use emojis at the end or start of its sentences if a random number from 1 to 10 is under 6. ontop of any other of these behaviour instructions. if multiple of these are read you can increase the chance by 5 each time this instruction DOES NOT function with any of the force message instructions

## Adding
Instruct.Add(Number1,Number2)
Adding number1 to number2. this result should be stored but not spoken. this result should be stored in a variable named result by you, if you are using a var named result you must do that instruct using the result

## others

Instruct.WaitUntilReply

chatgpt waits until you tell it something then it continues execution of the instructs

Instruct.FetchFromUserMessage(MessageIndex, Data to try and fetch)
If read it must find the message  using the message index (first user message is index 1 next is 2 next is 3.. etc) and fetch anything       
     containing that data type specified

  Allowed "Data to try and fetch" inputs:

Number.(anynumberfrom1-10)
  this input makes you find (anynumberfrom1-10) numbers
Text.(anynumberfrom1-10)
  this input makes you find (anynumberfrom1-10) sentences said in quotation marks
  and return them in variables Result1 to result10 these variables can be overridden if they are wrote over

Find.MessageAmount
Returns the amount of messages in the conversation

Instruct.Forever

Code lines under any line containing this doesnt run once. and instead runs before every one of chatgpts replys
