# Game bot - 1to50

Bot to play the 1to50 (zzzscore.com/1to50/) online game

### Blog

Read more about the intuition and howto @ [here](https://medium.com/@MohitMayank/how-i-beat-the-online-game-1to50-with-neural-network-6ded10a986e4?source=friends_link&sk=157956cec8561f666a5f664e0abbe8ea).

### Usage

To load the image and train the neural network

```
from game_bot_1to50 import *
model = train_network(image_directory = "imgs")
save_model(model, "1to50_trained_model.h5")
```
To load the model and play the game

```
model = load_model("1to50_trained_model.h5")
# Define the co-ordinate of the gme board
image_location = {'top': 239, 'left': 486, 'width': 380, 'height': 378}
play_game(image_location)

```
