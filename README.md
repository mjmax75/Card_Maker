# Business Card Maker using React

App that allows you to make a business card.

Demo Link → https://minji-youtube-mini-clone.netlify.app/

## 🗂 Table of Contents

1. [Tech Stack](#1-tech-stack)
2. [About this Project](#2-about-this-project)
3. [Structure](#3-structure)
4. [Improvements](#4-improvements)
5. [Acknowledgements](#5-acknowledgements)

## 1. Tech Stack

<img alt="JavaScript" src="https://img.shields.io/badge/javascript%20-%23323330.svg?&style=for-the-badge&logo=javascript&logoColor=%23F7DF1E"/> <img alt="CSS3" src="https://img.shields.io/badge/css3%20-%231572B6.svg?&style=for-the-badge&logo=css3&logoColor=white"/> <img alt="HTML5" src="https://img.shields.io/badge/html5%20-%23E34F26.svg?&style=for-the-badge&logo=html5&logoColor=white"/> <img alt="React" src="https://img.shields.io/badge/react%20-%2320232a.svg?&style=for-the-badge&logo=react&logoColor=%2361DAFB"/> <img alt="React Router" src ="https://img.shields.io/badge/react router-CA4245.svg?&style=for-the-badge&logo=reactrouter&logoColor=white"/> <img alt="Firebase" src ="https://img.shields.io/badge/Firebase-FFCA28.svg?&style=for-the-badge&logo=firebase&logoColor=white"/> <img alt="Cloudinary" src ="https://img.shields.io/badge/Cloudinary-3448c5.svg?&style=for-the-badge&logo=cloudinary&logoColor=white"/> <img alt="Netlify" src ="https://img.shields.io/badge/Netlify-00c7b7.svg?&style=for-the-badge&logo=netlify&logoColor=white"/>

## 2. About this Project

This is a business card maker project, which has the following features.

1. The login page allows users to sign in using either Google account or Github account
2. The maker page allows users to add/modify/delete information on cards
3. The maker page allows users to add/delete image on the card using cloudinary
4. The modification will be reflected in real time basis using Firebase
5. The modification will be saved even though user logs out

<img width="90%" alt="demo_gif" src="/public/images/readme/youtube_demo.gif">

### 🏠 Default Page

<div>
<img width="45%" alt="default_large_screen" src="/public/images/readme/default_mac.png"> 
<img width="45%" alt="default_mid_size_screen" src="/public/images/readme/default_mac_smaller.png">
</div>

<div>
<img width="45%" alt="default_ipad_screen" src="/public/images/readme/default_ipad.png"> 
<img width="45%" alt="default_small_screen" src="/public/images/readme/default_small.png">
</div>

- Receive data from the YouTube API using Postman to display the channel thumbnail, title, channel name, uploaded date of the most popular video as of today
- The number of videos displayed gets adjusted according to the screen size - Responsive design.

### 🔎 Search Page

<div>
<img width="45%" alt="search_mac" src="/public/images/readme/search_mac.png"> 
<img width="45%" alt="search_smaller" src="/public/images/readme/search_smaller.png">
</div>

- When the user types in keywords in the search bar, the application will display the corresponding videos using YouTube API.

### 📼 Play Video Page

<div>
<img width="45%" alt="play_mac" src="/public/images/readme/play_mac.png"> 
<img width="45%" alt="play_smaller" src="/public/images/readme/play_smaller.png">
</div>

- When the user clicks a thumbnail on the searched list, the page will display the video and the metadata that corresponds the videoid.

## 3. Structure

Demo Link → https://minji-youtube-mini-clone.netlify.app/

### 🏠 Default page - Most popular videos

<div>
<img width="100%" alt="default_structure" src="/public/images/readme/default_structure.png">
</div>

1. When the <em>App</em> component gets mounted, it will get the most popular videos using YouTube API stored in <em>youtube.js</em> and <em>.env</em>.
2. The <em>App</em> component will send props to <em>video list</em> and <em>video item</em> component (including number 3).
3. It will render the <em>video items</em> component in <em>video list</em> component.

### 🔎 Search Page

<div>
<img width="100%" alt="keyword_structure" src="/public/images/readme/keyword_structure.png">
</div>

1. The <em>App</em> component receives the keyword When the user types the keyword in the search input bar.
2. The <em>App</em> state gets changed.
3. Using the class function in <em>youtube.js</em>, it will get the corresponding videos.
4. It will update the <em>video list</em> component.
5. Then, it will render the <em>video item</em> component.

### 📼 Play Video Page

<div>
<img width="100%" alt="play_structure" src="/public/images/readme/play_structure.png">
</div>

1. The user clicks one of the video item.
2. The <em>App</em> component's state gets changed.
3. Using the class function in <em>youtube.js</em>, it will get the corresponding video url.
4. It will update the <em>play video</em> component.
5. Then, it will render the video

## 4. Improvements

Some of the features I would like to work on in the future are 1) infinite scroll function on the default page 2) channel label image on the side of channel title and uploaded date 3) the comments/ number of likes and dislikes/ number of subscribers 4) light and dark mode 5) the loading spinner and much more!

## 5. Acknowledgements

- YouTube Data API
- Dream Coding
