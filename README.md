# Business Card Maker using React

App that allows you to make a business card.

Demo Link → https://minji-card-maker.netlify.app/

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

<img width="90%" alt="demo_gif" src="/public/images/readme/card_demo.gif">

### 🔐 Login Page

<img width="90%" alt="login_gif" src="/public/images/readme/login.gif">

- Can login with Google or Github.
- The credential will be saved in firebase, so the user will be automatically logged in when returned.

<img width="90%" alt="login_saved_gif" src="/public/images/readme/login_saved.gif">

- The information on the cards will be saved in firebase even after logout. The user can return for the saved information.

### 📝 Maker Page

<img width="90%" alt="maker_add_gif" src="/public/images/readme/maker_add.gif">

- A user can create a business card on the <em>Card Preview</em> side by entering information on the <em>Card Maker</em> side and upload a image.

<img width="90%" alt="maker_edit_gif" src="/public/images/readme/maker_edit.gif">

- When the information is edited on the <em>Card Maker</em> side, it will be reflected on the <em>Card Preview</em> side at the same moment.

<img width="90%" alt="maker_delete_gif" src="/public/images/readme/maker_delete.gif">

- The cards can be added or deleted.

## 3. Structure

Demo Link → https://minji-card-maker.netlify.app/

### Overall

<div>
<img width="100%" alt="card_structure" src="/public/images/readme/card_structure.png">
</div>

1. When the login button is clicked, the login function is processed.
2. The login gets operated through Firebase, such as verification.
3. React Router sends the user to <em>Maker</em> page.
4. (Step 4-6) If the user is a returning user, the user's database will be called back from Firebase & the image from Cloudinary.
5. (Step 7) The data will be shown in the <em>Editor</em> and <em>Preview</em> section.
6. (Step 8) When the user makes changes on the <em>Maker</em> page, the data will be updated in Firebase and Cloudinary in realtime.

## 4. Improvements

One of the improvements I am planning to update is the performance improvements using memo() and useCallback() function to fix unnecessary components rendering, such as header, footer, buttons, and etc.

## 5. Acknowledgements

- Dream Coding
