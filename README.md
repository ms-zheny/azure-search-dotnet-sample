# C# Samples for Azure Cognitive Search

This repository contains C# code samples used in Azure Cognitive Search documentation. Unless noted otherwise, all samples run on the shared (free) pricing tier of an [Azure Cognitive Search service](https://learn.microsoft.com/azure/search/search-create-service-portal).

| Sample | Description |
|--------|-------------|
| check-storage-usage | Demonstrates checking storage usage of an Azure Cognitive Search service on a schedule. This sample may be modified to [adjust the service's capacity](https://docs.microsoft.com/azure/search/search-capacity-planning) or send an alert when the storage usage exceeds a predefined threshold. |
| create-mvc-app | This ASP.NET Core MVC sample demonstrates server-side search behaviors, such as filters and sorting. |
| data-lake-gen2-acl-indexing | This Azure Cognitive Search sample shows you how to configure an indexer connection to Azure Data Lake Gen2 that uses a managed identity and role assignments for selective data access. The sample loads data and sets up permissions for data access, and then runs the indexer to create and load a search index. |
| export-data | A console application that exports data from an Azure Cognitive Search service. |
| index-backup-restore | This .NET Core console app backs up an index (schema and documents) to your local computer and then uses the stored backup to recreate the index in a target search service that you specify. This sample can be helpful if you want to move an index into a different pricing tier.|
| multiple-data-sources | This .NET Core console app uses Azure Cognitive Search indexers and the .NET SDK to import data from Azure Cosmos DB and Azure Blob storage, combing data from two sources into one search index. | 
| multiple-search-services | This Azure Cognitive Search sample shows you how to issue a single query across multiple search services and combine the results into a single page. This sample uses [Good Books data](https://github.com/zygmuntz/goodbooks-10k). |
| optimize-data-indexing | This .NET Core console app builds off of the code used in the Quickstart and uses the Azure Cognitive Search .NET SDK to create an index, and efficiently load it with documents. The app allows users to test various batch sizes to understand the optimal batch size and then demonstrates how to efficiently upload 100,000 documents to a search index. This is done by splitting the data into batches, and spinning up several threads to upload the documents. Any failures are monitored and then retried using the exponential backoff retry strategy. The index is modeled on a subset of the Hotels dataset, reduced for readability and comprehension. Index definition and documents are included in the code. |
| quickstart | "Day One" introduction to the fundamental tasks of working with a search index: create, load, and query. This quickstart is a .NET Core console application. The index is modeled on a subset of the Hotels dataset, widely used in Cognitive Search samples, but reduced here for readability and comprehension. |
| search-website-functions-v4 | This sample builds a website to search through a catalog of books then deploys the website to an Azure Static Web App. The search experience includes a React app for the front-end. This app includes a search bar for free text queries, suggestions for type-ahead queries, and document lookup. |
| tutorial-ai-enrichment | This .NET Core console app creates an AI enrichment pipeline consisting of an index, indexer, data source, and skillset. The skillset calls Azure Cognitive Services image analysis and OCR, and natural language processing, extract information and structure from heterogeneous blob content, making it searchable in Azure Cognitive Search. |