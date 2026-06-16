# MP

MP is a small data-support folder used by the parking automation system. It stores parking-related JSON data that can be read or updated by other modules in the project. The current folder contains a `data` directory with a `parked.json` file, which keeps track of the parking slots that are currently occupied.

The `parked.json` file stores occupied parking slot IDs in JSON array format. For example, if slots `B1` and `B2` are occupied, the file contains `["B1", "B2"]`. This data can be used by the parking monitoring system, dashboard, or any connected application to display live parking availability.

This folder is mainly used as a shared data location between the parking detection system and other parts of the application. The parking system updates this file automatically when it detects occupied slots from video processing.

To use this project, make sure the connected parking automation script writes updated slot information into `data/parked.json`. Any frontend or backend system can then read this file to show the latest parking status.

Before pushing this project to GitHub, avoid committing temporary or system-generated files. If this folder is part of a bigger parking management system, include the main application files along with this data folder for better project completeness.

Developed by Mithun Ravi.
