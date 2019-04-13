## BACKGROUND

Blind people are people who have complete or nearly complete vision loss and may result difficulties in daily life routines such as walking, socialising and reading. As of 2015 there were 940 million people with some degree of vision loss (GBD 2015 Disease and Injury Incidence and Prevalence, Collaborators)<sup>1</sup>. Blind people do lead a normal life with their own style of doing things. But, they definitely face troubles due to inaccessible infrastructure and social challenges.

According to Erin Brady et al., the most common accessibility issues encountered in everyday life is Identification, making up 41% of the total sample. More than half of Identification questions were simple, “No Context” questions (58%) where the user did not provide any information about the subject of the object (Visual Challenges in the Everyday Lives of Blind People, CHI 2013: Changing Perspectives, Paris, France)<sup>2</sup>.

Other problem that are faced by blind people are locating object. Popular culture depicts that if one of the senses of a person stops working, the others become sharper. Blind people may rely more on their other senses and develop a strong memory, but this may not be well enough to identify object and their location. Blind people must memorise the location of every obstacle or item in their home environment. Any changes in location can put burden to the person to search the item again with varying difficulties.

Despite of the challanges faced by the blind, the most valuable thing for a disabled person is gaining independence. A blind person can lead an independent life with some specifically designed adaptive things for them. There are lots of adaptive equipment that can enable a blind person to live their life independently but they are not easily available in the local shops or markets. They have to put much effort to get each equipment that can take them one step closer towards independence (Lalit Kumar, Daily Life Problems Faced by Blind People)<sup>3</sup>.

Computers and the Internet are two of the most significant developments since the invention of braille, as for the first time ever many blind and partially sighted people have access to the same wealth of information as sighted people and on the same terms. Computing technology is promising greater accessibility to information, services, and society. (Anne Jarry et al., Blind Adults’ Perspectives on Technical Problems and Solutions When Using Technology)<sup>4</sup>.

With the premise above, we came up with a powerful and easy-to-use solution for the blind to identify and discover the location of objects that we called **"UNCOVer: UNsighted COmputer Vision"** 

## UNCOVer: UNsighted COmputer Vision

UNCOVer is an accessibility tool for sightless person that is worn like a sunglasses. UNCOVer will use the technology of Artificial Intelligence to aid user in identifying and locating objects and texts accurately.

UNCOVer differentiates itself from the currently available products by offering multiple object detection complete with object name and location, powerful and precise object description by detecting the object pointed by the user's finger, and optical character recognition that enables the user to "hear" the characters, all in a single, easy-to-use package.

UNCOVer core components consists of a single camera positioned to mimic user's field of view. This camera will be used to capture an image of the objects and texts to be analysed. To facilitate user with easy and simple to use interface, UNCOVer will feature a microphone powered by speech recognition so that the user can give command directly by speaking without pressing any button. All information will be given to the user as speech via the provided earphone.

UNCOVer's prototype will use a single Raspberry Pi 3 Model B to handle and process the information. To detect object and recognise characters, UNCOVer will be powered by Azure Cognitive Service for reliable object & character recognition and speech services to deliver the best possible experience.

## HOW UNCOVer WORKS

While the device is on, the microphone will constantly monitor for user's voice. The user can speak "What's in front of me" in order for UNCOVer to capture an image. After that, the image will be sent to Azure Vision API for object detection purposes. The API will then return information of object names and position in JSON format. If there are no object detected, then text-to-speech engine will output "There are no detected objects in front of you" through the speaker. If there are object(s) detected, then the device will be speaking each object(s) name and location. 

Alternatively, if a finger pointing to a specific object is detected, then the device will speak the pointed object's name. After that, the microphone will continue to monitor user commands. If the user say "Turn off", then the device will stop monitoring and turn off. Else, the device will keep monitoring and work as described.

For additional information, please visit out project website: https://unblinded.github.io
