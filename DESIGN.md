Olaf Kroon
10787321

# Design

## Classes

The app will be created using object oriented programming. Every pad on the drum machine will be represented by a class called DrumPad . The entire drum machine will be controlled using a singleton called DrumController.

### DrumController design

``` Swift
class DrumController {

  DrumController = SharedInstance
  privit init {
  }
  
  var DrumPad = Kick
  var DrumPad = HiHat
  var DrumPad = Snare
  var DrumPad = Tom
  
  
  func replaceHits (drumKit: String) {
      // Replace the sound of every pad 
  }
  
  func addFx (reverbWetness : Int, distortionWetness : Int, delayWetness: Int) {
      // Manipulate the amount of fx on the output of the drum machine
  }
    
}

```

