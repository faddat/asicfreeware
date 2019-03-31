# ASICs as an open platform

NB:  This story comes from my involvement in a number of Telegram chats with people working to pry open hardware platforms that have been intentionally closed by their makers.  It should absolutely be understood as advocating for a certain point of view with regard to how software should work on ASIC mining platforms.  Advocacy for open platforms is my express intent, and the intent of the people I've been working with on this.  

You can join the conversation here:  https://t.me/ExploitS15

# S15 vs. S9: Automation

Recently, the Bitmain S15 was released.  It was another in a long line of great miners from Bitmain, except that users were unable to use SSH to configure the miner, AND users were unable to use the cgminer API to configure the miner.  What this means is that purchasers of the S15 are stuck doing these tasks by hand through the WebUI, specifally:

* Setting the IP address
* Setting the mining pool configuration
* Changing settings after the fact

With both SSH and cgminer API access on the S9, these changes could be automated.  On the S15 they need to be done by hand, which massively complicates setup.  

Additonally, there's been no word from Bitmain as to why these changes were made, only that they are "expected behavior"

# ASICs as Open Platforms




