# Netflix: One Page, One Finding — Data Analysis Notebook

**Research question:** *What kind of company is Netflix now, and when did it change?*  
**Dataset:** [Netflix Movies and TV Shows — Kaggle (shivamb)](https://www.kaggle.com/datasets/shivamb/netflix-shows)

> **Scope of the evidence.** This dataset is a historical catalogue snapshot with additions dated through **25 September 2021**. Here, “now” can only mean **the most recent period observable in this dataset**, not Netflix in 2026. We investigate *catalogue entries and their metadata*, not viewing behavior, production spending, or Netflix's complete business strategy.

**Workflow:** 1. Load and profile → 2. State three hypotheses → 3. Clean with justification → 4. Explore → 5. Test each hypothesis → 6. Investigate three data problems → 7. Conclusion and limitations.

**By:** Isela Zhuga, Nigel Xherimeja, Sara Petro

## Conclusion and limitations

### The answer

In this snapshot, Netflix in 2019–2020 was still a movie-dominated catalogue (69.6% of all titles), but the balance of what it *added* had shifted. The TV share of additions climbed from 26.8% to 30.5% and kept climbing in 2021 (33.7%); the post-2018 additions tilted back toward US-linked productions (non-US-only share fell from 60.0% to 53.6%); and the fastest-growing categories were mainstream comedies and family films while the international-movie and documentary licensing wave receded. **The turning point sits between 2018 and 2019**: additions peaked in 2019 (2,016 titles), and every mix shift we measured changes direction around that year.

So, in one sentence: ***“Around 2018–2019 Netflix's catalogue additions peaked and pivoted — away from licensed international movies, toward TV shows and mainstream, largely US-linked, comedy and family content.”***

### Limitations — what would change this answer

- **We see additions, not the catalogue.** The file records when titles were *added*, not when they left. We cannot reconstruct what subscribers actually saw in any given year — a title added in 2017 may have been gone by 2019. If removals were concentrated among international titles, our “less international after 2018” finding would be understated, or wrong.
- **“Now” stops on 25 September 2021.** The dataset ends there, so nothing here speaks to the ad-tier, password-sharing, or games era. Our answer describes Netflix at the start of the decade, not Netflix today — and 2021 itself is a partial year, which is why no full-year comparison uses it.
- **Country and genre labels are imperfect.** Country is missing for 450 of the 6,732 comparison rows, and `listed_in` mixes geography with genre, so H2 and H3 partly measure Netflix's *labelling* habits, not just production reality.
- **We cannot identify Netflix Originals.** Release year equalling added year is only a rough proxy for first-run content, so we cannot cleanly separate commissioned originals from licensed catalogue — the distinction that most defines what kind of company Netflix is.
- **No viewing, revenue, or spending data.** What Netflix adds and what people actually watch can be very different things; this dataset cannot see the difference. Viewing-hours data, removal dates, and post-2021 additions are the three things most likely to change our answer.

*What this data could not tell you (poster line): what subscribers actually watched, what was removed from the catalogue, and anything after September 2021.*
