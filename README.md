
![App Screenshot](https://putusan3.mahkamahagung.go.id/public/frontend/images/logo.png)
# Kendari Decision Directory / Data Scraper

## Introduction
This dataset consists of Indonesian court decision documents for Kendari region criminal cases that have been annotated for the document sections. There are 134 documents in the dataset folder. The documents are available in xml format. The contents of the xml file are clean text extracted from the PDF files of court decision documents that are publicly available on the website of the [Indonesian Supreme Court Decision]

Data scraping from a website like https://putusan3.mahkamahagung.go.id/ involves the automated process of extracting information from the web pages of the site. This process typically includes several key steps:

## 1. Sending HTTP Requests
To initiate scraping, the script sends an HTTP request to the target website. In this case, the request is sent to https://putusan3.mahkamahagung.go.id/. The goal is to download the content of the web page.

## 2. Parsing HTML
After receiving a response from the server, the script then parses the HTML code of the web page. This parsing is done to extract relevant information. HTML parsers like BeautifulSoup (in Python) are often used for this task.

## 3. Extracting Data
Once the HTML is parsed, the script identifies specific elements within the HTML structure to extract the desired data. This may include the text of court decisions, dates of rulings, case numbers, and other relevant information. This process often involves searching for HTML elements with specific tags, classes, or IDs.

## 4. Handling Pagination
Many websites have data spread across multiple pages (pagination). The script may need to repeat the request and parsing process for each additional page to collect comprehensive data.

## 5. Saving Data
he extracted data is then stored in a useful format, such as CSV, a database, or JSON. The storage format depends on the subsequent use of the data.

## Instalation Requirement
```bash
  pip install pandas requests BeautifulSoup4 pdfminer.six lxml
```
```bash
  pip install pdfminer.six
```
## Feature Description
there are some sections were annotated from each court decision page:       "judul","nomor", "tingkat_proses", "klasifikasi","kata_kunci", "tahun", "tanggal_register", "lembaga_peradilan", "jenis_lembaga_peradilan","hakim_ketua","hakim_anggota","panitera","amar","amar_lainnya", "catatan_amar", "tanggal_musyawarah","tanggal_dibacakan","kaidah", "abstrak", "link","link_pdf","file_name_pdf","text_pdf",
