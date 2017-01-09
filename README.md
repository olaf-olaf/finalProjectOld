# finalProject
A sample based digital drumpad for your iPhone. 

## Problem
Musicians like to jam all day long. However, when there's a jam going on in places without proper sound isolation a drum kit is simply to loud. Drumpad is an application that will allow the user to use his screen as a drumkit by converting the screen of his device into a Roland SPD style drumpad. Now musicians can lay down some drum with a variety of sounds without being evicted due to noise complaints. 


![](doc/sketch.png)

## External libraries

For this project I will either use the AVAudioPlayer class in swift or the audiokit library. Audiokit has more potential for extending functionality of the app than AVAudioPLayer but is really synthesis focused instead of sample focused. I have to consider whether audiokit will reduce the amount of code needed to implement this project. AVAudioPlayer is really basic, which will 

## Decompsing the app

### View

The app will only have one view. This view consist of 4 pads (kick, hi hat, snare and tom) and a drop down menu in which users can select different drum kits. 

### Model

The only data this app needs to save are some small audio files. These will probably be saved in a dictionairy that will correspond with the drop down mene.

### Controller

The view and the model will work together via the controller. Samples will be triggerd via buttons and drum kits will be selected via a drop down menu. 

## Possible Problems / limitations

- Not being able to play two sounds simultaneously

This problem could arise if an audio player can only play one file at the time. The obvious solution for this problem is to use one audio player for each trigger.

- Mixing sound without code

Mixing the samples outside of Xcode (for example volume, EQ and panning) will save lots of code. However, it could create a problem when adding features that enable users to mix their sounds in app.

