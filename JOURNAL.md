# UShield

A compact USB security dongle with three physical modes: **OFF**, **POWER ONLY**, and **POWER + DATA**. It gives you direct control over what a connected USB device can access, with built-in ESD protection, power monitoring, and status indicators. No software or drivers are needed.

Total Time : ~10.5hrs

Software : EaseEDA

I worked on this for 2 days (one of them was full other i had school)

# DAY 1

Morning - I started thinking of an idea, settled on this one, then started work on the schematic
        - I chose all the components and locked in the logics - like what the 3 button states do, LED indicators, etc
        - I prepared thruh table and logic for oversurge protection
        - I found all the components i needed from LCSC ( i chose lcsc because it is the main provider JLC PCB uses for assembly)
        - **Total time : ~2.5 hrs**

<img width="1169" height="826" alt="Schematic_Dongle001_2026-08-29" src="https://github.com/user-attachments/assets/aad14be7-e7e6-4b3a-8f5b-4e7d0040088a" />



Afternoon - I started wiring the components in the schematic, this took a long time, it was very complex
          - I decided normal Wiring was too complex for this, so i scraped what i had and started using nets and I seperated component clustures based on function
          - I finished about 40 percent wiring, then took a break
          - **Total time : ~2 hrs**

<img width="716" height="496" alt="image" src="https://github.com/user-attachments/assets/b3a7ed7e-86e5-4774-9da4-c1005870060a" />


Evening & Night - I continued work on circuit, hit a few problems - like powersurge protection logic, component availability
                - I fianally finished the oversurge protection part - this was the longest for me
                - fixed the rgb led controler by replacing the old one with new one which has dual channel (earlier i was using 2 single channel - which was causing wiring issues)
                - Almost done with the circuit
                - **Total time : ~1 hr**

<img width="1169" height="827" alt="Schematic_Dongle001_2026-08-29 (1)" src="https://github.com/user-attachments/assets/d1fb063a-d240-4202-8f62-5aa4db89fbfb" />


# DAY 2

Today I had school, so less time, I woke up pretty early

Morning - I started assembling components in pcb
        - Realised i had no chance to fit all of them in a resonable board size and didnt know what to do
        - I did some thinking, and decided to switch out all my 0603 and 0805 smd components for 0402 ones
        - Fianally got enough space, and finished arranging everything
        - Knew I couldnt finish everything in 30 mins, so i asked for an extention, got it
        - **Total time : ~45 mins**

<img width="1117" height="417" alt="image" src="https://github.com/user-attachments/assets/77b3b025-37fe-4006-8672-9c166169f8fd" />



Evening - I started routing, it was so hard, there were too many components, this was my first time making such a dense pcb. I even tried autorouting.
        - (PS, now only I found out how to attach images to this file)
        <img width="1188" height="395" alt="image" src="https://github.com/user-attachments/assets/51d06e31-3a0c-4449-833f-77f917d7e8fb" />
        - I decided to rearrange all the components
        <img width="1125" height="361" alt="image" src="https://github.com/user-attachments/assets/47b35c84-0024-45ab-b59d-842e9cf5827a" />
        - Now autorouting worked ( i used an external auto router - FreeRouter ) and everything is connected
        - Took a Break
        - **Total time : ~2 hrs**

<img width="902" height="872" alt="image" src="https://github.com/user-attachments/assets/ea318af8-0701-4cab-aac3-f13873540a38" />


        
Night - I did some final checking and logical simulations to make sure it will work
      - then I worked on some design of the pcb (spent like 5 mins)
      - I started writing a Readme, Preparing The files for the Repo, etc
      - I finished and submitted!
      - **Total time : ~1 hrs**


**This is the Fabrication Quote:**

<img width="1313" height="760" alt="image" src="https://github.com/user-attachments/assets/419b2054-2cf7-43c2-b735-b28e7dd7872d" />



# Day 3

Morning - Was asked some changes:(route manually is the main thing, rest are for readme, journal and fabrication)
        - I started investigating why the original Quote was high, found that the 2 usb conectors were big and could only be assembled with PCBA standard, so when i added the BOM, it changed my assembly mode from economic to standard, i decided that I will manually solder those 2 things, and switched back to PCBA economic. But while I was checking this, I found that 2 of the componwents i need are out of stock, so i dont know what to do, they are 0402 smd components, so i cant solder on my own :(
        - Then i tried to route maually, almost finished but i couldnt find any way to rout like 8 of them. So i had to scrap it. here is a LAPSE of **a part** of me triying to route : https://lapse.hackclub.com/timelapse/xJ6XUpmo0znR
        - **Total time : 1.5 hrs**

<img width="1715" height="692" alt="image" src="https://github.com/user-attachments/assets/5d8596bf-67dd-42d9-aba3-029318b6a795" />

        

Night - I got some more time today after school and some other activities, decided to work on the docs, (mainly Journal), I calculated times for each session, and collected screenshots for day 1.
      - Finished almost all required changes except manual routing. It is really late now, so i decided I would finish that the next day, and i plan to use LAPSE for the first time on this  
      - **Total time : ~1 hr**


      
# Day 4

Morning - Started manuall routing (With LAPSE recording, see end of Day 4 for timelapse link)
        - Again got stuck at the same few connections
        - Decided to Continue in the evening(Had school).
        - Total time : ~1 hr

Evening - Continued Routing
        - Finally adjusted some connections and managed to rout up everything!
        - **Here is the LAPSE link** : https://lapse.hackclub.com/timelapse/zhhLOVxRxyuS (i recorded half during morning, pused it and finished in the evening)
        - I then started preparing all the files for the repo - pcb, 3d, new quote with correct settings etc
        - While getting quote, I found replacement for one of them, but other, still no solution
<img width="1917" height="1011" alt="image" src="https://github.com/user-attachments/assets/6a137657-a0c9-45cd-8623-cfa3a6a5e864" />
        -I also just found that one of my components are too small for PCBA standard, so i have to replace that component with a new one:
<img width="870" height="371" alt="image" src="https://github.com/user-attachments/assets/c443dc63-2de3-4353-9f91-b04517c92664" />
        


# Day 5

I didnt work on the next day, very busy. this is the day after that:

Evening - Finished routing
        - Did Art
        - Updated README and updated repo files
        - now only need to get quote from JLC


Night - I got quote, still one component tall or something so they wont assemble in economic, si ill manually solder that one after buying, one component out of stock, taht also i will buy seperately and solder. here are the quotes:

<img width="1816" height="857" alt="image" src="https://github.com/user-attachments/assets/98f586ec-f5e8-4274-9c5b-7c6c34f8b289" />
<img width="1746" height="872" alt="image" src="https://github.com/user-attachments/assets/ec5921fb-076b-42e7-b4bc-18376fa67c95" />


Night - I got quote, another compi
