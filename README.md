# IoTHubDemo
<h2>Simmulated Device for IoTHub Read/Write Messages Demo</h2>

<p>I'm really interested in IoT development and am a full stack developer, so this has been an awesome opportunity to start learning about how to send information to and from a "device" and how to handling that. I like the idea of eventually creating a UI that communicates with a web service to retrieve and send messages to a hub and then have that hub communicate with my device. This is the start of me building that up.</p>

<p>I am also doing this through Visual Studio as I am a .Net developer. I'm finding the Arduino IDE, Azure NuGet Packages, and the ease of having it all in one solution great!</p>

<p>The points below will correspond to projects in my solution. I started off with <a href="https://azure.microsoft.com/en-us/documentation/articles/iot-hub-csharp-csharp-getstarted">"Get Started with IoT Hub for .Net"</a> and then incorporated <a href="https://azure.microsoft.com/en-us/documentation/articles/iot-hub-csharp-csharp-c2d">"How to send cloud-to-device messages with IoT Hub and .Net"</a>. I have also played around with switching from AMQP to HTTP. I found it easy to change transport type for sending messages, but retrieving has been difficult (I was working on a network that didn't support AMQP, but it's fine on other networks).</p>

<h3>1. Create Device Identity with IoTHub:</h3>
<p align="center">
  <img src="https://github.com/SandraMuller/IoTHubDemo/blob/master/ScreenShot/IoTHubDashboard.png"/>
</p>
<p>This is part of the dashboard on Azures portal. You can see I have 1 Device registred with my IoT Hub - IoTDemoSMuller. The app I wrote is used to create a device identity in the hub's identity registry and returns a key that you will need to use to identify your device when communicating with the hub.</p>

<h3>2. Read Device to Cloud Messages:</h3>
<p align="center">
  <img src="https://github.com/SandraMuller/IoTHubDemo/blob/master/ScreenShot/ReadMessages.png"/>
</p>
<p>Above is a screen shot of my console app reading the messages from my IoT Hub that were sent from my simulated device. There is a lot more to be learnt around this with regards to how to process device-to-cloud messages at scale, but for the purpose of this project, this simple app is sufficient.</p>
