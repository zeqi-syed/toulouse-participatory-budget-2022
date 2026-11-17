# Toulouse Participatory Budget: What Did Citizens Vote For?

An analysis of Toulouse's 2022 participatory budget vote: 199 citizen projects and 4,532 voters.

## The questions
1. Which kinds of projects get the most votes?
2. How do people use their votes?
3. Does a project's cost affect how many votes it gets?
4. If the budget were spent in vote order, would the city centre take an unfair share?
5. Which districts support ecological projects most?
6. Who votes for waste and recycling projects: locals or people from other districts?

## Key findings
- **Greening wins:** "Nature en ville" projects (trees, parks, plants) get 51% of all votes, followed by eco-mobility at 22%.
- **People use their votes fully:** 75% of voters used all three of their votes. Most spread them across different categories.
- **Bigger projects get more votes:** projects costing 150k-200k EUR average 103 votes, compared with 41-49 for projects under 100k EUR.
- **But small projects give the best value:** mosquito-control projects costing 1,200-7,500 EUR got up to 258 votes, by far the most votes per euro.
- **No city-centre bias:** funding projects in vote order up to 8M EUR gives the centre (District 1) about 7% of the money, close to an equal share.
- **Waste projects have local support:** about two thirds of their voters also backed another project in the same district.

## Method
Python (pandas, matplotlib, seaborn). I split each ballot into individual votes and joined them to project details (category, cost, district). That made it possible to analyse voter behaviour, not only project totals.

## Files
- `analysis.ipynb`: the analysis, with charts and findings
- `data/projects.csv`: one row per project
- `data/voters.csv`: one row per anonymous voter, listing the projects they voted for

## Run it
```bash
pip install -r requirements.txt
jupyter notebook analysis.ipynb
```

## Data
Toulouse 2022 participatory budget, from [Pabulib](https://pabulib.org), an open library of participatory budgeting data (one file per district, merged here into one projects file and one voters file).

Faliszewski, P. et al. (2023). *Participatory Budgeting: Data, Tools and Analysis.* IJCAI 2023.
