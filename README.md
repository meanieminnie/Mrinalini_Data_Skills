# Data Skills

I'm a data-driven business and economics reporter based in Manhattan, New York, with 16 months of graduate school experience. Through this program, not only did I learn that data analysis is at the core of most investigative projects in today's world, but I developed the confidence to back my reporting with data. Suppose you, like me, have felt like your voice as a journalist could be encouraged by solid proof in the form of data, ranging from salaries for public servants to energy units required to run large language models. In that case, you only need to learn Python for journalists. 

I was a novice when I started my journey as a data reporter. I began by building websites using HTML and CSS. Starting from scratch, I delved into both front-end and back-end development, allowing me to experiment with dynamic website design. This is the story of how I built my coding skills in three different languages to analyze, chart, and contextualize data to support my journalism. 

## First semester

In the first semester, I learned how to clean, analyze, and merge datasets using Microsoft Excel Sheets. My favorite was VLOOKUP or XLOOKUP, a function that matches keys like area codes from two different datasets, providing key insights into the database. 

I also learned how to use Datawrapper, a free mapping and charting software that creates static and dynamic elements with custom datasets. What started with a simple line chart, would later help me explain complex stock comparison charts. 

Alongside all this, I set up my first GitHub account and uploaded all demos and published projects. What an exciting platform, almost like a social media platform for coders. I created a local repository, committed every change to the code, and files, and pushed it to the cloud origin. 
Link to GitHub. 
My first project, which was also a class assignment, was a story on immigrant communities facing language barriers in New York City. I learned how to write html and css code along with data wrapper charts and maps embedded in it. The full story is available here. 
Another crucial learning point: is how to organize files and folders to avoid confusion. If styles.css is not in the same folder as index.html, my website won’t show any style elements, no matter how much I try linking the two. 

## Second Semester: Introduction to Python, Pandas
*Clean, Analyse, Vizualize*
The second semester started on a completely different note. I was suddenly dealing with Jupyter Notebooks, anaconda, and github. Unbeknownst to me, these three would become my constant companions throughout the next year. 
I’d heard my software developer friends talk about Python with great anguish. At first encounter, Python looks a little intimidating. Like any new language, I had to start with the basics. 
1. What can Python do? It can run simple calculations like addition, subtraction, multiplication, and division. It imports different libraries - which are pre-packaged code environments - for specific applications. 
Every programmer has a preference for using Python. Some use the computer’s built-in terminal to access coding documents like Jupyter Notebooks. Others prefer installing launchpads like Anaconda to get there. I, like countless others, preferred Jupyter Notebooks through Anaconda. 
Think of Jupyter Notebooks as your Google Doc that can store and run desired code against your computer’s processor. 
2. I began my coding journey by understanding the difference between code and markup on Jupyter Notebooks. A code block is used to run functions and the markup block is used to write text. 
Because coding is often a lonesome and collaborative experience, Jupyter Notebook helps programmers strike the perfect balance between the two. When writing code alone, one can document their methodology using the markup #(text), for future reference for themselves and collaborators. 
Python can be used to create simple lists, and multiple lists within lists, which are called dataframes. It can clean data and then display it as a line chart. 
I  learned data analysis using the Pandas library. Pandas is the go-to data analyzer within the data journalism community. 
CLEAN
Within Pandas, one can import .csv, .xlsx, .pdf files from their laptop into jupyter notebooks to see the contents as a whole or call a specific set of values using the slice (n) feature. One could group information from a single column using the groupby function. 
.info() gives the complete information on a dataset, including type of data in each column. 
```
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 826 entries, 0 to 825
Data columns (total 15 columns):

#   Column                               Non-Null Count  Dtype  
---  ------                               --------------  -----  
0   SBA Physical Declaration Number      632 non-null    object 
1   SBA EIDL Declaration Number          824 non-null    float64
2   FEMA Disaster Number                 575 non-null    float64
3   SBA Disaster Number                  824 non-null    object 
4   Damaged Property City Name           824 non-null    object 
5   Damaged Property Zip Code            824 non-null    float64
dtypes: float64(10), object(5)
memory usage: 96.9+ KB
```
3. Sorting/filtering data sets using ‘sort’ and ‘query’ features. This feature is extremely helpful when combining columns with multiple values to create compact datasets   
```
data frame.sort_values(by="Value 1", ascending = True)
data frame.query('`column name` comparison_operator value')
```
**ANALYZE**
1. I learned to group specific columns to infer data, calculate mean, median and average. 
2. Nested lists: When multiple lists are placed within a big list, it can be difficult to extract them for calculations. Using ‘keys’ or .get() and ‘slice’ functions, I could now extract these nested lists. 
3. Data aggregation using .describe(), f strings, and reformatting them to desired decimal spaces. 
```
pd.options.display.float_format = '{:,.0f}'.format
```
Example of using all these functions on the dataset: Citi Bike Week 8 notebook. 
4. Using .merge to identify and collate two data sets with same keys, which is similar to VLOOKUP in excel. 
Looking up data in a large dataset using positional indexing - .iloc 
```
df.iloc[start_index:end_index]
Look up multiple rows and columns by labels using .loc
df.loc[[index_value1, index_value3, index_value4]]
```
**Visualization**
I learned that Python can not only clean and analyze data, but it could also create a line chart in Jupyter Notebooks for my understanding. 
Compare two values in Pandas: Insert notebook with oil vs gold project. 

**Final Project**

Analyzing complaints against online lender SoFi or Social Finance, Inc. from the Consumer Financial Protection Bureau (CFPB) 
- My goal with this project was to extract data from csv files, calculate the number of complaints, and find out how many customers felt like the company’s response to their complaints was satisfactory. 
- When I first saw the data, I could see the total number of complaints, the narrative, and a column titled ‘consumer disputed?’ that would give me my answer. 
- I used Pandas to filter out the complaints with consumer disputes marked N or NO. 
- Then I created a separate data frame with these entries to get a total count and turn it into a csv file for permanent storage. 
- This analysis would come in handy in writing personal finance stories in the coming year. 

## Third Semester: Python Investigations

I never thought I’d make it this far as a data journalist. I’d learned Pandas functions in the previous semester and tested my knowledge in the real world. I could use my skills to identify, clean, analyze and even visualize complex data sets. If I had a raw data set for complex investigations, I could methodically break it down into meaningful insights. 

But if someone told me I’d be learning things that seasoned programmers struggle with at times, I wouldn’t believe them. That I’d be running programs to extract information from websites, instead of spending hours copying it, I’d be relieved, to say the least. 

But why am I learning any of this? I want to simplify the process of gaining publicly available information, especially if it’s hidden from plain view. I want to distill this information and add important context for readers of all kinds. So, I began learning Python for complex investigations in journalism. 

List of tasks:
1. Scrape
I learned how to gather and scrape text and numbers across multiple document types (for example PDF, .txt) 
I even learned how to unzip document folders within Python, to access documents to be analyzed. 
2. Regular Expressions
I learned how to formulate and use regular expressions to search for patterns through large data sets. 
3. Natural Language Processing (NLP)
NLP helped me tokenize each word and categorize the data into larger buckets for further analysis. 
4. Artificial Intelligence
Using AI to generate code scripts to aid data analysis.
5. Python functions: I defined specific and universal functions in Python. Functions are reusable programs that store a set of complex instructions which aid our code. It saves time and effort. 
6. Gender Estimator: Python has a library called Genderize that calculates the gender probability of a proper noun. The only limitation is that it operates in the binary - male or female. 
7. Fuzzy Wuzzy: Cool word, cooler function! Fuzzywuzzy is a similarity algorithm that calculates the number of changes (additions, deletions, and moves) that are required to make one string identical to another. 
8. Advanced Scraping: I learned advanced scraping techniques during the second half of the semester, as a way to advance my investigative Python skills. 
These skills are invaluable when it comes to investigating publicly available data on government and agency websites. Tough as it sounds, thinking like an investigator is a lifelong skill, and the more you throw yourself into it, the better you get at it. 

Static URL:  When the website URL doesn’t change no matter which page you target, you try to scrape the contents, divide it into a list of dictionaries, and then slice that list to target the required information. A lot of this skill relies on Pandas operations learned in previous classes. 
Javascript scrape: This involves scraping the website using JSON.
API Scrape
Scrollers: In this, we learned how to scrape pages with endless scrolling. 



### Folders
1. Introduction to Jupyter Notebooks
2. Python Investigations
3. Advanced scraping

