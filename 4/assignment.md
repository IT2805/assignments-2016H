# Assignment 4: HTML5 Video and CSS

In this exercise you are going to use the video element to embed a video on a website and make it responsive, ensuring that it looks good on devices with different resolutions.

## Part 1: Playing Videos in HTML (20%)
Attached you will find an HTML file that you are going to embed a video in. The video is supplied in three different formats: OGG theora (````hovedbygget.ogv````), WebM (````hovedbygget.webm````) and MPEG-4 (````hovedbygget.mp4````).

Your first task is to alter the ````video```` element in the ````index.html```` file such that the MPEG-4 video automatically starts playing when a visitor enters the webpage. Make sure that the audio is disabled and that the video starts over when it is finished playing.

## Part 2: Ensure Browser's Support (20%)
The following table shows which video formats each major desktop web browser supports.

| Browser (version)          | Theora (OGG) | H.264 (MP4) | WebM |
|----------------------------|--------------|-------------|------|
| Internet Explorer (11)     |      No      |     Yes     |  No  |
| Mozilla Firefox (46)       |      Yes     |     Yes     |  Yes |
| Mozilla Firefox (46 Linux) |      Yes     |     No      |  Yes |
| Chrome (51)                |      Yes     |     Yes     |  Yes |

Ensure that visitors with browsers that do not support one particular format is served another instead. All three file formats must be supported by the ````video```` element.


## Part 3: Image Placeholder Fallback for Video (10%)
Browsers that do not support any of the provided formats be shown a placeholder image instead (````hovedbygget.png````) of the video.

You can emulate the behavior of an unsupported format by following [these](http://www.trishtech.com/2012/04/disable-html5-media-in-mozilla-firefox/) instructions for Firefox.

## Part 4: Responsive Design (20%)
Although the size of the video element changes proportionally to the window width of the browser, the article body does not. Change the CSS so that the article always has a margin of 20% of the width of the browser. The article should also be positioned in the center - but the text should stay aligned to the left.

Please note that this must be accomplished using CSS only.

Incorrect                  |  Correct
:-------------------------:|:-------------------------:
![](images/resize-incorrectly.gif) | ![](images/resize-correctly.gif)

## Part 5: More about Responsive Design (20%)
Finally you are going to replace the video with a still image (````hovedbygget.png````) using media queries. If the visitor is using a mobile device (resolution width lower than ````940px````) the video should be replaced with the image.

## Questions (10%)
1. Why do mobile phones usually ignore auto play on video elements?
2. What will the CSS snippet at the end of this section do if the visitor is browsing on a device with ````320 x 568 ```` resolution?
3. Mention some of the advantages of having a single responsive website instead of dedicated versions like ````m.til.no```` for mobile and ````til.no```` for desktop?

````css
@media only screen
and (min-device-width : 768px)
and (max-device-width : 1024px)  {
  #logo {
    display: none;    
  }
}
````

Deliver the answers as a .txt file together with your other deliverables.

## Deliverables
Note: Include the mp4 video file in your submission. It is not necessary to include all of the video files.

Submission should be uploaded as a zip file into It’s Learning before the deadline. Submissions are ONLY accepted via Its Learning. We DON’T accept late assignments. Emails or any other messages with late assignments are automatically discarded without further communication
