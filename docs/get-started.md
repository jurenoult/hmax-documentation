# Get started

Open the project with Matlab.

First, you need to train the model
```matlab
hmax('../dataset/training/', 'Train', true)
```

Then run it on your dataset
```matlab
hmax('../dataset/test/')
```

This will read recursively the `../dataset/test/` folder architecture and create a similar one in the `./result` folder.  
Each images will give a Matlab binary file containing the HMAX encoding.

If your folders name corresponding to the class name of the images, then you can run the following command:
```matlab
T = classifier.loadC2s('./results/')
```

Where `T` is a table containing the HMAX encoding with the corresponding encoding.

