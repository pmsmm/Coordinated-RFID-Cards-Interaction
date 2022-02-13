# Coordinated RFID Cards Interaction

The Coordinated RFID Cards Interaction is a mini game that was developed for my Master Thesis "Developing a Support Infrastructure for an Escape The Room and Peddy Paper Games".

This mini game, or interaction as I so call it, was developed to be part of an Escape the Room game that was also developed as part of my thesis. Since this interaction can work as a standalone mini game I decided to place it here for anyone interested in using it.

## List of Components

- MFRC522 RFID Reader (2x);
- Piezzo Speaker (1x);
- Arduino Nano (1x);

![WiringDiagram](images\CoordinatedRFIDCardsElectricalSchematic_bb.jpg)

In order to fully assemble the Interaction, so as to look like the picture below, you will also need to 3D Print the enclosure that can be found [here](enclosure/).

![AssembledInteraction](images\AssembledInteraction.jpg)

## The Purpose of The Game

The Coordinated RFID Cards Interaction does not have a specific purpose. It was developed to make use of the RFID technology and the many possibilities it gives us, allowing us to develop several types of interactions using this technology alone. 

In this case the purpose of this interaction is for people to use an RFID Card and RFID Tag and scan them within 1.5 seconds of each other (Hence the 'Coordinated' in the name of the interaction). If both the card and the tag are scanned within 1.5 seconds of each other then the player was able to successfully solve the interaction, otherwise he/she will need to try again.

## Instructions

First start by uploading the code to your Arduino Nano (This is the one I used so I can only guarantee proper working with this micro-controller).

### Starting the Game

To start the mini game you must first type in the Arduino IDE serial monitor the following:

- > COM:START;ID:123456789

After this, you can scan the tag/card and proceed to solve the interaction.

## WARNING

The source code for this interaction contains a lot of logic that was made to communicate with the infrastructure that was developed for my thesis and therefor it is not as clean as it could be when compared to a mini game that is developed with the intent of being used by the Arduino IDE directly.