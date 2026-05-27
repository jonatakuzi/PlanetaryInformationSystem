# PlanetaryInformationSystem

A modular Java Swing application that displays an interactive solar system dashboard. Planets and stars are represented as enums with rich attributes, descriptions loaded from external text files, and facts rendered in a live-updating table.

## Features

- **Enum-based data model** — `SolarSystemStarEnum` stores names, physical facts, and references to file-backed descriptions
- - **File-loaded descriptions** — `StarDescriptionLoader` reads from `star_descriptions.txt` at runtime
  - - **Dynamic fact table** — custom `StarFactsTableModel` populates a `JTable` from enum data
    - - **Planet icons** — per-planet `.png` assets rendered in the UI panels
      - - **Timer-based random selector** — `RandomStarTimer` cycles through objects on a schedule
        - - **Multi-panel layout** — `ControlPanel`, `EastPanel`, `WestPanel`, and `OrbitPanel` compose the full dashboard
          - - **JUnit test coverage** — tests for enum behavior, description loader, and timer logic
           
            - ## Tech Stack
           
            - - Java 17+
              - - Java Swing (`JFrame`, `JPanel`, `JTable`, `JLabel`, `JScrollPane`)
                - - Custom `AbstractTableModel` subclass
                  - - `javax.swing.Timer`
                    - - JUnit (unit tests)
                      - - IntelliJ IDEA
                       
                        - ## Project Structure
                       
                        - ```
                          PlanetaryInformationSystem/
                          ├── MainApp.java                  # Application entry point
                          ├── SolarSystemStarEnum.java      # Enum with planet/star attributes
                          ├── StarDescriptionLoader.java    # Reads descriptions from text file
                          ├── StarFactsLoader.java          # Loads facts for the table
                          ├── StarFactsTableModel.java      # Custom JTable model
                          ├── RandomStarTimer.java          # Timer-driven auto-selection
                          ├── ControlPanel.java             # Button panel for planet selection
                          ├── EastPanel.java / WestPanel.java / OrbitPanel.java
                          ├── SolarSystemStarPanel.java     # Main display panel
                          ├── star_descriptions.txt         # External description file
                          └── [planet icons].png            # Per-planet image assets
                          ```

                          ## Running the App

                          1. Clone the repo
                          2. 2. Open in IntelliJ IDEA
                             3. 3. Compile and run `MainApp.java`
                               
                                4. ## Concepts Demonstrated
                               
                                5. - Java enums with fields, constructors, and methods
                                   - - External file I/O integrated into a GUI application
                                     - - Custom `TableModel` for dynamic `JTable` data binding
                                       - - Multi-panel Swing layout composition
                                         - - Timer-driven UI updates
                                           - - JUnit testing for non-UI logic (loaders, enums, timers)
