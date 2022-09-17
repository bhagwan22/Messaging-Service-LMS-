# Lightning Messaging Service(LMS):
	- cross DOM messaging Service
	- client side event-bus between DOM branches
	- Use to publish throughout the lightning experience and subscribe the same message anywhere with lightning page
	- use to communicate between VF page, LWC and Aura & UI
	
> It is based on "Lightning Message Channels" metadata type & use "Lightning Message Channel" to access LMS API
	
## How to access lightning message channel
 - LWC: @salesforce/messageChannel/messagint_channel_Name__c
 - VF: $MessageChannel
 - Aura: 
```
# PUBLISH FROM AURA
 <lightning:messageChannel type="messagingChannel_Name__c" aura:id="auraId_channel"/>
 
 var param = = { recordId: event.target.contact.Id };
 comp.find('auraId_channel').publish(param);
 
# SUBSCRIBE IN AURA
  <lightning:messageChannel type ="messagingChannel_Name__c" aura:id="aura_recd_id" onMessage="{!c.handleMessage}"
  
  handleMessage: function(comp, message){
  	if(message && message.getParam('recordId')){
		// logic here
	}
  }

```
	
## Use case:
	- communicate b/w VF page/Aura & LWC 
	- communication b/w flexcards omniStudion
	
