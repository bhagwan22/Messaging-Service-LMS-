## Setp 1:
  > update package.xml file 
  ```
    <types>
       <members>*</members>
       <name>LightningMessageChannel</name>
    </types>
  ```
## Setp 2:
  > create a file with extension `.messageChannel-meta.xml`
## step 3:
  > define staructur of file
  ```
    <?xml version="1.0" encoding="UTF-8" ?>
    <LightningMessageChannel xmlns="http://soap.sforce.com/2006/04/metadata">
      <masterLabel>MyMessageChannel_Name</masterLabel>
      <isExposed>True</isExposed>
      <description>This LMC(lightning message channel) will help send msg b/w LWC, Aura, Vfpage</description>
      
      <lightningMessageFields>
       <fieldName>messageToSend</fieldName>
       <description>message To Send</description>
     </lightningMessageFields>

     <lightningMessageFields>
         <fieldName>sourceSystem</fieldName>
         <description>My source?</description>
     </lightningMessageFields>
    </LightningMessageChannel>
  ```
  ## step 4: 
    deploy to org
