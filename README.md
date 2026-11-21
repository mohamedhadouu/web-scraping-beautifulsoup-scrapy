# Web Scraping with BeautifulSoup and Scrapy

Two presentations (in French) on web data extraction in Python, each with a practical example.

| File | Content |
|---|---|
| `wez-scraping-BeautifulSoup.pdf` | Scraping the **list of the most-followed Twitter accounts** from Wikipedia with **requests + BeautifulSoup**, then building an interactive **Power BI** dashboard from the extracted data |
| `wez-scraping-scrapy.pdf` | **Scrapy** architecture (engine, scheduler, downloader, spiders, middlewares, pipelines) and a practical project that extracts **product information from an Amazon page** and exports it to CSV |

## Scrapy example: main commands

```bash
pip install scrapy
scrapy startproject amazon
scrapy crawl article -o article.csv
```

The project defines the data fields in `items.py`, the extraction logic in a spider, and exports the results to a CSV file.

## BeautifulSoup vs. Scrapy at a glance

| | BeautifulSoup | Scrapy |
|---|---|---|
| Best for | Small scripts, a few pages | Large crawls, many pages |
| Learning curve | Easy | Medium |
| Speed | Sequential by default | Asynchronous (built on Twisted) |
| Built-in export | No | Yes (JSON, CSV) |

## Tech stack

Python · requests · BeautifulSoup · Scrapy · Power BI

## Next steps

- Add the Python source code of both scrapers to this repository
- Add a sample of the extracted data (CSV)

## Author

**Mohamed Hadou** · [LinkedIn](https://www.linkedin.com/in/mohamed-hadou/) · [GitHub](https://github.com/mohamedhadouu)
