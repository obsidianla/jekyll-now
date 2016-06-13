1. create a project
  $ scrapy startproject my_crawler
  You will see the structure of a project like this:

  my_crawler
  |- my_crawler
  |    |- __init__.py
  |    |- items.py      (define the schema of data to be crawlered)
  |    |- pipelines.py  (The following manipulation after crawling)
  |    |- setting.py    (define all kinds of configuration)
  |    |- spiders       (Define the logic of crawling. You can define several spiders in one project)
  |    |    |- __init__.py
  |    |    |- crawl_spider.py
  |- scrapy.cfg
  
2. define the schema  
    Change items.py like this:
    
  import scrapy
  
  class MyCrawlerItem(scrapy.Item):
      # define the fields for your item here like:
      name = scrapy.Field()
      title = scrapy.Field()  # title
      url = scrapy.Field()    #url
      summary = scrapy.Field()# abstract
      pass
3. Write the code of analyzing the webpage
  Under my_crawler/spiders, create a file named craw_spider.py



