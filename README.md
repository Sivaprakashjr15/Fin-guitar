<h1 >
  Finguitar 🎸
</h1>

This web-app is called Finguitar (Finger-Guitar).  
It uses Computer Vision to build an online instrument which you can play using <strong><em>just your fingers</em></strong>. <br>
You can hold up a gesture with your hand and the web-app will record it using your webcam and play a music note for every gesture!
The idea is to then give the user the ability to combine these gestures to make a tune out of it.
So, it's like playing a guitar... but using Computer Vision!<br>
Currently we recognize <i>10 gestures</i> to play different sounds:
      <ul>
        <li>Palm</li>
        <li>Fist</li>
        <li>Thumb</li>
        <li>Index</li>
        <li>Middle 2 fingers</li>
        <li>Pinky</li>
        <li>Call</li>
        <li>Rock</li>
        <li>LShape(finger+thumb)</li>
        <li>Ok</li>
      </ul>

## 🤖Tech-Stack

#### Front-end
- ReactJS

#### Back-end
- Flask

#### Computer vision
- OpenCV

## 📲Communication b/w the web-app and the model
The communication is carried out on a <strong>WebSocket</strong> endpoint run by the server. The web-app uses the browser's Stream API to emit the current frame encoded as a base64 string via the WebSocket. The server receives the string, decodes it and runs the OpenCV model on it. The gesture recognized is then relayed back on the same endpoint as a response.
<br>


## 🔮Further additions
- Host the web-app and the model
- Improve the animations on the web-app
- Add a gamified experience for the user, and provide him with a score as a feedback
- Add a tutorial run, where the user can first train on the set of gestures and get familiar with the sounds.

