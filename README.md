# Introdiction

This repository contains json formatted data files for vaious aspects of the Genesis: Battle of Champions (GBOC) card game.
The goal of this project is to provide a central resource to archive various aspects of the game for the community to use for fan projects or app development.

## Data files
The Data files are stored in data/, with the primary file being data/core/all_cards.json. 

- data/core/ contains bulk conglomerate files of all cards in the game.
- data/set/ contains card information parsed setwise.
- data/custom/ contain card information that had been modified or ecpanded upon.

## Data Structure
The all_cards data is stored in a json format, with the following structure:

- **CardObject**
  - `Idiris`: Object - Primary Key dirrived from the card name
    - `name`: String
    - `type`: String
    - `sub_type`: String
    - `rule_text`: String
    - `chi`: String
    - `health`: Integer
    - `aura`: Integer
    - `energy`: Integer
    - `awareness`: String
    - `author`: String
    - `affiliation`: [Array of Strings]
    - `sets`: [Array of Strings]
    - `printings`: Object - Contains set specific information
      - `Alpha`, `Beta`, `JAE`, ...: Object
        - `rarity`: String
        - `card_number`: String
        - `rule_text`: String
        - `flavour_text`: String (Optional)
        - `artist`: String (Optional)
        - `card_images`: [Array of URLs] (Optional)

## Contributing
If you would like to see specific data added, or have data to contribute, please open an issue or pull request.
