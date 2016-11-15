# IoTHubDemo
Simmulated Device for IoTHub Read/Write Messages Demo

<p>I'm really interested in IoT development and am a full stack developer, so this has been an awesome opportunity to start learning about how to send information to and from a "device" and how to start handling that. I like the idea of eventually creating a UI that communicates with a web service that retrieves and send messages to a hub and then have that hub communicate with my device. So this is the start of me building that up.</p>

<p>I am also doing this through Visual Studio as I am a .Net developer. I'm finding the Arduino IDE, NuGet Packages, and the ease of having it all in one solution great!</p>

<p>The points below will correspond to projects in my solution. I started off with <a href="https://azure.microsoft.com/en-us/documentation/articles/iot-hub-csharp-csharp-getstarted">"Get Started with IoT Hub for .Net"</a> and then incorporated<a href="(https://azure.microsoft.com/en-us/documentation/articles/iot-hub-csharp-csharp-c2d">"How to send cloud-to-device messages with IoT Hub and .Net"</a>. I have also played around with switching from AMQP Protocol to HTTP Protocol. I found it easy to change transport type for sending messages, but retrieving has been difficult (I was working on a network that didn't support AMQP, but it's fine on other networks).</p>

<h3>1. Create Device Identity with IoTHub:</h3>
<p align="center">
  <img src="https://github.com/SandraMuller/IoTHubDemo/blob/master/ScreenShot/IoTHubDashboard.png"/>
</p>
<p>This is part of the dashboard on Azures portal. You can see I have 1 Device linked to this IoTHub named IoTDemoSMuller. The app I used to create the device identity returns a key that you will need to use to identify your device when communicating with the hub.</p>
