# DOCUMENTATION FOR MULTIMEDIA CAROUSEL GALLERY


The JSON can contain the following properties :

* instruction: This is the text you want to show above the widget as an instructional text for the multimedia carousel gallery,
* repeat: This key is used to determine whether the carousel slides will wrap around the slides. This key excepts two values, either true or false.
* slides: This key accepts an array of slides for the multimedia carousel and each slide is an object consisting of keys :
    * type : image/video/audio
        * Type can be only be of one type per slide. 
        * Image slide should be of type image.
        * Animation slide should be of type image. 
        * Video slide should be of type video. 
        * Audio slide should be of type audio.
    * link : This key contains the link to the audio/video/image/animation
    * caption : This key contains the caption for the slide. For a slide of type image, this caption text becomes the alt text for the image.

### A Demo JSON is below for reference :-

```
{
    "instruction": "Instructions : This portion will have instructions for every interactive.",
    "repeat": true,
    "slides": [{
            "type": "image",
            "link": "data/2/image01.jpg",
            "caption": "Las campañas electorales son comunes:  Pedro Pablo Kusczynski haciendo campaña electoral en Perú 2011"            
        }, {
            "type": "video",
            "link": "//d2zihajmogu5jn.cloudfront.net/elephantsdream/ed_hd.mp4",
            "caption": "Es la diapositiva de video. Gracias por ver"
        }, {
            "type": "audio",
            "link": "http://jplayer.org/audio/mp3/Miaow-07-Bubble.mp3",
            "caption": "Es la diapositiva de audio. Gracias por escuchar"       
        }
    ]
}
```

