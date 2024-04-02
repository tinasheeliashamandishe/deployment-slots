<h1>Configure Azure Web App Deployement Slots</h1>

<h2>Description</h2>
This lab will Configure Azure deployment slots.<br /><br />
Deployment slots in Azure Web Apps serve several purposes, primarily revolving around facilitating continuous deployment, testing, and seamless updates of web applications.<br />
<b>Here are some key purposes of deployment slots:</b>
<br />
<b>Continuous Deployment:</b> Deployment slots allow you to deploy your application continuously without interrupting the main production site. You can deploy new versions of your application to a staging slot, test it thoroughly, and then swap it with the production slot seamlessly when ready.
<br />
<b>Testing and Staging:</b> Deployment slots provide a separate environment for testing and staging new versions of your application. This allows you to perform various tests, such as functional testing, performance testing, or user acceptance testing, without affecting the live production environment.
<br />
<b>Zero Downtime:</b> By using deployment slots, you can achieve zero downtime deployments. When you swap deployment slots, Azure ensures that the transition is seamless, and there's no interruption in service for your users.
<br />
<b>Rollback:</b> If an issue occurs after deploying a new version to production, you can quickly roll back to the previous version by swapping the slots again. This minimizes the impact of errors or bugs on your users.


<h2>Environments Used </h2>

- <b>Microsoft Azure</b>

<h2>Lab walk-through:</h2>

<p align="center">
<h4>Step 1</h4>
Create a Web App Resource<br/>
<img src="https://i.imgur.com/Wa6gjfY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<h4>Step 2</h4> 
In the App Service editor, edit the deafult page to mark V1 of the App.<br/>
<img src="https://i.imgur.com/H9hu8AB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<br />

<h4>Step 3</h4> 
Create a deployment slot where you will, develop the updated version of your app.<br/>
<img src="https://i.imgur.com/eMFzNZr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<img src="https://i.imgur.com/LLdqHCC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>

<b>When both V1 and V2 have been created. You use Azure to swap the 2 deployemts.</b><br/>

Before the Swap.<br/>
<img src="https://i.imgur.com/2asnS5v.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>

<h4>Step 4</h4> 
Swap the 2 Deployments.<br/>
<img src="https://i.imgur.com/TL8Asdd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>

After the Swap.<br/>
<img src="https://i.imgur.com/g8ousIX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>

<b>The 2 deyployents have successfully been swapped.</b><br/>
