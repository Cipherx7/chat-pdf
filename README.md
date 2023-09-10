# Chat-pdf
Discription
This Python script is a Telegram bot that allows users to send a PDF file to be edited. The bot responds to two commands: `/start` and `/edit`. Here's a description of the code:

1. **Imports**: The necessary libraries and modules are imported. These include `logging` for logging information, `os` for interacting with the operating system, and the `telegram.ext` module for working with the Telegram Bot API. Additionally, the `pypdf2` library is imported for working with PDF files.

2. **Logging Configuration**: Logging is configured to display information about the bot's activity.

3. **Command Handlers**:
   - `start(update, context)`: This function is called when the user sends the `/start` command. It replies with a welcome message.
   
   - `edit_pdf(update, context)`: This function is called when the user sends the `/edit` command. It downloads the PDF file sent by the user, opens it using `PyPDF2`, applies an example edit (adding a watermark), saves the edited file, sends it back to the user, and then deletes the temporary files.

4. **Main Function**:
   - `main()`: This function sets up the `Updater`, adds the command handlers, starts the bot, and allows it to continuously poll for updates.

5. **Token**:
   - The `TOKEN` placeholder should be replaced with the actual token provided by the BotFather when you create a bot on Telegram.

This script creates a basic PDF editing bot. Keep in mind that for more complex edits or additional functionalities, you may need to expand on the `edit_pdf` function and potentially incorporate other libraries or services. Additionally, ensure that you have the necessary permissions and packages installed on your system for the script to run successfully.
