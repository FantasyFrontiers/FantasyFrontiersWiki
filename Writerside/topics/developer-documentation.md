# Developer Documentation

## Introduction

This section provides an overview of the project, its purpose, and objectives.

---

## Prerequisites

### Software Requirements

- Java 17 or higher
- Gradle

---

## Setup and Installation

### Installing Java

- Install a Java 17+ Development Kit of your choice. We recommend [Adoptium Eclipse Temurin](https://adoptium.net/)

### Installing Gradle

- Follow the instructions to install Gradle [here](https://gradle.org/install/).

### Loading Dependencies

- After cloning the repository, navigate to the project root and run the following command to load dependencies:
```
gradle --refresh-dependencies
```
- If you use IntelliJ (or any other advanced IDE), this step will be done automatically upon loading (see [Development Environment](#development-environment)).

---

## Development Environment

For development, we recommend using IntelliJ IDEA. You can download it [here](https://www.jetbrains.com/idea/download/).
You will also need a database for development. We recommend using [MariaDB](https://mariadb.org/).
Additionally, you will need a Discord bot token. You can get one by creating a new application [here](https://discord.com/developers/applications).

### Setting up IntelliJ

- Open IntelliJ and select "Open or Import".
- Navigate to the project root and select `Open as Project`.
- Wait for IntelliJ to load the project and import all gradle dependencies.
- Once the project is loaded, copy the `.env.example` file and rename it to `.env`.
- Fill in the values in the `.env` file with your database and Discord bot credentials.
- Run the `Main` class to start the bot.
  - You can use the `migrate` flag to seed the database with the default data. This is only necessary for the first run.
- You can now use IntelliJ to develop the project.

---

## Building the Project

1. Navigate to the project root.
2. Run the following command to build the project:
```
gradle build
```
3. The shadowed JAR file (for production use) will be generated in `build/libs`.

---

## Contributing Guidelines

Please read our [Contribution Guidelines](contribution-guidelines.md) before contributing to the project.

---

## Common Issues and Troubleshooting

This section lists common issues that developers might encounter and provides solutions or workarounds.

### Gradle Build Errors

- If you encounter any errors while building the project, try running the following command:
```
gradle clean
```
- If the error persists, try deleting the `.gradle` folder in the project root and running the `--refresh-dependencies` command again.

### IntelliJ Errors

- If you encounter any errors while loading the project in IntelliJ, try invalidating the cache and restarting IntelliJ.
