# Trajectory models 

## Background 
This repo is created to share the clinical models DIPS have been using to model patient trajectories. The purpose is to prepare for a potential review of these archetypes. 


## The patient trajectory 

### Background 
Disease is a process. Diagnostics and treatments are processes. Everything in health care is processes. There are several terms defining such processes. Clinical pathways, care plan and protocols are examples on such. 

We introduce the term patient trajectory as a generic concept for any clinical process. The term is an upper-level definition and as such a container for other fine-level INSTRUCTION/ACTION or Task planning defined activities. 

The term trajectory in health care can be defined as the assembling, scheduling, monitoring, and coordinating of all steps necessary to complete the work of patient care .|

The patient trajectory targets the sequence of events and turning points (which they call “critical junctures”) in treatment. Once a trajectory is initiated, there may be intermittent and alternating, acute, stable, unstable, and upward/downward phases. In its purest forms, a patient trajectory has no set course because it is shaped and managed through ongoing interactions of concerned actors . 

Each patient trajectory will be unique and follow different clinical pathways. The intention about this modelling is to cover an overall structured definition about what the trajectory is about and significant steps or turning points along the trajectory. 

The initial models for the concept were developed to standardised “package process” (in Norwegian: “Pakkeforløp”) for cancer diagnostics. The goal for the “package process” is to cut time where possible for the person with a potential cancer. A more detailed description of the process and the implementation is found here: https://github.com/bjornna/dips-ckm/blob/nymaster/doc/kreftpakkeforl%C3%B8p/kreftforlop_dokumentasjon_en.adoc 


## Archetypes 


|Archetype|Description|
|---------|-----------|
|INSTRUCTION.trajectory.v1|	Defines the start of a patient trajectory.|
|ACTION.trajectory_follow_up.v1	|Defines different milestones or tasks performed within a trajectory. The ACTION carry the significant state information about the trajectory. |
|EVALUATION.trajectory_summary|	A summary of the trajectory. This kind of data is persistent by nature. There will most likely be only one such entry within each trajectory. |
|COMPOSITION.trajectory.v1	|Used for compositions which contains information about the initializing/set-up or follow up of trajectories. |
|ADMIN_ENTRY.trajectory_manager.v1	|The healthcare provider responsible for the given trajectory|
|EVALUATION.trajectory_plan.v1	|Defines the overall plan for measurement/milestone events in the patient trajectory|
|openEHR-EHR-ACTION.medication_treatment_follow_up_dips.v1.adl|Used to follow up the state and progress of an order-set within medication|


## Resources
  https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3001102/ 
  https://onlinelibrary.wiley.com/doi/pdf/10.1002/9781118410868.wbehibs282 
