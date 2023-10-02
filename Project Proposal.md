# EEB313 Project Proposal - Malaria Modelling 

One of the oldest diseases affecting humankind, malaria is one of the severe challenges… sub-saharan africa… Caused by the protozoan Plasmodium spp., as many as triple the amount of deaths from armed conflicts… Efforts at reducing deaths include measures such as insecticide treated bed nets, artemisinin therapies, and indoor insecticide spraying. We are investigating… 

Malaria margaret philips…

Title: (clear and informative)
- Title for the project (clear title that frames the work we are trying to do)
 
  Introduction:
  - provide background context as to what the problem is and why it is essential we are doing the research
  - including statistics here about the problem is good
 
  Objective:
  **What are we researching?**
  - what are the goals of this modeling project? We need to narrow this down...
    - are we testing for virulence between different types of parasites? I.e. P. falciparum (most common in fatal cases), P. vivax, P. ovale,
      P. malariae, P. knowlesi (not relevant, found in Asia + infects macaques, animal --> human dubbed zoonotic malaria)
    - P. falciparum has already been proven to be the most deadly parasite bc it induces extreme hemolysis of RBCs at all levels
      (Wtf does this mean: red blood cells are recognized as infected (high levels of parasites in blood), so the body destroys them
      --> this results in severe anemia as the body destroys too many rbcs.
    - https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4800101/#:~:text=Unlike%20other%20Plasmodium%20species%2C%20P,falciparum%20infected%20children%20is%20high.
    - P. falciparum is also the most commonly found parasite in African countries (south of the sahara)
    - https://www.who.int/news-room/fact-sheets/detail/malaria#:~:text=P.%20falciparum%20is%20the%20deadliest,outside%20of%20sub%2DSaharan%20Africa.
    - If we aren't testing for the virulence, are we testing for the distribution of different malaria parasites?? (WE GOTTA NARROW THIS DOWN)

   **MODELLING OBJECTIVES**
  - what specific question are we answering with this model? (What is the model itself we will be using)
  - what variables are we measuring? How will we represent/track these variables?
      - what type of model will we use?
   
 There are MANY types of models we can use
 
 **Compartmental** --> divides population into sub-compartments
- SIR (susceptible, infected, recovered) or SEIR (susceptible, exposed, infected, recovered) simulate malaria spread through population

**Differential Equation**(aka Sam carries with thiccc math brain) --> dynamics of malaria transmission
- requires variables that measure transmission rate, recovery rate, and population demographics
- not sure how viable this is, the data on the website doesn't have these stats

**Regression Analysis** --> used to identify factors relating to malaria incidence (this might be worth looking into)
- requires variables that describe climate, population density, and socio-economic factors

**Age-structured models** (commonly used epidemiology model) --> model age-specific susceptibility/immunity to malaria infection, survival rate
THERE ARE MANY MORE MODELS, HOWEVER THESE ARE SOME THAT I HAVE SEEN IMPLEMENTED IN RESEARCH PAPERS REGARDING MALARIA INCIDENCE


Malaria is a deadly mosquito-borne herpesvirus caused by Plasmodium spp. As a vector borne disease, malaria is primarily transmitted by mosquitoes (Anopheles), whose bite allows the entry of Plasmodium into the bloodstream. Once in a human host, malaria presents as a set of non-specific symptoms, such as diarrhoea, fever, vomiting, and pulmonary complications. In many cases, malaria can lead to death -  UNICEF reported more than 600,000 malaria-related fatalities in 2021 alone. Unfortunately, children under the age of 5 from sub-Saharan Africa represent a disproportionate amount of these cases. 
Interestingly, patient outcomes vary depending on the species of Plasmodium causing the infection. In our study, we aim to investigate and model the incidence rate, severity, and outcomes of malaria across different African regions as a product of Plasmodium species. Further, we relate these differences to regional characteristics such as temperature, rainfall, and proximity to water bodies, in an effort to better explain case count in specific provinces. We expect to see a positive correlation between malaria deaths and rainfall/temperature. As such, we predict that temperature-sensitive Plasmodium falciparum, the most deadly malaria parasite, will primarily affect…


Phillips MA, Burrows JN, Manyando C, van Huijsduijnen RH, Van Voorhis WC, Wells TNC. Malaria. (2017). Nat Rev Dis Primers. 3:17050. 10.1038/nrdp.2017.50.
https://data.unicef.org/topic/child-health/malaria/#:~:text=Nearly%20every%20minute%2C%20a%20child%20under%20five%20dies%20of%20malaria,to%20619%2C000%20deaths%20in%20total.
Carvalho-Tavares, J. (2013). Malaria. Morgan & Claypool. 1615046364, 9781615046362





