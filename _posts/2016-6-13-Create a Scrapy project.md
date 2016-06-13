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
  
2. 

