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

#### 2) Choose Integrated components:     
Try to choose and use the most integrated components - RF ICs, Baluns, Filters, etc.     
Examples of RF ICs - CC2650, CC1310, AT86RF215, nRF24L01P(+) ans so many more integrated RF ICs are available...        

#### 3) 50 Ohms everywhere:     
Try to match everything to 50 ohms. If a component is not 50 ohms I/O or whatever, convert it to 50 ohms.     
How? - Refer to it's Datasheet (Matching/Application Circuit)
* Follow Manufacturer Recommendations (for matching)
* Route RF first

