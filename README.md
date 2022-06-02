# Praktikum MD
This repository contains the data for the hands-on Materials Discovery part of the lecture  "VL und Ü - TU Berlin, Datengesteuerte Entdeckung nachhaltiger Baustoffe"

The data has been extracted from the following reference: 

G. Mallikarjuna Rao & T. D. Gunneswara Rao (2018): A quantitative method of approach in designing the mix proportions of fly ash and GGBS-based geopolymer concrete, Australian Journal of Civil Engineering, DOI: 10.1080/14488353.2018.1450716

## Research question
This data set stems from a systematic lab study for selecting mix proportions for fly ash and GGBS- based geopolymer concrete. Very little information is available on complete methodology in designing the fly ash and GGBS-based geopolymer mix. The fly ash and GGBS were activated using sodium silicate and sodium hydroxide as alkaline activator solution. The Na2SiO3/NaOH (alkaline activator) ratio was taken as 2.5 and the concentration of NaOH solution was maintained at 8 M. The main parameters considered in this study were binder content and alkaline solution/ binder ratio for various combinations of fly ash and GGBS. The variables considered in this experimentation include: binder content (360, 420 and 450 kg/m3), proportions of fly ash and GGBS (70–30, 60–40 and 50–50), alkaline solution/binder ratios (0.45, 0.50, 0.55 and 0.60) and curing condition (outdoor curing and oven curing). Results concluded that the GGBS content, alkaline solution/binder ratio and curing condition are found to be most influential parameters on compressive strength and workability of geopolymer concrete. The work presents detailed examples of mix designs for various strengths.

## Your task:
You get 192 geopolymer recipes (digital materials), of which only 10 (randomly selected) materials have been validated in the lab. 
The goal is to discover materials with high compressive strength in the upper 5%. Use a data-driven approach to select the next promising material for validation. Your lab budget is 4 validations! 

The person with the highest average performance wins. <img width="870" alt="Bildschirmfoto 2022-06-02 um 13 47 23" src="https://user-images.githubusercontent.com/71640597/171622654-0f8586c4-6afa-4a3b-b9c6-3e0f6d139cc1.png">


### Overview of the parameters investigated
Binder content: 360, 420, 450
Fly-ash/GGBFS ratio: 70-30, 60-40, 50-50
Alkaline solution/binder ratio: 0.45, 0.5, 0.55, 0.6
Curing: ambient/oven
Fine/coarse aggregate: 774/1091, 811/966, 761/972
-> impact on strength 

### Fixed parameteres
Na2SiO3/NaOH ratio: 2.5 
NaOH: 8 Mol
Aggregates specific gravity
fineness modulus, Curing time 
superplasticizer type & -/binder ratio: Naphthalene-based at 4 wt.%

## Description of data

192 Digital materials, 10 validated in the lab (training data)

### #.  Name			                    Description
0.  Idx_Sample & Mixture Code 	  Index and name of mixture 
1.  FA (kg/m3)		                Fly ash content
2.  GGBFS (kg/m3)		              Slag content
3.  Total powder (kg/m3)	        Weight of powder
4.  Coarse aggregate (kg/m3)	    Weight of coarse aggregate 
5.  Fine aggregate (kg/m3)	      Weight of fine aggregate 
6.  Total aggregates (kg)	        Total weight of aggregates 
7.  NaOH (kg)		                  Weight of sodium hydroxide
8.  Water-eff (kg)		            Weight of water
9.  Weight mixture (kg)	          Total weight of mixture
10. Initial curing temp (C)	      Curing temerature	
11. f,c(28d) (MPa) 		            Target 28 day compressive strength
12. CO2 emissions (kg/m3)	        A-priori carbon footprint

## Optimization targets

#### 1. Single-objective
Target = high strength			
 	𝑓𝑐(28𝑑) > 60,2 𝑀𝑃𝑎 		 (95% 𝑞𝑢𝑎𝑛𝑡𝑖𝑙𝑒 −> 9/192) 
##### Budget: 4 iterations


#### 2. Multi-objective 
Target = high strength & climate friendly 	
	𝑓𝑐(28𝑑) > 55 𝑀𝑃𝑎
		𝐶𝑂2  < 150𝑘𝑔/𝑚3		(95% 𝑞𝑢𝑎𝑛𝑡𝑖𝑙𝑒 −> 9/192) 
##### Budget: 4 iterations

## Start SLAMD

To start SLAMD, follow one of these links:

Link 1: https://slamdbam.herokuapp.com 
Link 2: https://bamslamd.herokuapp.com 

## TO UPLOAD THE "MD_Example.csv" FILE YOU MUST CHANGE THE DELIMETER SETTINGS!!! Choose: Separator: ";" & Decimal delim: ","
