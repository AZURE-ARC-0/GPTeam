<p align="center">
  <h1 align="center">GPTeam: Collaborative AI Agents</h1>
  <p align="center">
    <img src="https://img.shields.io/github/stars/101dotxyz/gpteam.svg?style=for-the-badge">
    <img src="https://img.shields.io/github/license/101dotxyz/gpteam.svg?style=for-the-badge">
    <br />
    <a href="#"><b>View Discord Demo</b></a>
    ·
    <a href="https://github.com/101dotxyz/gpteam/issues"><b>Report Bug</b></a>
    ·
    <a href="https://twitter.com/101dotxyz"><b>Follow</b></a>
  </p>
    <div align="center">
    <img src="assets/gpteam.png" alt="GPTeam" width="400" height="267" />
  </div>
</p>

## About GPTeam

GPTeam uses GPT-4 to create multiple agents who collaborate to achieve predefined goals. The main objective of this project is to explore the potential of GPT models in enhancing multi-agent productivity and effective communication.

## How it works

GPTeam employs separate agents, each equipped with a memory, that interact with one another using communication as a tool. The implementation of agent memory and reflection is inspired by [this research paper](https://arxiv.org/pdf/2304.03442.pdf). Agents move around the world and perform tasks in different locations, depending on what they are doing and where other agents are located. They can speak to eachother and collaborate on tasks, working in parallel towards common goals.

## Getting started

To begin exploring GPTeam, follow these steps:

1. Clone the project repository to your local machine
2. Move to the repository: `cd gpteam`
3. Run `python setup.py` to check your environment setup and configure it as needed
4. Update the environment variables in `.env` with your API Keys. You will need an OpenAI API key, which you can obtain [here](https://platform.openai.com/account/api-keys). Supplying API keys for optional services will enable the use of other tools.
5. Launch the world by running `poetry run world`

Now you can observe the world in action and watch as the agents interact with each other, working together to accomplish their assigned directives.

## Changing the world

To change the world, all you need to do is:

1. Make changes to the `config.json` by updating the available agents or locations
2. Reset your database: `poetry run db-reset`
3. Run the world again: `poetry run world`

## Setting up the Discord Integration
Read through the dedicated [Discord setup docs](DISCORD.md)

## Contributing

We enthusiastically welcome contributions to GPTeam! To contribute, please follow these steps:

1. Fork the project repository to your own account
2. Create a new branch for your changes
3. Implement your changes to the project code
4. Submit a pull request to the main project repository

We will review your pull request and provide feedback as necessary.

## License

Licensed under the [MIT license](LICENSE.md).