# Variable dose scheduling and antibiotic resistance evolution in the EVolutionary biorEactor (EVE)

John Joyce<sup>1</sup>, Dr. Rowan Barker-Clarke<sup>2</sup>, Dr. Jacob Scott<sup>2</sup>

<sup>1</sup>Hawken High School, Gates Mills, Ohio; <sup>2</sup>Translational Hematology & Oncology Research, Cleveland Clinic Lerner Research Institute, Cleveland, Ohio

## Abstract
Multi-antibiotic resistance, occurring when a bacteria becomes tolerant to standard treatment through evolution and selection pressure, is a worldwide problem. An essential component of combating antibiotic resistance requires understanding multiple factors: ecological competition between bacteria, the prevalence and profiles of pre-existing resistance, selection pressure variability due to both varying drug uptake and schedule adherence to prescribed antibiotics, and more. To better model and address these factors in the lab, we looked to advance the in-silico and in-vitro simulations of variable dose uptake and scheduling.

In our work we used the EVE, a small, experimental, raspberry-pi based bioreactor that can pump drugs or nutrients into bacterial culture units. This study focuses on dose scheduling, and we used Python to develop mathematical models antibiotic resistance evolution to form predictions. At the same time, we developed new adaptive EVE algorithms to simulate, in-vitro, different pharmacodynamics and dosing schedules and their adherence. To study the effect dosing regimens have on the evolution of antibiotic resistance, we created three separate control algorithms for the EVE to simulate dosing processes, all of which work to automate dosing processes in a controlled setting. We then experimentally verified our predictions about the effects of different cefotaxime dosing regimens on the co-evolution of combinations of different wildtype and resistant Weinreich E. coli strains in the EVE.

## Introduction
Start with an introduction into antibiotic resistance and bioreactors, as well as how they interact with one another and some historical background.

Now into some of the biology - get into some background surrounding evolutionary tradeoffs, and some general background surrounding pharmacodynamics. Then also dive into variable dose scheduling, and how/why thats important. Basically, the first half of the abstract.

Antibiotic resistance is a worldwide problem associated with nearly 5 million deaths in 2019 alone1. Resistance occurs when different diseases become tolerant to drugs and other pharmaceutical treatments and was first documented when bacteria became resistant to antibiotics2. As drugs evolve it is vital to also evolve in our treatment techniques, such as scheduling, dosing, treatment methods, and more3. Furthermore, mathematical models and determining different drug and environment parameters is important for conveying information, as well as analyzing trends. An important component of minimizing antibiotic resistance is variable dose scheduling – a concept that relates to the evolution of antibiotic resistance in bacteria via dose timing, dose quantity, and dose type to try to and optimize dosing regimens in clinical treatment4. There are many examples of why variable dose scheduling is important: too much drug too fast could result in deleterious impacts on the patient but not leave much room for resistance, and slowly ramping up dosage could create a more resistant population, but constant dosing and intervals will quickly make the drug ineffective5. Hence why having a practical way of analyzing the effect different regimens have on the evolution of resistance is crucial, otherwise treatment becomes null.

I will be working with a low-cost morbidostat called the EVolutionary biorEactor (EVE), which is unique due to its smaller size and low cost which can provide extra educational benefits3. The EVE is a bioreactor that uses antibiotics to study the growth of bacteria and its evolution of antibiotic resistance, and uses a control algorithm to determine which media to introduce (i.e., antibiotic rich media or bacteria rich media), how much to introduce, and when to introduce it into the culture. The control algorithms can use a feedback loop of optical density, drug concentration, or introduce drug at pre-determined intervals. Initially, the EVE was programmed to be a morbidostat – a continuous culture device that measures the optical density of the microbial population, and accordingly adjusts the drug concentration to maintain a near constant growth rate3. However, our work has expanded the EVE to test things such as variable dose scheduling. The EVE’s feedback loops and experimental nature allows for the testing of many different control algorithms and “schedules”. This makes the EVE especially useful for studying drug scheduling and dosing, and how that impacts the evolution of drug resistance. The EVE can have several bacterial mediums being grown in a vial with controlled conditions (Figure 1A). The software algorithms maintain these controlled conditions by rotating the magnetic stir bars, introducing fresh medium into the vials with the pumps, monitoring the population growth via absorbance measurements, and introducing selective medium when these absorbance measurements exceed a certain value. 

### Variable Dose Scheduling


### The EVolutionary biorEactor (EVE)
Then the second half of the abstract. Start with claim about what we are trying to see short sentence - spec about VDS. Also about how we know similar research and results, but the question is whether or not we can use the eve. explain how the EVE is unique, with the ability to simulate a chemostat, morbidostat, turbidostat, etc. This can also provide a bit of background into how we created and used different algorithms. Then get into the experimental use value and cost effectiveness, drawing comparisons from other similar devices in the field and noting its open-source capabilities. 

Fig 1 - 

(A) Reservoirs containing permissive (i.e., drug-free) and selective growth media are each connected to a set of pumps. The pumps are controlled by the system displayed in figure B. These pumps then automatically feed into the culture unit (CU) vial, and an equivalent amount of waste is pumped out to medium pumped in. 

(B) The continues process is controlled by the Raspberry PI – on which the control algorithm, graphing process, and data is stored. The EVE WebUI is what controls the experiment, an easy to use UI which allows the user to test the pumps, edit the EVE config, and run the experiment. The PCB is linked to the incubator and records the optical density of the culture media.


## Methods



## Results


## Discussion

## Data Availability
## Refrences
