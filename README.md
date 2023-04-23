# Website Scraper Project (Manel Saddouki) 

## I. Explanation of the main concepts of the Web Scraper: main components, functional flow... 
 							
web-scraping is a tool used to scrape a webpage and extract the necessary data that one needs. This tool can be used in different fields for different purposes. It is mainly used for business goals: extract necessary data, analyze it to get fruitful insights and use them to make future decisions. 

This tool can be used for example for marketing purposes such as customer reviews analysis or competitors’ customers' analysis, and for financial and investment goals like crypto or stock prices analysis. 

As a business analysis student, and from my previous internships, I can confirm how important such a technique can be for us. Collecting data is one of the most fundamental and time-consuming tasks in our field. That’s why working on this project can indeed boost my skills for my future professional positions. 

The Web Scraping technique is based on certain basic steps. We may note first that we need to choose our target website(s) and then decide on the parts that we need to extract. Next, we have to use a web spider and parser programs that can visit the website and collect the data. When we reach this step, we can manipulate these data to get insights, visualize them and save them in a file (CSV/excel..). 

So, the main needed components are:  the web spider or web crawler which is used in order to access and navigate a website (this program can go through all the links included in this website. It starts with the seed URL and then finish with all the others that are connected with it). Second, we need an HTML parser that allows us to study the HTML code of the website. This program can identify all the components (head, body, div, table..), organize them in a hierarchy tree structure (Document Object Model DOM), and then based on the user’s request, identify the needed part. Next, we need to extract it, but the tool used here depends on the type of data. It can be for example text, table, or graph extraction. Lastly, a data visualization tool (Matplotlib..) or simply a data-saving program should be used. 	 	 						
This technique can be very useful as it gives access to a large amount of data in a short period of time. However, I believe that we have always to be careful concerning copyrights. Collecting data is not allowed if you don’t respect its writer/source. 	



## II. An overview of the main existing solutions. 
During this project, I will be using **Python**, which is a coding language that has a lot of libraries that help with web scraping.  Here I provide some examples: : 

\- **Requests:** It’s a tool that I can use in order to make HTTP requests, such as Get request which will allow me to get the website content

\- **BeautifulSoup:** It is a library that can be used to parse the web page, and identify its elements. It can work with HTML or XML

\- **Scrapy:** it’s also a library that’s used for web crawling. It can be more powerful than BeautifulSoup if we need a large amount of data (from numerous web pages). Also, it’s able to handle cookies and sessions. 

\- **Selenium:** It is also another existing solution for scraping. It is useful if we need to interact automatically with a web browser.
lxml: A very fast library used also for HTML or XML parsing

\- **html5lib:** it’s a tool that can accurately parse a website, and works even with malformatted HTML 

\- **Advertools:**  can be used for analyzing and extracting data for marketing purposes (data can be for example from facebook/Twitter/Google ads)

Those are the main solutions that I can use while coding with Python. It’s important to note here that there are other options that users with no IT background can use such as the services Webose.io or Parsehub, and browser extensions like Scraper or Data Miner. 

### Advantages & limits: 

The existing solutions mentioned above have a lot of **advantages** that we can mention. 

These tools are time effective as it allows us to collect a large amount of data in a short period of time. Being able to implement such a technique can help you save time for your research phase. Also, it makes you gain a competitive advantage as today’s world is indeed about data, the more you collect, the more powerful you are.

Web scraping programs or services are also not that hard to use and generally user-friendly, one can always choose the method/tool that matches his skills. They can be adapted to one’s needs and freely scaled. 

Despite all that, web scrapers has also some **limitations**. For example, browser services and extensions have standard forms which cannot meet specific users’ needs. On the other hand, coding languages cannot differentiate between relevant and non-relevant data, it’s the users’ task to pay attention to the quality of the data to be extracted. Users need also to put extra effort into highly dynamic websites which can sometimes lead to un-updated or inaccurate data extraction.

Last but not least, it’s important to mention the problem related to websites that do not guarantee permission for web scraping. The concern of copyrights should always be taken into consideration. That’s why one has to get the website’s permission or work only with public data.
		 	 	 		
## III. A Design for the proposed solution:

### Problematic: 
In the past few years, Tunisia has been suffering from a hard economic situation. During my previous internships, and in my finance and micro-economic classes, I had the opportunity to discuss how crucial this issue is. Thus, I will take advantage of this project in order to go further with this topic.

### Project Goal: 

During my project, I will be developing a Python code that permits us to extract economic indexes from reliable sources, and visualize and analyze them. Those indexes can help me understand better our economy and get insights about today’s situation. 

### Exchanged messages/data:		

   1. The **inputs** for my project will be from reliable sources such as the INS website (Institut Nationale de Statistique), and CBT (Central Bank of    Tunisia)... 

   2. I will use their URL(s) in order to send requests to access their contents. 

   3. The data I will extract will be GDP (Gross Domestic Product), Unemployment rate, and Private sector enterprises... They will be saved in a pandas dataframe/files 

   4. These data will be then manipulated to get fruitful **outputs**: graphs visualization, and economic analysis. 


### Design and components: 

\-The first step is **websites identification**: 

     * BCT Central Bank of Tunisia) website for PIB 
     
     * INS (Institut Nationale de Statistique) website: Private sector enterprises, and for the unemployment rate 

   Those are examples of the websites that contain the data I will need to extract 

\-The second step is **website crawling**: I will send a request to access the contents of the web pages

\-The Third step is the **HTML parser** that will give me the structure of the websites (based on the HTML codes’ elements) 

\-The fourth step is **data extraction**: for the tables for example I will go use a function to go through all existing tables, identify  the necessary columns/rows, and then get all the data I need 

\-The fifth step is **data manipulation**: I will manipulate the collected data and convert them into a useful version (for example use iloc() to get the part I need or reset_index() to manipulate my tables’ indexes)

\-The sixth and last version is **data visualization**: I will plot graphs that will help me with the economic analysis (the graphs will be line/bars/Pie chart..)


This project is based on a combination of inputs (various data from various sources), and my analysis will be based on those inputs. For each step during the development phases, I will be using specific Python libraries. 
						
## IV. The tools and the development phases. 
 							
		
### The tools:

\-Coding Language: **Python**

\-Web Crawler Library: **Requests** 

\-Web Parser Library: **BeautifulSoup**

\-Data Manipulation & Analysis: **Pandas** 

\-Data Visualization: **Matplotlib** 

I did choose to work with these tools as I am used to working with some of them and they can easily be implemented. For web crawler and parser libraries, I chose the ones mentioned above as they serve my project goal. I cannot work with Advertools for example since it works on different topics. 

### The development phases: 

\-**Idealization and planning**: All the parts mentioned above summarize this phase. During this period, I selected the project I will work on, the topic I will analyze, the tools I will use, and the functional flow I will go through.

\-**Web scraping code development**: During this phase, I develop Python code that uses libraries to read the websites’ content, and extract data. The data will be saved for example in the pandas dataframe for future use

\-**Data visualizing code development**: My second part of the code will be to develop plot graphs that can help me in my analysis. These plots are line/ bars/ pie charts.. For instance, PIB and Unemployment indexes will be visualized in a way we can get the necessary insights. 

\-**Data Analysis**: During this part, a clear analysis will be done based on the data and graphs we presented. This step will permit us to present an economic report about our country. 

This code can be used for academic researchers who work on socio-economic-related topics. It also serves non-government organizations such as OECD for policy recommendations. 

## V. Executable version of the solution: 

The first version of my code solution is attached to this repository! 

		
 							
				
