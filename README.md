---

# Telegram Member Scraper & Adder Bot

This Python tool allows you to scrape members from a Telegram group and add them to another group. The bot uses the Telethon library to interact with the Telegram API.

## Features

- **Scrape Members:** Extract members from a target group and save them to a CSV file.
- **Add Members:** Add the scraped members to your group in batches to avoid rate limits.
- **Multi-account support:** Use multiple Telegram accounts to distribute the load.

## Requirements

- Python 3.7+
- Telegram API credentials (API ID and API Hash)
- Telethon library

## Installation

1. **Clone the repository:**

```bash
git clone https://github.com/Frex-IQ/TelegramMemberAdder.git
cd TelegramMemberAdder
```

2. **Install dependencies:**

```bash
pip install telethon
```

3. **Configure your Telegram API credentials:**

You will need to obtain your API ID and API Hash from [my.telegram.org](https://my.telegram.org). Once you have them, you will be prompted to enter them when running the script.

## Usage

1. **Run the script:**

```bash
python3.12 app.py
```

2. **Provide the required inputs:**

- **API ID and API Hash:** Your Telegram API credentials.
- **Phone Numbers:** The phone numbers of the Telegram accounts you will use (with country code).
- **Group Username:** The username of the group you want to add members to.
- **Target Group Link:** The invite link or username of the group you want to scrape members from.

3. **Follow the OTP process:**

When prompted, enter the OTP sent to your phone number for authentication.

4. **Scrape and Add Members:**

The script will first scrape members from the target group and then add them to your group in batches, with delays to avoid Telegram's rate limits.

## Customization

You can adjust the following parameters in the script:

- **CSV File:** The name of the CSV file where scraped members are stored.
- **Number of Users Per Account:** Number of users to add per account before taking a break.
- **Delay Between Adds:** Delay between each add action in seconds.
- **Delay Between Batches:** Delay between batches of adding users.

## Logging

The script logs its actions to a `telegram_bot.log` file, including errors, successes, and rate limit avoidance.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue if you encounter any problems.

## Disclaimer

This script is for educational purposes only. Use it responsibly and ensure you comply with Telegram's terms of service. The authors are not responsible for any misuse of this tool.

## License

This project is licensed under the MIT License.

---
