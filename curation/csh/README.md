`List of meds CSH.xlsx` is the unmodified curation returned by Christine Hessler.

We used [Trifacta Wrangler](https://www.trifacta.com/products/wrangler/) to:

+ import the unmodified excel file
+ clean the `classification` column so all values are in {`DM`, `SYM`, `NOT`}
+ export to CSV (`curation-CSH.csv`)

The Wrangler script (`curation-CSH.wrangle`) details the specific operations performed. Since Wrangler is a proprietary application, we used it only for a task that may otherwise have been performed manually. Comparing the input (`List of meds CSH.xlsx`) to output (`curation-CSH.csv`) is sufficient to evaluate the changes made using Wrangler.
