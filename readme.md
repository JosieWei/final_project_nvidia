#The Ultimate Manga Machine 

 Add short description of project here > 
This project can analyze my collection of manga and tell me what volume each manga I show to the camera is. I chose this project because I love manga and have a lot of volumes, so having a bot that can easily tell me what volumes they are(nomatter the language, because at times it gets hard), would mak emy life easier(instead of just searching on google what the volume list is. 
![add image descrition here](direct image link here)

## The Algorithm

Add an explanation of the algorithm and how it works. Make sure to include details about how the code works, what it depends on, and any other relevant info. Add images or other descriptions for your project here. 

First, I imported a couple of things(shown below in required libraries). Then I defined my camera(which was easy as it was a logi 2700, in doing this I set the height and length of my camera while confirming its capture device number, and I made sure the camera would turn on with a boolean. I defined my categoried, which were volumes 1-13(these are all the volumes of my favorite manga, and they are in most need of this programs, as multi-languages are present here). And then I defined 4 datasets(this was mainly for testing each dataset to see what method would be most effective, so I basically could have just used 1). Then I made sure all of the images would be of the same size, using a transforms variable. Then I made a directory to store the data. Then I boot the dataset I am on, by making a new container that holds the dataset I am on, which would be position[0]. Since I was using Jupyter notebook for my project(for ease of taking the pictues), I had to create the camera's image preview, and the widgets that show up. I did this by using the .Dropdown, .IntText, .Button, functions, with a discription(what shows up as the icon). Then, when I add an image during the training proccess, the count goes up, through .value(). I then use def(), to set the current dataset, I also use def() to up the "count"(which is going up through the list) when I select a different category, and to actually save the work I also need to use this(along with .save_entry. For this I used RESNET-18, so I had to use my previously imported torch modules, and using this ad my model to make it work. I defined load_model and save_model(using my previously defined "save" to do so), and I also had to make the widgets for them as well. Next, I had the challenge of both the stop/live widgets, but what was even harder, was the prediction scrollers, which required me to use a def and if statement, so it can know if in the live function, the predicting sliders can work, and accurately meassure the accuracy. ![2022-07-08 (7)](https://user-images.githubusercontent.com/108949653/178089723-889021df-42b2-4f64-b457-0e86194b0b9a.png)  <-- This is an image of some of the code I used, since explaining it would take a while. And then I set epochs, and batch_size, for the training process. I defined the training process, and used if statements for it. ![2022-07-08 (9)](https://user-images.githubusercontent.com/108949653/178089820-f44f595c-e78a-47b5-93ed-a223376e6817.png) <-- this is another image of some of the code I used. I had to run the model, in order to get my output, and do a couple of if statements, to show when it is in the training progress. The next, and basically last step was to show the display, or at least put everything created onto the display, I had to use a couple of references for this, but I ended up with 
![2022-07-08 (11)](https://user-images.githubusercontent.com/108949653/178090443-96446265-66b0-4e95-b876-9c49052eba0b.png) <-- This is the code. And that is all of the steps(and some of my thought proccess), to this project. I do want to mention that I used some references for particular sections of this. 

 
## Running this project

1. Add steps for running this project.
You can run this project in the Jupyter notebook, I made the code that way so that you can use the widgets(as that was easiest for me). But I do want to mention that this program is pretty specific to my managa, so it would be hard to use for general purpose(like I don't even know if other people could run the command, as I think that the code I uploaded is a little outdated, as in I made some changes to them, so if there is an error message or the code does not run then message me or just watch the video demonstration. And I think I might have the physical training on my jupyter account, so I would really recommend watching the video(sorry for the inconviencce, I did run into a lot of technical difficulties during this process so I wouldn't be suprised if another arose). 
2. Make sure to include any required libraries that need to be installed for your project to run.

First, I imported a couple of things(shown below in required libraries). This includes: My usb camera, from dataset import ImageClassificationDataset(the dataset), ipywidgets, traitlets, from IPython.display import display, from jetcam.utils import bgr8_to_jpeg, torchvision, torch, threading, time, from utils import preprocess, torch.nn.functional(as f), OS, and IPython(this time to shut down my camera). 
[View a video explanation here](video link)
