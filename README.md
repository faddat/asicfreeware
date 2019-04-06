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


# Why should mining hardware be sold as an open platform, with hardware and software decoupled?

Without the ability to modify the code running on hardware, the user really isn’t buying hardware at all.  They’re paying for hardware+software with no right to modify the software.  Today’s ASICs have fairly capable Linux computers that control the ASIC chips themselves.  If software was entirely unrestricted, ASIC owners and competitive vendors would be free to develop tools and systems that suit their needs, both open and closed.  

In this regard, our complaint is really about ownership.  We BUY ASICs, and we would like to be able to use them in any way that we see fit.  The only way that owners are going to be able to use their ASICs for any purpose they’d like, without restriction, is for hardware manufacturers to return to their actual role: making hardware.  That hardware could ship with an initial distribution of software, or not.  We’re all quite satisfied with the hardware that we buy, but we’re in no way satisfied with the software that comes with it.  

# How about that MicroSD slot?

Most miners ship with a microSD card slot.  In a more ideal world, that MicroSD card slot would be active by default when there’s a microSD in it, instead of needing to change a number of jumpers on the miner control board.  The Miner could then boot from the SD card any time there’s an SD card in it, and the user could try out various flavors of both open and closed mining OSes.  


If this Pi were a miner, it would attempt to boot from the SD Card



If this Pi were a miner, it would run manufacturer firmware, as there’s no installed SD card



The main thing here isn’t software openness, even though Bitmain should certainly open its firmware and cgminer implementation.  Instead, the main thing is the openness of the miner as a hardware platform, and the user’s freedom to run whatever software they’d like on the mining machine that they bought with their hard-earned money.  Making the MicroSD card slot function in this manner would also make it easier for large farms to identify individual machines and manage their setup statically.  Additionally, if all machines run the same image, a machine like this one could prove helpful:





This machine clones SD or MicroSD cards.  It could be easily used to roll out custom software across a mining farm in a timely manner.  

With MicroSD boot enabled by default, it would also be possible for an OWNER of ASICs to create a script that creates images with a range of IP addresses, which get flashed onto a series of labeled MicroSD cards.  This would enhance customization and allow miners to run more secure software, as well as allowing owners to control their miners more effectively.  

## What does all this look like, practically speaking?

* Linux 5.0 on your miner (instead of 2.6)
* Security benefits
* Miners with bespoke configurations
* Miners that natively support software networks like ZeroTier for secure, easy user access
* Miners that don’t have a WebUI because they don’t need one because they’re driven by the same software that drives the mine
* Limitless creativity in terms of what a miner can and cannot do
* Faster, Easier setup
* Easier to use layer2 networks by creating bespoke images for each miner using a script
* Automated maintenance and configuration changes
* More robust 
* Mines that work *exactly* as their OWNERS want them to
* Miners that update their own software from servers their OWNERS control.


Thanks for reading!  
You can reach me at jacob@droneenergy.com 

