# Scale

Scale is an easy way to access GPT-4 and other LLMs through deployed "apps" that act like API endpoints.

Currently, Scale doesn't support token streaming and configuring parameters like temperature through SillyTavern's UI.

**Scale API is not free, but offers a $5 trial if you verify your phone number.**

## Quick Start

- Create a Scale Spellbook account at <https://spellbook.scale.com> (if your country is not supported, use a VPN)
- Create an "App" with any name and description
- Create a "Variant", which sets the parameters (system prompt, model, temperature, response token limit, etc)
- Select a proper language model to be deployed (GPT-4 is recommended)
- Replace the contents of the "User" section of the prompt with the following:

>Complete the next response in this fictional roleplay chat.
>
>\{\{ input \}\}

- Configure the model parameters.
  - **Model:** GPT-4
  - **Temperature:** ~0.6 - 0.9
  - **Maximum Tokens:** 400 - 600 (depending on message length preference)
- Click "Save New Variant"
- Go to your new Variant and click Deploy
- This will create an API key and URL for your bot
- Navigate to SillyTavern, select "Chat Completion" API, and Scale source
- Paste the API key and URL into the appropriate fields and click "Connect"

## Credits

Implementation and documentation are inspired by the work of [khanon](https://github.com/khanonners): <https://github.com/khanonners/TavernAIScale>
