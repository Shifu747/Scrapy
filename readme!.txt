1. starting a virtual environment. * virtualenv venv 
2. activating it. * venv/scripts/activate.ps1
3. create scrapy project. * scrapy startproject projectname
4. start scrapy shell. *scrapy shell 'url'
5. check 200 response before  In[1]: 
6. use response.css('tag').get() or .getall() for information
7. use response.css('tag::text').get() or .getall() for text inside the tag
8. .getll() returns a list
9. get whole box using a variable. *products = response.css('div.details-pricing')
10. use that variable to crawl. *products.css('h4').get()
11. products.css('tag.class::text').get()
12. exit shell
13. scrapy genspider dronespider https://www.jessops.com/drones
13.1. scrapy genspider name url
14. inside dronespider.py write code according to shell commands
15. yield dictionary or other data 
16. go to terminal : scrapy crawl dronespider
16.1. scrapy crawl genspider_name
16.2. scrapy crawl genspider_name -o name.csv