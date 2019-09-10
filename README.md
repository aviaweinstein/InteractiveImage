# InteractiveImage
Interact with images by dragging either mouse on computer or finger on touch screen.

## How to get started

### Download and include the code
1. From this repo, download and add drag_move.js to your app.
2. Include jquery and drag_move.js in the head of your app, like so:
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
        <script src="assets/javascript/drag_move.js"></script>

### Set up your images
1. Name your series of images as follows: <number starting at 0>-<your image name>.<your image file extention>. If your image frames were sunrise.jpg, then you would take each frame of the images and name 0-sunrise.jpg, 1-sunrise.jpg, 2-sunrise.jpg, etc.
2. Add your series of images to your app and take note of the file path.
3. Include the <img> tag, set the href to the first image you want to display and give the tag an identifiable id, `#move` is defaulted.

### Make your image interactive
In your javaScript, call interactiveImage(...) with the appropriate parameters.


## Function parameters

interactiveImage(pathToImage = 'assets/images/', fileName = 'image.jpg', totalFrames = 12, targetedImage = '#move')
The interactiveImage function takes in 4 parameters. All of which have defaults as shown above.
* `pathToImage` is the relative path to your images
* `fileName` is the name if the images files without the leading number or dash
* `totalFrames` is the largest number image you have. Remember the numbering starts at 0, so if you have 11 images `totalFrames` should be set to 10
* `targetedImage` is the id, class, or tag (or some combo of these) that targets the img tag where the images are sourced.
