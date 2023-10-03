# EEB313 Project Proposal - DRC Malaria Modelling 

## Leading Question

Malaria is a deadly mosquito-borne herpesvirus caused by Plasmodium spp [1,2]. As a vector borne disease, malaria is primarily transmitted by mosquitoes (Anopheles), whose bite allows the entry of Plasmodium into the bloodstream. Once in a human host, malaria presents as a set of non-specific symptoms, such as diarrhoea, fever, vomiting, and pulmonary complications [1]. In many cases, malaria leads to death - in 2021 alone, UNICEF reported more than 600,000 malaria-related fatalities [3]. Unfortunately, children under the age of 5 were the most vulnerable demographic, comprising a total of 77% of malaria related deaths [3]. The Democratic Republic of the Congo (DRC) is among the hardest hit countries, representing 12% of all global cases in 2021 [4]. Consequently, malaria research is a field of global interest. Besides research into the physiological, immunological, and genetic causes and consequences of malaria, many researchers focus on mathematical modelling as a measure to explain infection/death rates [5]. Such models inform institutional decisions, especially when variables include environmental, social, economic, and migration [5].

## Model Inspiration

For the first part of our project, we are interested in examining the predictive power of the Ross-Macdonald model for malaria transmission. This model is derived from two equations, one of which observes human infections, and the other vector infections (which in this context is mosquitoes) [5,6]. More specifically, this model focuses on the susceptible populations ($S$), the infected population ($I$), and briefly considers the recovered population ($R$). Here is a quick summary of the different variables used within the model:
* $a$: mosquito biting rate,
* $b$: transmission probability from an infectious mosquito to a susceptible human per bite,
* $c$: transmission probability from an infectious human to a susceptible mosquito per bite,
* $m$: ratio of mosquitoes to human,
* $V / H$: number of vectors (mosquitoes) and number of humans,
* $I_v / I_h$: number of infectious vectors and number of infectious humans,
* $S_v / S_h$: number of susceptible vectors and number of susceptible humans,
* $\gamma$: human recovery rate,
* $\mu$: mortality rate of mosquitoes.

Furthermore, the model itself is as follows,

$$\frac{dI_h}{dt} = ab \frac{I_v}{H}S_h - \gamma I_h \ \ \ \ \ \text{and } \ \ \ \ \frac{dI_v}{dt} = ab \frac{I_h}{H}S_v - \mu I_v,$$

where $S_h = H - I_h, S_v = V - I_v,$ and $R_0 = \sqrt{\frac{a^2 bcm}{\gamma\mu}}$. However, the Ross-Macdonald model considers many of 
the parameters to be fixed (e.g., $a$, $b$, and $c$), which is rarely the case in actual populations. Moreover, interpreting these values 
as functions of time might provide greater accuracy in a malaria model. The number of mosquito bites on humans per mosquito per month is 
influenced by both human and environment-driven factors. Consider migration and resource allocation to combat mosquitoes for human factors, 
and precipitation and the temperature for environmental factors [7,8,9]. It would thus be of interest for $a(t)$ to take these values into 
its output. Moreover, $b$ may be impacted by the number of infectious mosquitoe, and the opportunities for infectious mosquitoes to feed 
on succeptible humans. Note that humans can be feeded on several times a day, but that mosquitoes may only feed a finite number of times 
each day. This can be perceived as there being no particular lack or resources, but that one given mosquito can only infect a finite number 
of individuals in a day. Moreover, $c$ may be impacted by quarantining procedures and the virulence of the virus. As such, in the second 
part of our project we will be exploring whether and how incorporating the aforementioned variables impact the predictive value of the 
Ross-Macdonald model. Findings from our research have the potential to present an improved model that may better depict real-life malaria 
cases and perhaps even infer interactions between mechanisms. It will also be of interest to compare our model against the standard 
Ross-Macdonald model to verify possible discrenpsies, and where certain models are more advantageous (one may be overwhelmingly better, 
or these may be advantageous on case-by-case conditions). Should our model prove to accurately ressemble real-life data, it may also be 
of interest to use it for predictive purposes, to enable more insightful approaches to combatting malaria. 

# Citations

1. Phillips MA, Burrows JN, Manyando C, van Huijsduijnen RH, Van Voorhis WC, Wells TNC. Malaria. (2017). Nat Rev Dis Primers. 3:17050. 10.1038/nrdp.2017.50.
2. Tavares, Juliana Carvalho. Malaria. *Morgan*; Claypool, 2013. 
3.  “Malaria in Africa.” UNICEF, 5 May 2023, data.unicef.org/topic/child-health/malaria/#:~:text=Nearly%20every%20minute%2C%20a%20child%20under%20five%20dies%20of%20malaria,to%20619%2C000%20deaths%20in%20total.
4.  “Malaria.” World Health Organization, World Health Organization, 2021, www.who.int/news-room/fact-sheets/detail/malaria.
5.  Mandal, Sandip, et al. “Mathematical models of malaria - A Review.” Malaria Journal, vol. 10, no. 1, 2011, https://doi.org/10.1186/1475-2875-10-202.
6.  Jin, Xiulei, et al. “Mathematical analysis of the Ross–MacDonald model with quarantine.” Bulletin of Mathematical Biology, vol. 82, no. 4, 2020, https://doi.org/10.1007/s11538-020-00723-0. 
7.  “Migration Profile Democratic Republic of Congo.” Migrants Refugees, 4 Aug. 2023, migrants-refugees.va/country-profile/democratic-republic-of-congo/#:~:text=In%201990%20immigrants%20were%202.1,economic%20or%20voluntary%20international%20migrants.
8.  “Overview.” The World Bank, 2023, www.worldbank.org/en/country/drc/overview#:~:text=DRC%20is%20among%20the%20five,in%20SSA%20lives%20in%20DRC.
9.  Castro, Marcia C. “Malaria transmission and prospects for malaria eradication: The role of the environment.” Cold Spring Harbor Perspectives in Medicine, vol. 7, no. 10, 2017, https://doi.org/10.1101/cshperspect.a025601. 
