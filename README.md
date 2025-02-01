# buzzline-03-kilchenmann

Streaming data does not have to be simple text.
Many of us are familiar with streaming video content and audio (e.g. music) files. 

Streaming data can be structured (e.g. csv files) or
semi-structured (e.g. json data). 

We'll work with two different types of data, and so we'll use two different Kafka topic names. 
See [.env](.env). 


## Task 1. Use Tools from Module 1 and 2

Before starting, ensure you have completed the setup tasks in <https://github.com/denisecase/buzzline-01-case> and <https://github.com/denisecase/buzzline-02-case> first. 
Python 3.11 is required. 

## Task 2. Copy This Example Project and Rename

Once the tools are installed, copy/fork this project into your GitHub account
and create your own version of this project to run and experiment with.
Name it `buzzline-03-yourname` where yourname is something unique to you.
Follow the instructions in [FORK-THIS-REPO.md](https://github.com/denisecase/buzzline-01-case/blob/main/docs/FORK-THIS-REPO.md).
    

## Task 3. Manage Local Project Virtual Environment

Follow the instructions in [MANAGE-VENV.md](https://github.com/denisecase/buzzline-01-case/blob/main/docs/MANAGE-VENV.md) to:
1. Create your .venv
2. Activate .venv
3. Install the required dependencies using requirements.txt.

## Task 4. Start Zookeeper and Kafka (2 Terminals)

If Zookeeper and Kafka are not already running, you'll need to restart them.
See instructions at [SETUP-KAFKA.md] to:

1. Start Zookeeper Service ([link](https://github.com/denisecase/buzzline-02-case/blob/main/docs/SETUP-KAFKA.md#step-7-start-zookeeper-service-terminal-1))
2. Start Kafka ([link](https://github.com/denisecase/buzzline-02-case/blob/main/docs/SETUP-KAFKA.md#step-8-start-kafka-terminal-2))

## Task 5. Start a JSON Producer

In VS Code, open a terminal.
Use the commands below to activate .venv, and start the producer. 

Windows:

```shell
.venv\Scripts\activate
py -m producers.json_producer_kilchenmann
```

Mac/Linux:
```zsh
source .venv/bin/activate
python3 -m producers.json_producer_kilchenmann
```

What did we name the topic used with JSON data? 
Hint: See the producer code and [.env](.env).

## Task 6. Start a JSON Consumer

Consumers process streaming data in real time.

In VS Code, open a NEW terminal in your root project folder. 
Use the commands below to activate .venv, and start the consumer. 

Windows:
```shell
.venv\Scripts\activate
py -m consumers.json_consumer_kilchenmann
```

Mac/Linux:
```zsh
source .venv/bin/activate
python3 -m consumers.json_consumer_kilchenmann
```

## Task 7. Start a CSV Producer

Follow a similar process to start the csv producer. 
You will need to:
1. Open a new terminal. 
2. Activate your .venv.
3. 
Windows:

```shell
.venv\Scripts\activate
py -m producers.csv_producer_kilchenmann
```

Mac/Linux:
```zsh
source .venv/bin/activate
python3 -m producers.csv_producer_kilchenmann
```

## Task 8. Start a CSV Consumer

Follow a similar process to start the csv consumer. 
You will need to:
1. Open a new terminal. 
2. Activate your .venv.
3. Windows:
```shell
.venv\Scripts\activate
py -m consumers.csv_consumer_kilchenmann
```

Mac/Linux:
```zsh
source .venv/bin/activate
python3 -m consumers.csv_consumer_kilchenmann
```

## Later Work Sessions
When resuming work on this project:
1. Open the folder in VS Code. 
2. Start the Zookeeper service.
3. Start the Kafka service.
4. Activate your local project virtual environment (.env).

## Save Space
To save disk space, you can delete the .venv folder when not actively working on this project.
You can always recreate it, activate it, and reinstall the necessary packages later. 
Managing Python virtual environments is a valuable skill. 

## License
This project is licensed under the MIT License as an example project. 
You are encouraged to fork, copy, explore, and modify the code as you like. 
See the [LICENSE](LICENSE.txt) file for more.
