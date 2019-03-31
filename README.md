# ASICs as an open platform

NB:  This story comes from my involvement in several Telegram chats with people working to pry open hardware platforms that have been intentionally closed by their makers.  It should absolutely be understood as advocating for a certain point of view with regard to how software should work on ASIC mining platforms.  Advocacy for open platforms is my express intent, and the intent of the people I've been working with on this.  

You can join the conversation here:  https://t.me/ExploitS15

# S15 vs. S9: Automation

Recently, the Bitmain S15 was released.  It was another in a long line of great miners from Bitmain, except that users were unable to use SSH to configure the miner, AND users were unable to use the cgminer API to configure the miner.  What this means is that purchasers of the S15 are stuck doing these tasks by hand through the WebUI, specifally:

* Setting the IP address
* Setting the mining pool configuration
* Changing settings after the fact

With both SSH and cgminer API access on the S9, these changes could be automated.  On the S15 they need to be done by hand, which massively complicates setup and ongoing administration.    

Additonally, there's been no word from Bitmain as to why these changes were made, only that they are "expected behavior"

# The Hack!

Two of our community members have worked hard to restore S9-like functionality to the S15.  They were successful not only in restoring SSH access to the S15, but also changes to settings from the cgminer API.  After a good deal of work, they were able to ensure that the changes to the S15 were persistent.  

But it really shouldn't have to be this way.  When customers purchase ASIC mining devices, they should have access to the full functionality of the device, and all open-source compiled binaries should have their source code published so that users can modify their devices as they see fit.   


# ASICs as Open Platforms



