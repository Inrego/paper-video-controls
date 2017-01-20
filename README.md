# \<paper-video-controls\>

A video container element that will provide material design controls for the video. Easy to use and easy to style. 
The interface part is based heavily off of [`<paper-video>`](https://github.com/AKHXtern/paper-video) by [AKHXtern](https://github.com/AKHXtern/paper-video).

To better suit my needs, I made some quite big changes to how the element works and interacts with the video element compared to `<paper-video>`.
Where `<paper-video>` tries to replace the video element, this is instead just a container for the video element.
This provides some advantages. I the biggest one is, that there is no need to replicate all video properties and functions on my element.
Since you will still have the original video element in your DOM, you can still do databindings on it, call functions on it and all the other fun stuff you normally can do with the HTML video element.

Here's an example of usage:

    <paper-video-controls>
        <video>
            <source src="demo.mp4" type="video/mp4">
        </video>
    </paper-video-controls>

This simple example will put material design controls on top of the video.