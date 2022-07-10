# BHAG
Create a chat server that allows multiple people to chat in realtime.

## User Requirements
As a user I should be able to...
* Login / Logout
* Create chatroom
* Delete chatroom
* Send chat messages
* Join a chatroom
* Make an account

## Questions
* Am I going to use a DB?
	* Yes, to store username, password
	* Possibly store active chatrooms aswell as messages

* How to use websockets?
	* IDK

* How are passwords going to be stored?
	* Definetly not plaintext, some hash function maybe, not meant to be super
	Secure.

* Username requirements?
	* Only alphanumeric; case sensitive

* What information is the user going to provide?
	* When creating an account; username and password;

* How do I know when to remove a chatroom?
	* Probably after empty or innactive for period of time; clean up on backend

* How long will the user be logged in?
	* Maintain session for day initially; saved on front end; cookies?

* How do I handle username dups?
	* Send back messages saying unavailabe username

* Will messages be stored on backend? How long?
	* Only while chatroom is active

* How will chatrooms be shared? Via public list? Private code?
	* On front end list of public rooms; with stats; Private not shown only join
	* via code(key)

* How will server generate code?
	* IDK some random number algorithm key generator

