# SJFJavaFX

A JavaFX-based application that demonstrates the Shortest Job First (SJF) CPU scheduling algorithm with a visual Gantt chart.

SJFJavaFX helps students understand how an operating system schedules processes based on their CPU burst times. The application presents the scheduling sequence visually, making it easier to study process execution and scheduling behavior.

This project was developed by Ichiro Yamazaki in January 2024.

## Features

- Shortest Job First Scheduling: Demonstrates the SJF CPU scheduling algorithm.
- Gantt Chart Visualization: Displays the process execution sequence in a Gantt chart.
- JavaFX Interface: Uses JavaFX to provide a graphical user interface.
- Process Scheduling Demonstration: Helps visualize how processes are arranged according to their burst times.
- Educational Purpose: Supports learning about operating systems and CPU scheduling concepts.

## Requirements

- Java Development Kit (JDK) compatible with your JavaFX version.
- JavaFX SDK and libraries.
- A JavaFX-compatible IDE, such as IntelliJ IDEA, Eclipse, or NetBeans.
- The project source files.

## Installation and Setup

### 1. Install Java

Download and install a compatible JDK from a trusted Java distribution.

Verify your installation:

```bash
java -version
javac -version
```

### 2. Download JavaFX

Download the JavaFX SDK from the official OpenJFX website:

https://openjfx.io/

Extract the SDK and locate its `lib` directory.

### 3. Configure Your IDE

Configure your IDE to recognize the JavaFX libraries. Depending on your setup, you may need to add the JavaFX SDK to your project dependencies and configure the JavaFX module path.

For a modular JavaFX project, your VM options may look like this:

```bash
--module-path "PATH_TO_FX/lib" --add-modules javafx.controls,javafx.fxml
```

Replace `PATH_TO_FX` with the actual path to your JavaFX SDK. Adjust the modules to match the project's imports and configuration.

### 4. Open and Run the Project

1. Open the project in a JavaFX-compatible IDE.
2. Configure the JDK and JavaFX SDK.
3. Set the correct main class.
4. Build and run the application.

The exact setup may vary depending on the IDE and project structure.

## How SJF Scheduling Works

Shortest Job First selects the eligible process with the shortest CPU burst time for execution.

For non-preemptive SJF, once a process starts running, it continues until completion. The resulting execution order can be represented using a Gantt chart.

For example:

```text
Process:  P1    P2    P3
Burst:     6     2     4
```

If all processes arrive at time zero, the execution order is:

```text
0    P2    2      P3      6       P1       12
|---------|---------------|----------------|
```

This example illustrates non-preemptive SJF scheduling when all processes are available at the beginning.

## Project Information

- Project Name: SJFJavaFX
- Programming Language: Java
- GUI Framework: JavaFX
- Algorithm: Shortest Job First (SJF)
- Developer: Ichiro Yamazaki
- Build Date: January 2024
- Project Category: Operating Systems and CPU Scheduling

## Disclaimer

This project is intended for educational purposes. Scheduling behavior and supported inputs depend on the implementation included in the source code.

## License

No license has been specified. All rights are reserved by the respective copyright holder unless a license is added to this repository.
