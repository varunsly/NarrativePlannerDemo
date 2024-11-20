
# Interactive Fiction: Action Castle Simulation

This project implements a narrative planning simulation inspired by the Parsely Action Castle game, where characters interact in a structured environment governed by predefined actions and rules.

## Project Overview

The narrative planner uses **Sabre Narrative Planning** to define and simulate interactions in the Action Castle universe. The planner incorporates utility-based decision-making to achieve goals, handle character actions, and simulate various outcomes in the interactive fiction.

Key components of the simulation include:

- **Character Management**: Includes multiple characters (Player, Princess, Troll, etc.), their states, and relationships.
- **Entity Interactions**: Covers items (e.g., Crown, Candle, Sword) and locations (e.g., Cottage, Drawbridge).
- **Actions**: A rich set of precondition-effect actions such as `walk`, `give`, `unlock`, and `propose`.
- **Utilities and Triggers**: Governs character goals and dynamic changes in the narrative.

## Features

- Customizable actions and character behaviors.
- Utility-based heuristic progression search.
- Outputs include planned solutions and state transitions.

## Dependencies

- **Java**: The narrative planner leverages the Sabre library, requiring Java to execute.
- **Sabre Narrative Planning Tool**: Version 0.7 is used for this project.

## File Structure

- **Notebook File**: The notebook outlines the narrative rules and generates the problem definitions.
- **Action-Castle Problem File**: Contains the problem specification in a structured format.
- **Sabre Execution**: Java commands to run the planner and produce results.

## How to Run

1. Ensure Java is installed on your system.
2. Clone this repository.
3. Install the Sabre Narrative Planning Tool by placing the `sabre.jar` file in the `lib` folder.
4. Execute the notebook or run the Sabre command manually using:
   ```bash
   java -jar sabre/lib/sabre.jar -v -p action-castle.txt -h h+ -el 1
   ```

## Results

The planner outputs the optimal sequence of actions for achieving the defined goals. Examples include:

- Unlocking doors and walking between locations.
- Interacting with NPCs like the Troll and Princess.
- Achieving character-specific goals like marriage or becoming crowned.

## Customization

You can customize the problem by editing the following sections in the notebook:

- **Entities**: Add or modify characters, items, and locations.
- **Actions**: Define new actions with preconditions and effects.
- **Utilities**: Modify character goals and priorities.

## References

- [Parsely Action Castle Game](http://memento-mori.com/pdf/parsely-preview-n-play-edition)
- [Sabre Narrative Planner](https://github.com/stephengware/sabre)

## License

This project is licensed under the MIT License. See the LICENSE file for details.
