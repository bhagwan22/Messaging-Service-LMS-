# Lightning Messaging Service(LMS):
	- cross DOM messaging Service
	- client side event-bus between DOM branches
	- Use to publish throughout the lightning experience and subscribe the same message anywhere with lightning page
	- use to communicate between VF page, LWC and Aura & UI
	
> It is based on "Lightning Message Channels" metadata type & use "Lightning Message Channel" to access LMS API
	
## How to access lightning message channel
	- LWC: @salesforce/messageChannel
	- VF: $MessageChannel
	- Aura: lightning:messageChannel
	
## Use case:
	- communicate b/w VF page/Aura & LWC 
	- communication b/w flexcards omniStudion
	
