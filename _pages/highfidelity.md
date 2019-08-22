---
layout: single
title: High Fidelity VR
permalink: /highfidelity/
author_profile: true
gallery:
  - url: /assets/images/hifi/general/hifiheader.jpg
    image_path: assets/images/hifi/general/hifiheader.jpg
  - url: /assets/images/hifi/general/hifi1.jpg
    image_path: assets/images/hifi/general/hifi1.jpg
  - url: /assets/images/hifi/general/hifi2.jpg
    image_path: assets/images/hifi/general/hifi2.jpg
  - url: /assets/images/hifi/general/conference.jpg
    image_path: assets/images/hifi/general/conference.jpg
---

<p>A collection of my projects while working as an VR Content Developer on the Experiences team at High Fidelity.</p>

<br />

<h2 id="avatar101-hifi">Avatar Customization 101 App</h2>


<h3>Problem</h3>

<p><strong>"How do I customize my avatar?"</strong> - the most common user question</p>


<h3>Design Process</h3>

<p>I worked closely with the Avatar, Engine, and Art Teams to design and implement a simple app to explain texture entities, avatar joint physics, and facial blendshapes.</p>

<p>Because this app is a <strong>hifi app blueprint</strong>, it includes a detailed README to teach users how to integrate these customizations into their own avatar and create their own customization hifi app.</p>

README and source code: [github.com/hifi-content/avatarCustomization101](https://github.com/highfidelity/hifi-content/tree/master/marketplaceItems/avatarCustomization101)

<br />

<h2 id="statuss-indicator-hifi">Status Indicator</h2>

<p>I created a script to notify your availability status and in-world location to your coworkers via a job board to
encourage water-cooler talk.</p>

<p>With a button click or VR controller trigger, change your status to busy to be unreachable.</p>

<h3>Technologies Integrated</h3>

<p>Hifi Javascript API, a MySQL database, Linux server running
Node.js, JavaScript, HTML, and CSS</p>

<br />

<h2 id="vote-app-hifi">Vote App</h2>

<a href="/assets/images/hifi/voteApp/avatarcontest1.jpg" title="Avatar Contest">
  <img src="/assets/images/hifi/voteApp/avatarcontest1.jpg" alt="Avatar contest" style="width: 400px" class="align-center" />
</a> 

<p>I developed a High Fidelity app for desktop and VR users to vote on their favorite visited environments and
avatars. The app was adapted for our events: 
<a href="https://www.youtube.com/watch?v=QhWcI1gswqs">Futvrelands Avatar Contest</a>, 
the Holiday Tree Decorating Contest, and 
<a href="https://www.youtube.com/watch?v=2KmXllrBNHw">Multicon Best Environment and Avatar Contests</a>.</p>

<h3>Requirements</h3>

<ul>
    <li>Update list in real-time</li>
    <li>Made by the non-technical producers</li>
    <li>Can only vote once</li>
    <li>Keep the app loaded until 1 week after the event ends</li>
    <li>Adaptable and scalable for future contests</li>
</ul>

<h3>Solutions</h3>

<ul>
    <li>Utilize Google Sheets for an easy user interface for edits</li>
    <li>Update all apps connecting the Hifi API to Google Scripts API</li>
    <li>Limit users to vote only once on both the hifi side and Google sheets </li>
    <li>Have an unload event triggered via the date UTC time</li>
</ul>

<h3>Technologies Integrated</h3>

<p>Hifi Javascript API, Vue.js, Google
Scripts, Google Sheets, HTML, and CSS</p>

<br />

<h2 id="sit-script-hifi">Sit Script</h2>

<p>The sit script is one of the most downloaded Hifi marketplace items and most popular script used in domains
across High Fidelity. I redesigned, refactored, and optimized the original unusable sit script into a clean UX
experience for desktop and VR modes. I created a lock and unlock mechanism to ensure only one avatar sat in
one seat, improved the stand up conditions for VR mode, added all UI elements, and redesigned avatar
location tracking to increase performance.</p>

README and source code: [github.com/hifi-content/sitScript](https://github.com/highfidelity/hifi-content/tree/master/marketplaceItems/sitPoint)

<br />

<h2 id="griefer-detector-hifi">Griefer Detector or "The Loud App"</h2>

<h3>Problem</h3>

<p>Occasionally loud noises and other sounds from a user's microphone disrupts the event experience.</p>

<h3>Solution</h3>

<p>Discover a way to detect and mitigate users exploiting the platform to disrupt our event experience for other users.</p>

<p>Within one week, we were able to implement an app to pinpoint a user with an open mic or a mic that is louder than most other users for event cases. We successfully mitigated any issues.</p>

<p>Later, I advocated for and designed a Hifi Javascript API call to optimize the performance of this app with the Engine Team. This improvement removed the need for an API call per user present in the domain with packet loss to one single API call and 100% success rate.</p>

README and source code: [github.com/hifi-content/loudApp](https://github.com/highfidelity/hifi-content/tree/master/usefulUtilities/loudApp)

<br />

<a href="/assets/images/hifi/general/sittingonBridge.png" title="Sitting on a bridge">
  <img src="/assets/images/hifi/general/sittingonBridge.png" alt="Sitting on a bridge" style="width: 100%; border-radius: 2%" class="align-center" />
</a> 