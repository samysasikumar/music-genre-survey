# Music Genre Survey

A data science project by Samyuktha Sasikumar for the **Introductory Data Science Workshop** on Udemy. I surveyed Redmond High School students and others about how they listen to music, then cleaned and analyzed the responses using the five stages of data science.

## Question

What music do people listen to, how long do they listen each day, and how do they listen?

## The five stages

### 1. Ask a question
What genres do people like, how much do they listen per day, and do they use earphones or a speaker?

### 2. Collect raw data
A Google Form fed a Google Sheet (`Form Responses 1`). I collected **56 responses** between Oct 31 and early Nov 2026. The questions used in the analysis:

1. What is your #1 favorite music genre?
2. How many hours/minutes do you listen to music per day?
3. What is your most preferred way to listen to music?
4. What school do you go to? (Redmond High School or Other)

### 2b. Privacy
The Form also asked for a name. Names are not used in the analysis, and should be removed from any public copy of the data.

### 3. Clean and organize (`Clean Data` sheet)
Answers were typed as free text, so they needed cleaning:

- **Genres:** matched spelling and wording, such as "pop", "Pop" and "Pop music" counted as Pop, and "Bollywood" and "Bollywood Music" counted as Bollywood.
- **Listening time:** converted answers such as "1 hour", "1.5 hours", "90 minutes" and "30 min" to **minutes per day** with a formula.
- **Unclear answers:** 9 responses were left out of the cleaned data, mostly range answers such as "2-3 hours", "8-9 hours" and "6+ hours" that can't be turned into one number. That leaves **47 usable responses** (26 Redmond High School, 21 other).

### 4. Analyze and visualize
Counts and averages by genre, listening time and listening method, overall and by school group.

### 5. Results

| Finding | Result |
|---|---|
| Most popular genre | **Pop**, 7 of 47 (15%) |
| Next most popular | EDM and Metal, 5 each; then Latin, 4 |
| Variety | 15 different genres appeared |
| Average listening time | **87 minutes a day** (median 90) |
| Most common answer | 90 minutes (14 of 47) |
| Range | 20 to 300 minutes a day |
| Listening method | **Earphones/headphones 31 (66%)**, speaker/phone 16 (34%) |

**Redmond High School (26) vs other respondents (21)**

| | Redmond High School | Other |
|---|---|---|
| Average listening time | 94 min/day | 78 min/day |
| Earphones/headphones | 20 of 26 (77%) | 11 of 21 (52%) |
| Top genres | Pop, EDM, Hip Hop and Metal tied at 3 | Pop (4), then Latin and Rock (3 each) |

### Conclusion
Pop was the most common favorite genre, but tastes were spread across 15 genres. Most people listen for about an hour and a half a day, and about two thirds use earphones or headphones. Redmond High School respondents listened a bit longer on average and used earphones or headphones more often than other respondents.

## Limits
- Small sample of 47 usable responses, so differences of one or two people (such as between genres) are not meaningful.
- Respondents chose to answer, so they may not represent all students.
- Listening time is self-reported and typed as free text.
- The "Other" group mixes people from different schools and backgrounds.

## Files
| File | What it is |
|---|---|
| `Music_Survey_Data.xlsx` | Form responses and the cleaned data (`Clean Data` sheet with the minutes-per-day formula) |

## Tools
Google Forms, Google Sheets, Excel.

## Next steps
- Collect more responses and compare more schools.
- Ask about listening time with number choices instead of free text, to avoid range answers.
