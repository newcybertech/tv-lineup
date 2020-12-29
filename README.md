# CAS-Cable-Channel-Line-up-Skill
CAS Cable Channel Line-up Skill
Properties
The channel object
The Alexa.ChannelController interface uses the channel property as the primary property. The property values are objects. Use the channel property to specify a channel by number, call sign, or affiliate call sign.

Channel object details

Field	Description	Type
number	The channel number, such as 256 or 13.1.	String
callSign	The call sign of the channel, such as PBS.	String
affiliateCallSign	The local affiliate call sign of the channel, such as KCTS.	String
uri	The URI of the channel, such as entity://provider/channel/12307.	String
 Note: None of the fields are required, but at least one of channel.number, channel.callSign, channel.affiliateCallSign, channel.uri, or channelMetadata.name must always be specified.
Channel object example

{
   "name":"channel",
   "value": {
     "number": "9",
     "callSign": "PBS",
     "affiliateCallSign": "KCTS"
  }
}
The channelMetadata object
The channelMetadata property provides additional information about a channel.

ChannelMetadata object details

Field	Description	Type
name	Another name for the channel, such as "The CW".	String
image	The URL of an image or logo for the channel.	String
 Note: None of the fields are required, but at least one of channel.number, channel.callSign, channel.affiliateCallSign, channel.uri, or channelMetadata.name must always be specified.
ChannelMetadata object example

{
   "name":"channelMetadata",
   "value": {
     "name": "Alternate channel name",
     "image": "<url for image>"
  }
}
