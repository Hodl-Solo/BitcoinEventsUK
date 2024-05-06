# Telegram Group Setup Guide

1. Make your Telegram group public and then change the URL to something that matches your group name and is human readable. 
2. Search for Shieldy and add it to the group. 
3. Make Shieldy an admin. 
4. Prevent anyone except admins from interacting with Shieldy with the `/lock` command.
5. The rest of the setup is up to your personal preference, but here are some recommendations. 
	1. Set a custom greeting with /greeting
	2. Type `/deleteGreetingTime 100` to remove greeeting messages for new users after 100 seconds. 
	3. /captcha and choose digits.


To save time you can copy/paste the following text to setup Shieldy in one message -

  
/setConfig
language: en
captchaType: digits
timeGiven: 240
adminLocked: true
restrict: false
noChannelLinks: false
deleteEntryMessages: false
greetsUsers: true
customCaptchaMessage: false
strict: true
deleteGreetingTime: 120
banUsers: false
deleteEntryOnKick: true
cas: true
underAttack: false
noAttack: false
buttonText: Not set
allowInvitingBots: false
skipOldUsers: false
skipVerifiedUsers: false
restrictTime: 24
banNewTelegramUsers: false
greetingButtons:
Not set


Note - Shieldy needs to be an admin to display welcome messages. 




Make sure @shieldy_bot is an admin at your chat and it's all done! You can also further setup the behaviour with the following commands:

/help — shows this message

/language — switches language

/captcha — changes type of captcha used
/timeLimit — changes amount of time given to newcomers
/lock — makes commands accessible only by admins
/restrict — restricts newcomers to send only text messages in the first 24 hours
/deleteEntryMessages — delete messages about user entry
/greeting — greets users who pass the test
/trust — reply with this command to a message sent by user that you don't want to check
/ban — same as trust, but the opposite
/strict — use when you don't want to receive any newcomers' messages but captcha solutions until they pass captcha
/customCaptchaMessage — setup custom captcha message
/deleteGreetingTime — setup when to delete Shieldy's greeting in seconds like /deleteGreetingTime 100, reset by setting it to 0
/banUsers — whether to ban or to kick users
/deleteEntryOnKick — whether to delete entry messages for users who failed captcha
/cas — whether to use Combot Anti-Spam or not
/underAttack — toggle the mode to automatically kick all newcomers
/noAttack — disables Shieldy
/noChannelLinks — automatically delete messages that link to other telegram channels
/viewConfig — view the current Shieldy configuration
/buttonText — change the captcha button text in the form of /buttonText I'm not a bot!
/allowInvitingBots — whether users can invite other bots or not
/greetingButtons — setup buttons for greeting message
/skipOldUsers — don't show captcha to Telegram accounts with ID less than 1000000000
/skipVerifiedUsers — don't show captcha to users who have ever passed captcha in any chat
/setConfig — setup Shieldy configuration in one message
/banForFastRepliesToPosts — turn on or off banning users who reply to new channel posts within 5 seconds after posts are created
/restrictTime — setup how much time will Shieldy /restrict a newcomer in hours like /restrictTime 24, reset by setting it to 0
/banNewTelegramUsers — instantly ban (or kick) newcomers with Telegram ID over 1 000 000 000
