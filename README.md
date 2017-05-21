###**Usage:**

```npm
$ git clone https://github.com/tahaipek/Nodcam.git

$ npm install

$ npm run express-server
(Web server - node index.js)
	
$ npm run streaming-server
(Web Sockets - node stream.js <secretKey>)
	
$ npm run mac
(Streaming camera ffmpeg command => 
ffmpeg -f dshow -i video="<cameraDeviceName>":audio="<audioDeviceName>" <outputName>.mp4 -f mpeg1video http://localhost:<webSocketsStreamingPort>/<secretKey>/<width>/height)
if you don't want to record, remove 'output' keyword.
```

###**Requirements**
  * **NodeJs** https://nodejs.org/
  * **ffmpeg** https://www.ffmpeg.org/

