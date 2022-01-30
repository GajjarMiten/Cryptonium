
# Cryptonium
A simple web app to display information about different cryptocurrency's pirce, news and market cap.
- This project created using React.JS and RapidAPI


## Run Locally

Clone the project

```bash
  git clone https://github.com/GajjarMiten/Cryptonium.git
```

Go to the project directory

```bash
  cd Cryptonium
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run dev
```


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`VITE_APP_RAPIDAPI_KEY`

`VITE_APP_CRYPTO_API_URL`

`VITE_APP_NEWS_API_URL`

`VITE_APP_NEWS_RAPIDAPI_HOST`

`VITE_APP_CRYPTO_RAPIDAPI_HOST`


## API Reference
In this I've use two APIs from RapidApi
- [Conin Ranking API](https://rapidapi.com/Coinranking/api/coinranking1/)
- [Bing News Search](https://rapidapi.com/microsoft-azure-org-microsoft-cognitive-services/api/bing-news-search1/)

#### Headers required*
```json
  x-rapidapi-host: CRYPTO_RAPIDAPI_HOST,
  x-rapidapi-key: RAPIDAPI_KEY,
```

#### Get all coins with limit

```http
  GET https://coinranking1.p.rapidapi.com/coins?limit=$limit
```

#### Get details of a coin

```http
  GET https://coinranking1.p.rapidapi.com/coin/${coidId}
```

#### Get history of coin

```http
  GET https://coinranking1.p.rapidapi.com/coin/${coinId}/history?timeperiod=${timeperiod}
```

#### Get Crypto News

```http
  GET https://bing-news-search1.p.rapidapi.com/news/search?q=${newsCategory}&safeSearch=Off&textFormat=Raw&freshness=Day&count=${count}
```


