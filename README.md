# Indexer Historical Data Download

This R Markdown script allows you to fetch and analyze historical data for indexers on the Arbitrum network using The Graph's API.

## Setup Instructions

1. Open the file `indexer_daily_data_download.Rmd` in RStudio or your preferred R environment
2. Locate the API key section at the beginning of the file:
   ```r
   # set api key:
   api_key = ''
   ```
3. Insert your API key from The Graph between the quotes. You can obtain an API key from [The Graph's website](https://thegraph.com/studio/apikeys/).

## Running the Script

1. Make sure you have all required R packages installed:
   - flexdashboard
   - shiny
   - readr
   - dplyr
   - DT
   - ghql
   - jsonlite
   - tidyverse
   - anytime
   - snakecase
   - shinycssloaders

2. Run the R Markdown script:
   - In RStudio: Click the "Run Document" button or press Ctrl+Shift+K (Cmd+Shift+K on Mac)
   - This will launch a Shiny dashboard where you can:
     - Enter an Ethereum wallet address
     - Specify the number of historical dates to fetch (up to 365 days)
     - Click "Fetch Data" to retrieve and display the indexer data

The script will fetch historical data including:
- Staking information
- Delegation metrics
- Indexing rewards
- Query fees
- And other relevant indexer metrics

The resulting data can be exported to various formats including CSV, Excel, and PDF.

Live version available at: https://predictcrypto.shinyapps.io/indexer_daily_data_download/
