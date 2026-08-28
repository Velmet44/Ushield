# UShield

A compact USB security dongle with three physical modes: **OFF**, **POWER ONLY**, and **POWER + DATA**. It gives you direct control over what a connected USB device can access, with built-in ESD protection, power monitoring, and status indicators. No software or drivers are needed.

Total Time : ~9hrs

Software : EaseEDA

I worked on this for 2 days (one of them was full other i had school)

# DAY 1

Morning - I started thinking of an idea, settled on this one, then started work on the schematic
        - I chose all the components and locked in the logics - like what the 3 button states do, LED indicators, etc
        - I prepared thruh table and logic for oversurge protection
        - I found all the components i needed from LCSC ( i chose lcsc because it is the main provider JLC PCB uses for assembly)

Afternoon - I started wiring the components in the schematic, this took a long time, it was very complex
          - I decided normal Wiring was too complex for this, so i scraped what i had and started using nets and I seperated component clustures based on function
          - I finished about 40 percent wiring, then took a break

Evening & Night - I continued work on circuit, hit a few problems - like powersurge protection logic, component availability
                - I fianally finished teh oversurge protection part - this was the longest for me
                - fixed the rgb led controler by replacing the old one with new one which has dual channel (earlier i was using 2 single channel - which was causing wiring issues)
                - Almost done with the circuit

        

# DAY 2

Today I had school, so less time, I woke up pretty early

Morning - I started assembling components in pcb
        - Realised i had no chance to fit all of them in a resonable board size and didnt know what to do
        - I did some thinking, and decided to switch out all my 0603 and 0805 smd components for 0402 ones
        - Fianally got enough space, and finished arranging everything
        - Knew I couldnt finish everything in 30 mins, so i asked for an extention, got it

Evening - I started routing, it was so hard, there were too many components, this was my first time making such a dense pcb. I even tried autorouting.
        - (PS, now only I found out how to attach images to this file)
        <img width="1188" height="395" alt="image" src="https://github.com/user-attachments/assets/51d06e31-3a0c-4449-833f-77f917d7e8fb" />
        - I decided to rearrange all the components
        <img width="1125" height="361" alt="image" src="https://github.com/user-attachments/assets/47b35c84-0024-45ab-b59d-842e9cf5827a" />
        - Now autorouting worked ( i used an external auto router - FreeRouter ) and everything is connected
        - Took a Break
        
Night - I did some final checking and logical simulations to make sure it will work
      - then I worked on some design of the pcb (spent like 5 mins)
      - I started writing a Readme, Preparing The files for the Repo, etc
      - I finished and submitted!

<img width="1140" height="421" alt="image" src="https://github.com/user-attachments/assets/b47a03a9-6b09-4c1d-8b6c-7ff79c4e0ab3" />
<img width="1152" height="391" alt="image" src="https://github.com/user-attachments/assets/d349ab9c-479c-4994-8f95-089c5ad420e7" />
<img width="1102" height="392" alt="image" src="https://github.com/user-attachments/assets/daa3eca2-a419-46fd-94b7-c071d1b16ea2" />
<img width="1169" height="827" alt="Schematic_Dongle001_2026-08-28 (1)" src="https://github.com/user-attachments/assets/d03087a6-0b5b-498b-94c3-5d31f505fb3e" />




