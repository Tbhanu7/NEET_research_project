# CLAUDE.md

@LESSONS.md

## Project
- Course research project on NEET (not in education, employment, or training) youth.
- Data: CPS ASEC (Annual Social and Economic Supplement) extracted from IPUMS CPS.
- Analysis: a Python notebook (`.ipynb`) run in Google Colab.

## Data rules
- Never commit raw IPUMS data files (`.dat`, `.csv`, `.gz`, `.xml`); IPUMS terms restrict redistribution.
- Keep data files out of git; list them in `.gitignore`.
- In Colab, load data from Google Drive or an upload, not from the repo.
- Use the IPUMS sample weight (`ASECWT`) for all population estimates.
- Check the IPUMS codebook before recoding any variable; note special codes (e.g. 99 = NIU, "not in universe").

## Code style
- Write simple code: short lines, plain pandas, no clever tricks.
- Put a short comment on every line of code, e.g. `df = pd.read_csv(path)  # load the data`.
- Use clear names (`age`, `weight`, `neet`), not abbreviations only the author knows.
- Prefer small steps over long chained expressions.
- One idea per notebook cell; add a short text cell above each section explaining it.

## Notebook rules
- The notebook must run top to bottom in a fresh Colab session.
- Install packages in the first cell with `!pip install`, only if Colab lacks them.
- Set paths and file names in one cell near the top.
- Clear huge outputs before saving the notebook.
- Do not hardcode personal Drive paths or credentials.

## Communication
- Explain every change in plain English: what changed and why, with no jargon.
- Say what you did not verify; never claim code ran if it did not.

## Lessons (LESSONS.md)
- When I correct you or state a preference, add a line to LESSONS.md: what happened and the rule for next time.
- When I paste an error from Colab, or you find a mistake in your code, fix it and add a line on the cause.
- Update an existing line instead of repeating it.
- Keep each line short.
- Commit LESSONS.md with your other changes.

## Git workflow
- Commit with a clear, descriptive message.
- Push the changes, then merge them into `main` directly.
- Do not open pull requests.
