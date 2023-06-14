### Why Scrap arXiv?
Researchers often need to review the latest scientific literature. Although this process can be done manually by running different requests in search engines like Google Scholar, it is recommended to follow a systematic procedure (even if it is not a systematic review paper) to obtain the most relevant evidence. To automate this process, we provide these two functions for scraping arXiv search results.

Hope it helps!

<br><br>

### Code description
This code consists of two functions for scraping and downloading papers from arXiv. The functions are as follows:

1. scrap_arxiv(url, output_filepath='output.xlsx'): This function takes a search strategy URL for arXiv and scrapes the search results. It retrieves the titles, authors, abstracts, and PDF links for each article and returns a pandas DataFrame with this information. The search results are also saved in an Excel file specified by output_filepath (default is 'output.xlsx'). The function is authored by Enrique Callejas Castro.

2. download_papers(links_list, path='papers'): This function takes a list of PDF links and downloads the corresponding papers. The downloaded files are saved in a folder specified by path (default is 'papers'). The function utilizes the requests library to download the files and tqdm for displaying a progress bar. The function is authored by Enrique Callejas Castro.
