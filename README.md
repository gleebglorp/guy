### Wiki Guy is built from scratch to support <a href="https://conecorp.cc">CONECORP</a> wikis.
![](https://static.wikitide.net/stackdwiki/2/26/834_1x_shots_so.png)
<br>
<p align="center">
  <a href="https://discord.com/oauth2/authorize?client_id=1472272697798037524">Add to server</a>
<br>ദ്ദി◝ ⩊ ◜.ᐟ
</p>

## Setup
Please note that `server.js` exists on the repository so that Instatus is able to get active status of the bot. It can be removed.

1. **Clone the repository**
   ```bash
   git clone https://github.com/conecorp/wikiguy.git
   cd wikiguy
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment variables**
   - Copy `.env.example` to `.env`:
     ```bash
     cp .env.example .env
     ```
   - Open `.env` and replace `your_discord_token_here` with your actual Discord Bot Token.

4. **Run the bot**
   ```bash
   npm start
   ```

## Configuration

You can customize the bot's behavior by editing `config.js`. This file includes:
- **WIKIS**: Define the wikis the bot supports, including their API endpoints and article paths.
- **CATEGORY_WIKI_MAP**: Map Discord category IDs to specific wikis for context-aware embedding.
- **STATUS_OPTIONS**: Customize the bot's rotating status messages.
- **STATUS_INTERVAL_MS**: Change how often the status updates.
