# 2D Worlds dataset


This is a dataset of 2D worlds.

Each world is a rectangular HxW grid, each cell is encoded by color in the range 0-9
The size of grid is limited to H = [0..32] and W = [0..32]. 
The grid is encoded as a standard 2d array [[]] 

All worlds are grouped by their hidden similarity/build principles and each class has a unique 8-digit hexdecimal id (e.g. 00576224), and comprises of example and test parts.

The train subset consists of input-output pairs of worlds, while the test subset has only input world.   


Below is an example of one class of the world with hid=00576224, providing 2 traing pairs and 1 test input.

```json
{
  "00576224": {
    "train": [
      {"input": [[7, 9], [4, 3]], "output": [[7, 9, 7, 9, 7, 9], [4, 3, 4, 3, 4, 3], [9, 7, 9, 7, 9, 7], [3, 4, 3, 4, 3, 4], [7, 9, 7, 9, 7, 9], [4, 3, 4, 3, 4, 3]]}, 
      {"input": [[8, 6], [6, 4]], "output": [[8, 6, 8, 6, 8, 6], [6, 4, 6, 4, 6, 4], [6, 8, 6, 8, 6, 8], [4, 6, 4, 6, 4, 6], [8, 6, 8, 6, 8, 6], [6, 4, 6, 4, 6, 4]]}
    ], 
    "test": [
      {"input": [[3, 2], [7, 8]]}
    ]
  }
} 
```

