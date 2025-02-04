# Better Way Electronics - PS5 NOR Tool
 
![BwE](https://webtools.bwe.dev/img/ps5.png)

## Introduction ##
	I am BwE of betterwayelectronics.com.au and I have been creating software to validate the PlayStation's flash since 2008 with the help of psdevwiki.com :)
	I also repair consoles locally in Australia and have been doing that since 2008 also. I am only recently slowing that down due to commitments with a PhD I am undertaking.

## FAQ ##

### Why isn't it free? ###
	This program is targeted towards businesses with bulk amounts of PS5s to repair. My products also come with support and continued development.
 	You can however use this program online at a huge discount: https://validate.betterwayelectronics.com.au/
	
### Will you add more features? ###
	More features are added whenever I have time to experiment with my PS5s here and or when I get a large amount of PS5 dumps from the public.

### Will this diagnose hardware issues? ###

	No, that is the PS5 Code Reader (https://betterwayelectronics.com.au/ps5codereader) - You can buy that and this program together as a package and save 15%!

### Your program is a VIRUS/SPYWARE WAAAH! ###
	I protect my programs with Themida. The problem with this is that heuristically some AV software see it as a threat.
	This is totally fine and normal, but also very annoying and unavoidable. 
	
	Visit https://betterwayelectronics.com.au/virus.html for more information!
	
## TLDR ##

* Will this fix my BLOD? It depends, if the console beeps once and flashes briefly then theres a higher chance. Same if there is no beep at all.
* Will this prove my BLOD is software based? Yes, if the dump comes up 100% valid then it is likely a hardware issue.


  ## NOR Menu: ##
	
	1 - Select Different Dump
	
		Return to Main Menu!
		
	2 - Extract Selected Dump
		
		Extract the individual files within the NOR itself
	
	3 - Re-Generate Dump
	
		Attempts to make an entirely fresh dump, but with your consoles important data within. Will likely fix any corruption you may had, but this process is not perfect.
		Now supports all firmwares and all SKU's but needs more testing. Let me know of any issues, updates to the PS5 FW may require updates to this feature.
	
	4 - Switch Between Disc/Digital
	
		Only uses flags within the dump itself to change whether it is a disc or digital console. May fix SU-101312-8 errors during updates.
		
	5 - IDU Toggle
	
		Simply enable and disable IDU Mode. Use at own risk!
		
	6 - Data Transfer/Harvest Data
	
		The PS5 will not boot and will beep once if your MAC address (or its hash) is corrupted, harvesting one from another console is the only solution as it cannot be generated/modified.
		Another use for this is if you have one working dump and want to transfer its key data (MAC, Serial, SKU, Board IDs) to a corrupt one. It will let you select which data you want to transfer over and will make a patch.
		I would still recommend using the re-generator process instead of your own dump as it patches significantly more, but this is a valuable alternative should it fail, though a lot of per-console data will be gone forever.
		
	7 - Change/Patch Southbridge
	
		Fix your current Southbridge or patch it from one with a different version. This helps facilitate swapping between different types of Southbridge chip. 
		Illustration provided on what to mask on the board for this to work.
		
	8 - Validate + Statistics
		
		Attempts to validate each file/area within the PS5 based on various aspects such as hash, entropy, statistics, repetition, block validation etc.
	
		Also uses aggregate statistical data of the entire dump to determine if the console is significantly corrupt or not.

## File Information: ##
    File MD5: 2B427A27E8BF07F4EE30E56746B134E4
    Technical Support: bweps5readme@betterwayelectronics.com.au
    
    System Requirements:
    	Minimum 4 CPU Threads
    	Windows XP, 7-11 (64bit) 
    	100mb+ Storage Space
    
    Archive Password:
    BwE
	
## Version History: ##
	> Client
	1.0.1 (14/10/24) Bug Fix
	1.0.0 (13/10/24) WebTools Version Release! Main App Don't Need Updating - It Is Now Auto Updated & Cloud Based!
	
	> Main App
	1.3.0 (3/1/25) Updated All Patches, Updated Regenerator, Updated Validations to 10.40
	1.2.8 (19/8/24) Added Thousands Of New Validations, Bug Fixes
	1.2.7 (21/6/24) Significantly Updated Validations, Updated Re-Generator, Updated Southbridge Patcher, Other Internal Changes
	1.2.6 (1/4/24) Significantly Updated Validations, Updated Re-Generator, Updated Southbridge Patcher, Updated Bulk Extractor
	1.2.5 (11/2/24) Significantly Updated Validations, Updated Re-Generator, Changed MAC Harvester to Data Transfer/Harvest, Fixed Bulk MD5 Output.
	1.2.4 (18/1/24) Updated Validations, Bug Fixes
	1.2.3 (3/1/24) Updated Validations, Updated Patcher, UI Fixes (Text & Menu)
	1.2.2 (21/12/23) Updated Re-Generator (New Method), Updated Validations.
	1.2.1 (11/12/23) Added Southbridge Patcher, Completed NVS Validations (Alpha), Updated Existing Validations, Added Statistics For Bulk Tools, Updated Re-generator, Fixed Bugs Throughout
	1.2.0 (19/11/23) Added More Validations, Changed Validation Method (Testing)
	1.1.9 (14/11/23) Added 2000 Support (Re-Generator & Validation), Added Some NVS Validations (Will Complete Later), Updated Overall Validations (Rehaul), Fixed Connection Issues, Fixed File Handling Issues, Other Small Bug Fixes.
	1.1.8 (1/11/23) Added Repetition Checks, Added WiFi MAC, Updated MAC Harvester, Updated Bulk Tools, Updated Re-generator, Improved Version Detection, Improved Extraction, Improved Validation, Fixed Bulk Tools Bug.
	1.1.7 (22/10/23) Updated Re-Generator (Better 1200 Support)
	1.1.6 (21/10/23) Significantly Updated Validations, Added Dump Extractor, Added Dump Patcher, Reworked Bulk Tools Menu, Added Bulk Extractor
	1.1.5 (5/9/23) Updated Menu, Updated Validations1
	1.1.4 (7/8/23) Updated Re-generator, Updated Validations, Other Small Updates/Fixes
	1.1.3 (3/8/23) Updated MAC Harvester (1200 Issue)
	1.1.2 (2/8/23) Updated To Suit Latest PS5 FW, Better Firmware Handling (Current & Past), Updated Comparison Tool (Better Outputs, More Options)
	1.1.1 (23/7/23) Fixed MAC Harvester, Other Small Fixes.
	1.1.0 (18/7/23) IDU Mode Toggle, Fixed Input Issues, Fixed NOR Uploading (Please Re-Upload!)
	1.0.9 (12/7/23) HWID Generator Update, Better Support for Chinese Systems
	1.0.8 (10/7/23) Added MAC Harvesting, Bug Fixes
	1.0.7 (17/6/23) Better 1200 & FW 6.00+ Validation & Generation
	1.0.6 (11/6/23) Bug Fixes, Updated HWID Generation
	1.0.5 (19/5/23) Updated Re-Generation Process (Full/Partial Methods), Updated Validations
	1.0.4 (17/5/23) Updated Validations, Bug Fixes
	1.0.3 (15/5/23) Total Rebuild of Re-Generation Process (Full FW/SKU Support), Update to Statistics Validation, Added File/Area Validation, Menu Fixes
	1.0.2 (3/5/23) Added USB Licensing Support
	1.0.1 (21/4/23) Updated Generation Process
	1.0.0 (18/4/23) First Release!

 ### Greetz/Credit: ###

 	Thailand (Xohke!)
	omgitsben
	PS3/PS4 Dev Wiki (+ Its Contributors)
	3absiso
	Totte
	Palestine!
	Hoea
	DigiMod 
	johnnydebt
	SCE
	You! 

    Proudly made in Perl with Notepad++ by BwE, alone </3

## Links ##

### Support/Donate: ###
https://www.buymeacoffee.com/BwE

### Console Repair Discord: ###
- https://discord.com/servers/console-repair-discord-754165317961383997
- https://discord.gg/pXeUHMy

### Videos Featuring My Program: ###	
- https://www.youtube.com/watch?v=hcmMSYmwSUQ <--- My Video!
- https://www.youtube.com/watch?v=noS8wfZA99g <--- My Other Video!
- https://www.youtube.com/watch?v=NDNld92tsZc <--- My PS5 Video
- https://www.youtube.com/watch?v=cegGCQwKTtU <--- My Code Reader & NOR Tools Video
- https://www.youtube.com/watch?v=fE4qGHJyX8E
- https://www.youtube.com/watch?v=q1F0AL3ttjY
- https://www.youtube.com/watch?v=W7RpkG5hiA0
- https://www.youtube.com/watch?v=2hXO60rUt40
- https://www.youtube.com/watch?v=D8-AMvsfadM (Uncredited)
- https://www.youtube.com/watch?v=syfiph70reQ
- https://www.youtube.com/watch?v=NBktKSx4FzQ
- https://www.youtube.com/watch?v=LCOUepj5_8o
- https://www.youtube.com/watch?v=GXOBX6BDg0I
- https://www.youtube.com/watch?v=p8DyudhA7ME
- https://www.youtube.com/watch?v=1gk7HtYih84
- https://www.youtube.com/watch?v=m3wgiudcTEA
- https://www.youtube.com/watch?v=EISO-t2fnMw
- https://www.youtube.com/watch?v=Yal7cwdIKCg
- https://www.youtube.com/watch?v=m5ZUEyya82g
- https://www.youtube.com/watch?v=gHifHpquN6E
- https://www.youtube.com/watch?v=laxB_D80nJE
- https://www.youtube.com/watch?v=7D4Zte3vzvg 
- https://www.youtube.com/watch?v=35DFGCim_WY
- https://www.youtube.com/watch?v=m9nopeQw6dI (Uncredited)
- https://www.youtube.com/watch?v=mSiMdqTJTk8 (Uncredited - Spanish)
- https://www.youtube.com/watch?v=mEDRb-XIqlw (Uncredited - Spanish)
- https://www.youtube.com/watch?v=G7Vboawafc4 (Uncredited)
- https://www.youtube.com/watch?v=5q0WWyYNsTs (Uncredited)
- https://www.youtube.com/watch?v=AH-9jE1uDPk
- https://www.youtube.com/watch?v=iSOWV-r_0J4 (Uncredited)
- https://www.youtube.com/watch?v=kol1Zy9xc8I
- https://www.youtube.com/watch?v=AH-9jE1uDPk
- https://www.youtube.com/watch?v=E-ukC-Jjwfg
- https://www.youtube.com/watch?v=QjkbB3lnRLw (Weird)
- https://www.youtube.com/watch?v=A2c2UeM9V3A (Uhhh)
- https://www.youtube.com/watch?v=FAk2oF0cByg
- https://www.youtube.com/watch?v=PLrudwJHycU (Kinda Uncredited)
- https://www.youtube.com/watch?v=bGnEu4UwsU4
- https://www.youtube.com/watch?v=5q0WWyYNsTs (Uncredited)
- https://www.youtube.com/watch?v=ZEwgtvKcB58 (Uncredited)

### Website Featuring My Program: ###
- https://repair.wiki/w/PS4_UART_Guide
- https://wololo.net/tag/bwe/
- http://www.logic-sunrise.com/recherche/bwe/
- https://www.biteyourconsole.net/?s=bwe
- https://psdevwiki.com/ps4/
- https://psx-core.ru/forum/48-3196-3
- https://consolefix.ru/aktivaciya-uart-dlya-diagnostiki-blod/
- https://vlab.su/
- https://gbatemp.net/search/3666652/?q=bwe&o=relevance
- https://gamegaz.com/2022122937784/
- https://www.psxhax.com/threads/release-bwe-ps4-nor-validator.6139/
- https://www.playstationhax.xyz/forums/topic/5259-release-bwe-ps4-nor-validator/
- https://www.psx-place.com/threads/tutorial-how-to-take-a-nor-backup-on-every-ps4.28070/
- https://tieba.baidu.com/p/8196671153
- https://yoschi.cc/gaming/es-ist-anscheinend-moeglich-ihre-ps4-ohne-backup/
- https://psx-core.ru/forum/48-3196-5

### My Websites: ###
- https://www.betterwayelectronics.com.au/
- https://instagram.com/betterwayelectronics
- https://github.com/BetterWayElectronics/
- https://twitter.com/BwE_Dev
- http://www.ps5repair.com.au/

## Purchase Link ##

If you are a commercial user, I highly suggest you buy the software here: https://betterwayelectronics.com.au/bweps4norvalidator
Otherwise there is a cheaper alternative available at https://webtools.bwe.dev

I also sell Syscon writing hardware here: https://betterwayelectronics.com.au/#hardware

After purchase, provide your HWID via the provided application to obtain your license key.

