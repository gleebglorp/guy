<div align="center">
	<h1>CONECORP's Wiki Guy</h1>
</div>

![](https://static.wikitide.net/stackdwiki/2/26/834_1x_shots_so.png)

<h3 align="center">
  Wiki Guy is built from scratch to support <a href="https://conecorp.cc">CONECORP</a> wikis.
</h3>

<p align="center">
		<a href="https://sb64.conecorp.cc"><img src="https://static.wikitide.net/superblox64wiki/7/76/Super_Blox_64_wordmark_with_cubes.png" alt="SUPER BLOX 64! Wiki" height="70" hspace="15"></a>
		<a href="https://sr.conecorp.cc"><img src="https://static.wikitide.net/superstarracerswiki/0/08/Superstar_Racers_wordmark.webp" alt="Superstar Racers Wiki" height="70" hspace="15"></a>
		<a href="https://abj.conecorp.cc"><img src="https://static.wikitide.net/ablocksjourneywiki/2/24/A_Blocks_Journey_wordmark_with_doodles.png" alt="A Block's Journey Wiki" height="70" hspace="15"></a>
</p>
<br>
<p align="center">
  <a href="https://discord.com/oauth2/authorize?client_id=1472272697798037524">Add to server</a>
<br>ദ്ദി◝ ⩊ ◜.ᐟ
</p>

## Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/conecorp/wikiguy.git
   cd wikiguy
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Configure environment variables:**
   - Copy `.env.example` to `.env`:
     ```bash
     cp .env.example .env
     ```
   - Open `.env` and replace `your_discord_token_here` with your actual Discord Bot Token.

4. **Run the bot:**
   ```bash
   npm start
   ```

## Configuration

You can customize the bot's behavior by editing `config.js`. This file includes:
- **WIKIS**: Define the wikis the bot supports, including their API endpoints and article paths.
- **CATEGORY_WIKI_MAP**: Map Discord category IDs to specific wikis for context-aware embedding.
- **STATUS_OPTIONS**: Customize the bot's rotating status messages.
- **STATUS_INTERVAL_MS**: Change how often the status updates.
