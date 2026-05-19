# Follow the Money: How EU Research Agenda Influences the Future of Society
a workshop for Future Earth 2026 in Lausanne run by Sciences Citoyennes and Scientists Rebellion France

### WORKSHOP RESOURCES
- [Presentation slides](https://canva.link/78u6piohcxliilk) from Future Earth 2026 that gives background on the Framework Programs and how we can do research differently.
- Link to the [Doc](https://pad.liiib.re/pa27xhM9QrCHpGPwau5G5g?view) with all of the instructions and documentation
- [Binder Link](https://mybinder.org/v2/gh/sciences-citoyennes/Future-Earth-Workshop/HEAD) to run the code directly through a browser
- [ADEME Scenarios](https://www.ademe.fr/les-futurs-en-transition/les-scenarios/) to contextualize the research projects in our wider societal direction



## Background (why this workshop & what does it do?)
#### Current Challenge:

Horizon Europe aims to fund research that tackles climate change, helps achieve the UN's Sustainable Development Goals, and boosts EU competitiveness and growth. Yet a significant portion of its €95.5 billion budget flows to corporations whose business models conflict with these sustainability goals. This contradiction reveals a deeper problem: current funding mechanisms lack meaningful democratic oversight, allowing decisions about our technological futures to bypass citizen input. This workshop investigates this accountability gap by analyzing how Horizon Europe funds are allocated, with particular attention to the outsized role of polluting organizations in shaping publicly-funded research directions.
#### Workshop Objectives:

- Analyze how public research funds are distributed among different organizations and project themes
- Investigate potential conflicts between corporate interests and stated EU sustainability goals
- Examine the lack of democratic input in research funding decision-making process
- Connect funding patterns to broader questions about future societal pathways.

This workshop aims to reveal the gaps in democratic oversight of research funding. Participants will investigate how public money shapes technological pathways and whether funding decisions align with sustainability principles. By connecting ADEME's 'pathways to carbon neutrality' framework to actual EU funding patterns, we ask: **whose futures are being funded, and who gets to decide?**

Moving beyond theoretical debates about democracy in research, this workshop give participants hands-on experience investigating actual funding flows. This makes the “who decides our technological future” question concrete and actionable. Focusing on public data detailing the distribution of public research money in the EU Research Framework Programs, each participant will be able to pick an organisation and analyze for themselves how much public money gets allocated to them and on what major projects the chosen company works on. This will allow participants to critically analyse how the research goals set by the European commission fund specific research themes and thus shape the direction in which our society goes.

#### How did we build it?
Sciences Citoyennes and Scientists Rebellion France developed a code that analyses public data of four Framework Programs (FP6, FP7, H2020, Horizon Europe). To make it easier to reach interesting results in the timeframe of a workshop we simplified the steps but are in the process of documenting exactly what we did so that anyone can restrace our steps and make their own edits. 

Firstly, with the help of the collective [EIES](https://eies.fr/) (Entreprise Illégitime Enseignement Supérieur) we developed a 'super list' of the top 60 companies that have the most connections to universities and research projects in France. To start we collected the Top 50 companies that EIES found has the most ties to universities. We also looked through the companies present in the ANR (French National Research Agency / Agence National de la Recherche) and cross checked to add the ones not present in the EIES list. Finally we also added to the list the private companies present in the French national thematic groups (GTN - Groupe Thématique Nationaux) who decide the research goals and direction for France. This results in a list with 64 French companies : [French Super List](https://github.com/sciences-citoyennes/Future-Earth-Workshop/blob/main/Super%20List%20pdf.pdf).

From there we filtered through the public CORDIS data of the four Framework Programs to extract all of the projects that these companies are a part of and put them in a sheet we called ['EU-fundings-TopFRcomp'](https://github.com/sciences-citoyennes/Future-Earth-Workshop/blob/main/EU-fundings-TopFRcomp.csv) in the GitHub but that we call 'Clean Data' for short. In other words, to make the analysis simple, we created an already filtered dataset containing the project information for only the companies on the Super List. This dataset contains the project abreviation, company name, project title, country, ecContribution, netEcContribution, total costs, start & end dates, and the European Science Vocabulary (EuroSciVoc) keywords. 

Many of these big companies have different branches so, to extract the projects for each company, we searched by keywords. For example, we used 'AIRBUS' and it caught all instances with that name including its other branches like 'AIRBUS OPERATIONS SAS' and 'AIRBUS ATLANTIC'. It is important to note that some companies have subsidiaries with completely different names so this code will miss those. EIES is currently developing a database with all of the affiliated names for each company but with limited time we chose to simply filter by keywords as it catches a significant portion already. 




#### How does it work?
We have many components to this workshop that we bring together at the top of this file in the RESOURCES section, including: 
- [Presentation slides](https://canva.link/78u6piohcxliilk) from Future Earth 2026 that gives background on the Framework Programs and how we can do research differently.
- Link to the [Doc](https://pad.liiib.re/pa27xhM9QrCHpGPwau5G5g?view) with all of the instructions and documentation
- [Binder Link](https://mybinder.org/v2/gh/sciences-citoyennes/Future-Earth-Workshop/HEAD) to run the code directly through a browser
- [ADEME Scenarios](https://www.ademe.fr/les-futurs-en-transition/les-scenarios/) to contextualize the research projects in our wider societal direction

Read through the doc for the workshop instructions, happy exploring ! 
