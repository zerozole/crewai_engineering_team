# EngineeringTeam Crew

This project is based on crewai agentic framework. It is an engineering team consisting of four members:

1. Engineering lead
2. Frontend engineer
3. Backend engineer
4. Test Engineer

This project addresses the problem of building a simple account management system for a trading simulation platform, enabling users to create accounts, deposit and withdraw funds with safeguards against negative balances, record buy and sell transactions while preventing purchases beyond available funds and sales beyond owned shares, track holdings, compute total portfolio value using a provided share price function with test prices for AAPL, TSLA, and GOOGL, calculate profit or loss relative to initial deposits, and list all transactions so users can view their financial activity at any point in time.

Test engineer and backend engineer ran the code in a docker cointainer for testing out the code. The frontend engineer prepared a Gradio UI.


## Installation

Ensure you have Python >=3.10 <3.13 installed on your system. This project uses [UV](https://docs.astral.sh/uv/) for dependency management and package handling, offering a seamless setup and execution experience.

First, if you haven't already, install uv:

```bash
pip install uv
```

Next, navigate to your project directory and install the dependencies:

(Optional) Lock the dependencies and install them by using the CLI command:
```bash
crewai install
```
### Customizing

**Add your `OPENAI_API_KEY` into the `.env` file**

- Modify `src/engineering_team/config/agents.yaml` to define your agents
- Modify `src/engineering_team/config/tasks.yaml` to define your tasks
- Modify `src/engineering_team/crew.py` to add your own logic, tools and specific args
- Modify `src/engineering_team/main.py` to add custom inputs for your agents and tasks

## Running the Project

To kickstart your crew of AI agents and begin task execution, run this from the root folder of your project:

```bash
$ crewai run
```

This command initializes the engineering_team Crew, assembling the agents and assigning them tasks as defined in your configuration.

After this app.py file will be generated in the output folder in your directory. Run it for the application created by the engineering team to be launched.




