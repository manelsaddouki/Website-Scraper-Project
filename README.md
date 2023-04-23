# Website Scraper Project (Manel Saddouki) 

## I. Explanation of the main concepts of the Web Scraper: main components, functional flow... 
 							
web-scraping is a tool used to scrape a webpage and extract the necessary data that one needs. This tool can be used in different fields for different purposes. It is mainly used for business goals: extract necessary data, analyze it to get fruitful insights and use them to make future decisions. 

This tool can be used for example for marketing purposes such as customer reviews analysis or competitors’ customers' analysis, and for financial and investment goals like crypto or stock prices analysis. 

As a business analysis student, and from my previous internships, I can confirm how important such a technique can be for us. Collecting data is one of the most fundamental and time-consuming tasks in our field. That’s why working on this project can indeed boost my skills for my future professional positions. 

The Web Scraping technique is based on certain basic steps. We may note first that we need to choose our target website(s) and then decide on the parts that we need to extract. Next, we have to use a web spider and parser programs that can visit the website and collect the data. When we reach this step, we can manipulate these data to get insights, visualize them and save them in a file (CSV/excel..). 

So, the main needed components are:  the web spider or web crawler which is used in order to access and navigate a website (this program can go through all the links included in this website. It starts with the seed URL and then finish with all the others that are connected with it). Second, we need an HTML parser that allows us to study the HTML code of the website. This program can identify all the components (head, body, div, table..), organize them in a hierarchy tree structure (Document Object Model DOM), and then based on the user’s request, identify the needed part. Next, we need to extract it, but the tool used here depends on the type of data. It can be for example text, table, or graph extraction. Lastly, a data visualization tool (Matplotlib..) or simply a data-saving program should be used. 	 	 						
This technique can be very useful as it gives access to a large amount of data in a short period of time. However, I believe that we have always to be careful concerning copyrights. Collecting data is not allowed if you don’t respect its writer/source. 	

			

## II. An overview of the main existing solutions. 
During this project, I will be using Python, which is a coding language that has a lot of libraries that help with web scraping.  We can note: 

\- **Requests:** It’s a tool that I can use in order to make HTTP requests, such as Get request which will allow me to get the website content

\- **BeautifulSoup:** It is a library that can be used to parse the web page, and identify its elements. It can work with HTML or XML

\- **Scrapy:** it’s also a library that’s used for web crawling. It can be more powerful than BeautifulSoup if we need a large amount of data (from numerous web pages). Also, it’s able to handle cookies and sessions. 

\- **Selenium:** It is also another existing solution for scraping. It is useful if we need to interact automatically with a web browser.
lxml: A very fast library used also for HTML or XML parsing

\- **html5lib:** it’s a tool that can accurately parse a website, and works even with malformatted HTML 

\- **Advertools:**  can be used for analyzing and extracting data for marketing purposes (data can be for example from facebook/Twitter/Google ads)
		 	 	 		
## III. A High-Level Design for the proposed solution: 
In the past few years, Tunisia has been suffering from a hard economic situation. During my previous internships, and in my finance and micro-economic classes, I had the opportunity to discuss how crucial this issue is. Thus, I will take advantage of this project in order to go further with this topic. 
During my project, I will be developing a Python code that permits us to extract economic indexes from reliable sources, and visualize and analyze them. Those indexes can help me understand better our economy and get insights about today’s situation. 

### Exchanged messages/data:		

The inputs for my project will be from reliable sources such as the INS website (Institut Nationale de Statistique), and CBT (Central Bank of Tunisia)... 

I will use their URL(s) in order to send requests to access their contents. 

The data I will extract will be GDP (Gross Domestic Product), Unemployment rate, and Private sector enterprises... 

These data will be then manipulated to get fruitful outputs: graphs visualization, and economic analysis. 


### Design and components: 

\-The first step is websites identification: 

     * BCT website for PIB 
     
     * INS website: Private sector enterprises, and for the unemployment rate 

=> Those are examples of the websites that contain the data I will need to extract 

\-The second step is website crawling: I will send a request to access the contents of the web pages

\-The Third step is the HTML parser that will give me the structure of the websites (based on the HTML codes’ elements) 

\-The fourth step is data extraction: for the tables for example I will go use a function to go through all existing tables, identify  the necessary columns/rows, and then get all the data I need 

\-The fifth step is data manipulation: I will manipulate the collected data and convert them into a useful version (for example use iloc() to get the part I need or resr_index() to manipulate my tables’ indexes)

\-The sixth and last version is data visualization: I will plot graphs that will help me with the economic analysis (the graphs will be line/bars/Pie chart..)
				
						
## IV. The tools and the development phases. 
 							
		
### The tools:

\-Coding Language: **Python**

\-Web Crawler Library: **Requests** 

\-Web Parser Library: **BeautifulSoup**

\-Data Manipulation & Analysis: **Pandas** 

\-Data Visualization: **Matplotlib** 
		

### The development phases: 

\-Idealization and planning

\-Web scraping code development 

\-Data visualizing code development 

\-Analysis 



		
 							
				
