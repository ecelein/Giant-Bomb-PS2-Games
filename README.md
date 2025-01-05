# Giant Bomb Wiki - PlayStation 2 Games List

This dataset contains a list of games which are listed under the category of the console "PlayStation 2", in the Wiki section of the website Giant Bomb, which is an American video game website and wiki that includes personality-driven gaming videos, commentary, news, and reviews.

Data was scraped from the following address, filtered to adjust the purpose: https://www.giantbomb.com/games/

## Format of the files in the corpus

There are three files that can be found:

- **Giant_Bomb_PS2_Games.ipynb** which includes the code that was used to scrape the website and some additional data exploration.
- **giantbomb_games.csv** which is the output, displaying the data that was scraped.
- **README.md** which is the markdown file, which contains information about this corpus.

Below are the data columns and their descriptions that can be found in the "giantbomb_games.csv" file.

| Column Name  | Description                      |
| ------------ | -------------------------------- |
| Title        | Title of the PlayStation 2 game. |
| Release Date | Release date of the game.        |
| Description  | A brief description of the game. |

### Terms of Use

Giant Bomb has their own official API, which they make clear it is a free resource, for non-commercial use only. They ask us to link back to them on every page used.

Terms of use can be found in the following link:
https://www.giantbomb.com/api/

**robots.txt** file consists of the following:

```# robots.txt for https://www.giantbomb.com/
User-agent: AhrefsBot
Disallow: /

User-agent: AwarioRssBot
User-agent: AwarioSmartBot
Disallow: /

User-agent: barkrowler
Disallow: /

User-agent: BLEXBot
Disallow: /

User-agent: CCBot
Disallow: /

User-agent: DataForSeoBot
Disallow: /

User-agent: dotbot
Disallow: /

User-agent: GPTBot
Disallow: /

User-agent: ImagesiftBot
Disallow: /

User-agent: MJ12bot
Disallow: /

User-agent: SemrushBot
Disallow: /

User-agent: TurnitinBot
Disallow: /

User-agent: *
Allow: /api/$
Disallow: /api/*
Disallow: /notifications/
Disallow: /search/
Disallow: *login=*
Disallow: /videos/embed
Disallow: /videos/feed/
Disallow: /podcast-xml/*premium*
Disallow: /wiki/moderation/
Disallow: /postRender
Disallow: /forums/*/flag/
Disallow: /forums/*/delete/
Disallow: /forums/*/edit/
Disallow: /forums/*/lock/
Disallow: /forums/*/anchor/
Disallow: /forums/*/add-to-favorite/
Disallow: /forums/*/best-answer/*/
Disallow: /jsonsearch/
Disallow: /chat/
```

### Data preparation steps taken

1. Initially used dropna() method on some columns of the dataframe in order to ensure a smooth analysis.
2. Removing punctuation.
3. Converting to lowercase.
4. Tokenizing words.
5. Removing the stopwords.
