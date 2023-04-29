# Website Scraper Project (Manel Saddouki) 

## I. Explanation of the main concepts of the Web Scraper: main components, functional flow... 
 							
web-scraping is a tool used to scrape a webpage and extract the necessary data that one needs. This tool can be used in different fields for different purposes. It is mainly used for business goals: extract necessary data, analyze it to get fruitful insights and use them to make future decisions. 

This tool can be used for example for marketing purposes such as customer reviews analysis or competitors’ customers' analysis, and for financial and investment goals like crypto or stock prices analysis. 

As a business analysis student, and from my previous internships, I can confirm how important such a technique can be for us. Collecting data is one of the most fundamental and time-consuming tasks in our field. That’s why working on this project can indeed boost my skills for my future professional positions. 

The Web Scraping technique is based on certain basic steps. We may note first that we need to choose our target website(s) and then decide on the parts that we need to extract. Next, we have to use a web spider and parser programs that can visit the website and collect the data. When we reach this step, we can manipulate these data to get insights, visualize them and save them in a file (CSV/excel..). 

So, the main needed components are:  the web spider or web crawler which is used in order to access and navigate a website (this program can go through all the links included in this website. It starts with the seed URL and then finish with all the others that are connected with it). Second, we need an HTML parser that allows us to study the HTML code of the website. This program can identify all the components (head, body, div, table..), organize them in a hierarchy tree structure (Document Object Model DOM), and then based on the user’s request, identify the needed part. Next, we need to extract it, but the tool used here depends on the type of data. It can be for example text, table, or graph extraction. Lastly, a data visualization tool (Matplotlib..) or simply a data-saving program should be used. 	 	 						
This technique can be very useful as it gives access to a large amount of data in a short period of time. However, I believe that we have always to be careful concerning copyrights. Collecting data is not allowed if you don’t respect its writer/source. 	



## II. An overview of the main existing solutions. 
Companies have the option whether to build there own scraper using web scraping libraries or to use the existing Off-the-shelf solutions that can be divided into three main categories: low-to-no code web scrapers/ Could web scrapers/ Browsers extensions web scrapers. 

### 1. Web scraping libraries: 
web crawlers are a type of software that automatically targets online websites and pulls their data in a machine-readable format. 
Those are examples of top open-source web crawler tools (different coding languages): 
* Java: Apache Nutch, Jspider, Heritrix 
* Javascript: Node Crawler, Porita
* Python: Scrapy, Pyspider

 let’s focus for example on Python, and the characteristics of its libraries. Here I provide some examples: 
* ***Scrapy:*** it’s also a library that’s used for web crawling. It can be more powerful than BeautifulSoup if we need a large amount of data (from numerous web pages). Also, it’s able to handle cookies and sessions. 
* **Requests:*** It’s a tool that I can use in order to make HTTP requests, such as Get request which will allow me to get the website content 
* ***BeautifulSoup:***  It is a library that can be used to parse the web page, and identify its elements. It can work with HTML or XML
* ***Selenium:*** It is also another existing solution for scraping. It is useful if we need to interact automatically with a web browser.
* ***LXML:*** A very fast library used also for HTML or XML parsing
* ***html5lib:*** it’s a tool that can accurately parse a website, and works even with malformatted HTML 
* ***Advertools:***  can be used for analyzing and extracting data for marketing purposes (data can be for example from Facebook/Twitter/Google ads)	

***Advantages & limits:***
The main advantages of web scraping libraries is that it allows you to customize scrapers based on your particular needs. Also it can be cheaper than pre-build tools.

The limits that they may have is that they require their users to have some advanced IT skills (etc knowledge of HTML structures, elements, and the use of libraries such as Python). Plus, it’s more time consuming and require more effort.

### 2. Off-the-shelf web scrapers:
* ***Low-to-no code web scrapers:*** we can note as an example ScrapingBee and doccparser => they can enable users to extract data from websites without writing any code. 
* ***Could web scrapers:*** like Zyte, Scraperapi, and AcrapingANT
* ***Browsers extensions web scrapers:*** such an example there are Parsers and Data Miner

***Advantages & limits:***
Those pre-build tools have multiple advantages as they don’t require IT skills and they user-freindly. Also, the code can be automatically updated to make sure that the data is constantly extracted. 
Yet, they still have some limits. We can mention that those tools are generally more expensive. Also they are less flexible as the provide standard format. 

=> All those options can be used by companies for different department and different applications, we can mention: 
Security: it can be for vulnerability scanning (scan the ones present in a certain website) or to gather information about potential threats (collect IP addresses/ online profiles etc of cybercriminals..)
Data analytics & Data science: like training predictive models (collect large volume of data to train models)
Marketing and sales: extract competitors’ prices and customers behavior to improve their performance.
Finance & Banking: collect data about a certain business to calculate its credit risk score 
		 	 	 		
## III. A Design for the proposed solution:

### Problematic: 
In the past few years, Tunisia has been suffering from a hard economic situation. During my previous internships, and in my finance and micro-economic classes, I had the opportunity to discuss how crucial this issue is. Thus, I will take advantage of this project in order to go further with this topic.

### Project Goal: 

During my project, I will be developing a Python code that permits us to extract economic indexes from reliable sources, and visualize and analyze them. Those indexes can help me understand better our economy and get insights about today’s situation. 

### Exchanged messages/data:		

   1. The **inputs** for my project will be from reliable sources such as the INS website (Institut Nationale de Statistique), and CBT (Central Bank of    Tunisia), and Donnees Mondiales

   2. I will use their URL(s) in order to send requests to access their contents. 

   3. The data I will extract will be for instance GDP (Gross Domestic Product), inflation rate, Unemployment rate, and Private sector enterprises. The data will be in different forms: tables/images... Then They will be saved in a pandas dataframe/files 

   4. These data will be then manipulated to get fruitful **outputs**: graphs visualization, and economic analysis. 


### Design and components: 

 1. The first step is **websites identification**: 

     * BCT (Central Bank of Tunisia) website for PIB 
     
     * INS (Institut Nationale de Statistique) website for : Private sector enterprises, and the unemployment rate 
     
     * Donnees Mondiales & Zewya websites for Inflation rate 

   Those are examples of the websites that contain the data I will need to extract 

 2. The second step is **website crawling**: I will send a request to access the contents of the web pages

 3. The Third step is the **HTML parser** that will give me the structure of the websites (based on the HTML codes’ elements) 

 4. The fourth step is **data extraction**: for the tables for example I will go use a function to go through all existing tables, identify  the necessary columns/rows, and then get all the data I need 

 5. The fifth step is **data manipulation**: I will manipulate the collected data and convert them into a useful version (for example use iloc() to get the part I need or reset_index() to manipulate my tables’ indexes)

 6. The sixth and last version is **data visualization**: I will plot graphs that will help me with the economic analysis (the graphs will be line/bars/Pie chart..)


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

 1. **Idealization and planning**: All the parts mentioned above summarize this phase. During this period, I selected the project I will work on, the topic I will analyze, the tools I will use, and the functional flow I will go through. The extraction will include data from tables/images...

 2. **Web scraping code development**: During this phase, I develop Python code that uses libraries to read the websites’ content, and extract data. The data will be saved for example in the pandas dataframe for future use. The extraction will include data from tables/images/texts... 

 3. **Data visualizing code development**: My second part of the code will be to develop plot graphs that can help me in my analysis. These plots are line/ bars/ pie charts.. For instance, PIB and Unemployment indexes will be visualized in a way we can get the necessary insights. 

 4. **Data Analysis**: During this part, a clear analysis will be done based on the data and graphs we presented. This step will permit us to present an economic report about our country. 

This code can be used for academic researchers who work on socio-economic-related topics. It also serves non-government organizations such as OECD for policy recommendations. 

## V. Executable version of the solution: 

The first versions of my code solution are attached to this repository! 

		
 							
				
