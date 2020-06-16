# IonicDemo Tutorial

HI Guys,

if you want to play a bit with ionic here is an example to get warm with the Ionic Framework, the UI Elements and the Ionic CLI.

First you have to install ionic with npm install `$ -g @ionic/cli`

For this first experience we use one of the pre-made app templates. We will use the tabs App.
With ´$ ionic start myApp tabs` and by following the Instructions of the Ionic CLI the App will be created.

You can run the App with `$ ionic serve`. If you use `$ionic serve --lab` you will see your App like it was on a Smartphone. 

Now you can try out a bit and if you want to you can try to build your first app to look like the one I did in this project. I used Cards, an Alert, some Buttons, some of the ionic Icons and a Date & Time Picker. 


In the [Docs](https://ionicframework.com/docs/components) you can have a look at all the UI Components.


## Here is a short tutorial how I created this app

### 1. Start new App
`$ ionic start` follow the istructions of the Ionic CLI and choose the Tab template 

### 2. Serve the App
`$ cd ./yourApp`
`$ ionic serve`

### 3. Open in your IDE
Choose the IDE you feel most comfortable with - I use VS Code

### 4. Add a new page 
`$ionic generate page tab4`

### 5. First Page 
At the first page I added some Cards to create a beautiful start page.
Here is an example card code 

` <ion-card>
  <img src="./madison.jpg" />
      <ion-card-header>
         <ion-card-subtitle>Destination</ion-card-subtitle>
         <ion-card-title>Madison, WI</ion-card-title>
      </ion-card-header>
      <ion-card-content>
        Founded in 1829 on an isthmus between Lake Monona and Lake Mendota, Madison was named the capital of the Wisconsin Territory in         1836.
      </ion-card-content>
  </ion-card> ` 
  
  You can change the Text and the Pictures if you want to
  
  ### 6. Second Page 
  
 At the Second page I played a bit around with buttons, Checkboxes and Radio Buttons . 
 [Here](https://ionicframework.com/docs/api/button) you can have a look at all the Buttons.
 [Here](https://ionicframework.com/docs/api/checkbox) you have the docs of the checkboxes.
 [Here](https://ionicframework.com/docs/api/radio) you have the docs of the radio buttons.
 
 
### 7. Third Page 

At the third page I added some little datetime picker 

`<ion-app>
    <ion-header translucent>
      <ion-toolbar>
        <ion-title>DateTime</ion-title>
      </ion-toolbar>
    </ion-header>,
    <ion-content fullscreen>
      <ion-list>
        <ion-item>
          <ion-input placeholder="Title"></ion-input>
        </ion-item>
        <ion-item>
          <ion-input placeholder="Location"></ion-input>
        </ion-item>
        <ion-item-divider></ion-item-divider>
        <ion-item>
          <ion-label>Start Date</ion-label>
          <ion-datetime value="1990-02-19" placeholder="Select Date"></ion-datetime>
        </ion-item>
        <ion-item>
          <ion-label>Start Time</ion-label>
          <ion-datetime display-format="h:mm A" picker-format="h:mm A" value="1990-02-19T07:43Z"></ion-datetime>
        </ion-item>
        <ion-item>
          <ion-label>Ends</ion-label>
          <ion-datetime value="1990-02-20" placeholder="Select Date"></ion-datetime>
        </ion-item>
        <ion-item>
          <ion-label>Repeat</ion-label>
          <ion-datetime placeholder="Never" disabled></ion-datetime>
        </ion-item>
        <ion-item>
          <ion-label>Travel Time</ion-label>
          <ion-datetime placeholder="None" disabled></ion-datetime>
        </ion-item>
        <ion-item-divider></ion-item-divider>
        <ion-item>
          <ion-label>Alert</ion-label>
          <ion-datetime placeholder="None" disabled></ion-datetime>
        </ion-item>
      </ion-list>
    </ion-content>`

### 8. fourth page

At the fourth page I just added some Icons i liked. 
[Here](https://ionicons.com/) are all the Ionic Icons you can use.

### 9. Change names in Navbar 

At the last step I changed the names in the Navbar at the bottom.

You have to change the names in the File `tabs.page.html`

