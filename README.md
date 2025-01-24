# Polpo-Cheat
This extension allows you to see the answers of any task, without Polpo or your teacher knowing. The use of this extension is completely invisible in your digital footprint, it is secure to use this extension. Although teachers might catch on if they're looking at your screen and constantly see the answers, so use this cheat wisely. I am not responsible if you get expelled from school.
Your personal information is never collected or distributed by Polpo-Cheat.

## Installation

1. Clone or download this repository.
2. Unzip the downloaded file and put the files in a folder.
3. Open your browser's extension management page (usually `chrome://extensions` or `about:addons` depending on the browser).
4. Enable Developer Mode if using Chrome.
5. Load the folder as an unpacked extension.

## Usage

Once the extension is loaded and active, navigate to your Polpo tasks. Press `Alt + H` to toggle vissible answers and tips on or off. Answers will be highlighted.

### Legal notice
As stated under [Polpo's terms of conditions](https://www.polpo.be/legals/gebruiksvoorwaarden), any form of hacking or attempt to hack a component of POLPO could be considered as such, and result in an account termination.
However, this extension cannot be considered as such, since it is not breaking into POLPO's systems. It does not provide you with any form of private or sensitive information. The answers have always been available to the said client. This extension does not make any requests to the server and never contacts POLPO's system. Therefor it is merely a useful user-tool.
If requested by Die Keure, we will oblige and delete the extension under the condition that POLPO enhances their encryption security and promises their platform to make a better product.

### How does Polpo-Cheat work?
Polpo-Cheat uses CryptoJS like Polpo uses. The decryption format is AES. It uses the iv (initialization vector), the salt, and the ct (which is the cyphertext). The iv, salt and ct are all provided by the Polpo's servers. It only needs a password to finally decrypt the ct. Oh, how would I ever get that password? `this.pass = "ludo"`... The password is hardcoded into every client and is not even dynamic.

Finally, the ct has been decrypted. The output is an xml containing questions, answers, and settings for that Task. At last, Polpo-Cheat highlights the answer to the question.
