# RF Circuit Design
#### [Link to the Video](https://youtu.be/TnRn3Kn_aXg)         

### Five Rules: 
#### 1) Use 4 Layers:      
* Top (RF and Signals)          
* GND just below 1                 
* VCC above the bottom (15 on Eagle)           
* Bottom (Signals)             

* Use a consistent stack-up            
* Dedicate entire inner layers to unbroken power supply planes           
* Keep RF Signals on Top     

##### 4-Layer Board stackup:   
The 4 layer board stackup is as follows:      
* 1 mil solder resist      
* 1 oz Cu (1.4 mil)    
* 6.7 mil prepreg     
* 0.5 oz Cu (0.7 mil)   
* 47 mil Core     
* 0.5 oz Cu (0.7 mil)           
* 6.7 mil prepreg        
* 1 oz Cu (1.4 mil)         
* 1 mil solder resist         

[Setting up Multi-layer on Eagle](https://youtu.be/0sVUkjXbqrM)            

#### 2) Choose Integrated components:     
Try to choose and use the most integrated components - RF ICs, Baluns, Filters, etc.     
Examples of RF ICs - CC2650, CC1310, AT86RF215, nRF24L01P(+) ans so many more integrated RF ICs are available...        

#### 3) 50 Ohms everywhere:     
Try to match everything to 50 ohms. If a component is not 50 ohms I/O or whatever, convert it to 50 ohms.     
How? - Refer to it's Datasheet (Matching/Application Circuit)    

* Follow Manufacturer Recommendations (for matching)  -------------  **(4)**      

##### Note: For matching the RF traces on the Top layer of the circuit board to 50 Ohms, they have to be 12 mils wide (Considering the 4 layer board stackup specifications as mentioned above). So, on Eagle, Set - Trace width = 12 mils, Trace thickness = 1.4 mils             

After making your circuit, with all the above rules in mind:       
* Route RF first  --------------  **(5)**    
* Keep RF traces short and direct     
* Keep other signals away from RF (keep buffer zones next to RF traces, try to route other signals considerable away from RF signals)         

