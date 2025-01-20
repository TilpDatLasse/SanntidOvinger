Problemet er at de to funksjonenen prøver å endre i samtidig (data race), og da kan vi ikke vøre helt sikre på hva som skjer.  

### C
Bruker mutexes fordi vi bare trenger p holde styr på èn variabel. Dermed er det ikke noe problem å låse vareiebelen helt mens vi endrer den. semafor blir unødvendig komplisert her.