SolarSystemDashboard

A modular Java Swing application that visualizes solar-system objects using enum-based data, file-loaded descriptions, dynamic icons, and interactive UI components. The project demonstrates event-driven GUI design, data modeling, and clean object-oriented structure.

 Structure

data/ — Loads text descriptions and fact data (StarDescriptionLoader, StarFactsLoader, CSV).

model/ — SolarSystemStarEnum with names, facts, and file-backed descriptions.

ui/ — Panels for layout and interaction (ControlPanel, EastPanel, WestPanel, SolarSystemStarPanel, StarFactsTableModel, etc.).

icons/ — Application and planet/star icons.

util/ — MainApp launcher class.

 Features

Displays icons, facts, and descriptions for each solar-system object.

Loads descriptions from external text files.

Fact table powered by a custom TableModel.

Event-driven updates via buttons and timer-based random selector.

Reusable and extensible panel-based UI.

 Running the App

Compile and run MainApp from the util package.
