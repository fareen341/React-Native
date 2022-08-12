<pre>
Reactive Native:
React Native components are cross platform
FOr all the components follow React Native website

Can be build using 
1)Expo CLI: tool or framework that sits on top of react native and do most of the work easy.
2)React Native CLI

Installing Expo cli:
$ sudo npm i -g expo-cli

Requitrement:
Node version 12 or higher

Creating first project
$ expo init app_name

Running the app:
$ npm start 	-> on browser select the option where we want to run.

Extensions:
React Native Tools
React-Native/React/Redux/Redux snippets for es6/es7
Material Icon Theme: for having themes 

Extra Extensions:
Prettier
Format On Save: use prettier to format the code


To run developer on expo:
Shake the device

To run the chrome extension for debugger:
Open developer mode in phone -> Debug remote js -> when done with debugging stop it cuz it show down the app

Publish:
It can be publish on expo store for testing. It can be downloaded by anyone in the world.
After successfully published it'll be visible on browser with a link

REACT NATIVE COMPONENTS:
View is like div in react native
SafeAreaView: Sometimes upper area of phone covers the part of our app component, to make it inside the app we use SafeAreaView. 

ADDING STYLES:
1)inline style:
&gt;Button style={{ backgroundColor: "orange"}}&gt;Click&lt;Button&gt;

2)Using javascript object(Styles defined below):
One benefit of using this styles is it shows error on the device where as inline style does not
&gt;Button style={styles.container} &gt;Click&lt;Button&gt;

const styles = StyleSheet.create({
	container:{
		backgroundColor: "green",
		flex: 1,
	}
})

3)Refering style:
const contStyle = { backgroundColor: "pink" }
&gt;Button style={contStyle} &gt;Click&lt;Button&gt;

DEFINING MORE THAN ONE STYLE
&gt;Button style={[styles.container, contStyle]} &gt;Click&lt;Button&gt;

Note: style on the left side overwrites the style on the right.

DESIGN ON PLATFORM SPECIFIC
On styles:
Platform : can be use to design platform specific app
paddingTop: Platform.OS === "android" ? 20 : 0

CALCULATE THE HEIGHT OF THE STATUS BAR
paddingTop: Platform.OS === "android" ? StatusBar.currentHeight : 0

cuz height of the status bar is different on different android devices.

NAVBAR
1)STACK
i)install and follow steps given on react-navigation

2)DRAWER
i)follow steps given on:
https://reactnavigation.org/docs/drawer-navigator#installation

use expo for installation and import the line given

If it gives reanimated error then:

Follow steps:
https://docs.expo.dev/versions/latest/sdk/reanimated/#installation

Note:
dont forget to $ expo start --clear
if bable file is not visible then search in vs code

API CALL:
1)Api call does not work on localhost we've to run backendapi on our ip address 
i)on terminal cehck:
	$ ip a
ii)python3 manage.py runserver ip_addr:8000
ii)give this api url in axios request


ADDING ICON IN REACT NATIVE:


Steps to install and usage Ionicons, FontAwesome and Entypo font Icons in react-native.


If react-native does not work then use npm

First you need to install using following command.
$ react-native install react-native-vector-icons

Then Required to Link:
$ react-native link react-native-vector-icons

Import font package files to your page:

import Ionicons from 'react-native-vector-icons/Ionicons';
import FontAwesome from 'react-native-vector-icons/FontAwesome';
import Entypo from 'react-native-vector-icons/Entypo';

Usage Example:
<View>
    <Text>Ionicons Icons</Text>
    <Icon name='md-bicycle' />

    <Text>FontAwesome Icons</Text>
    <FontAwesome name='trophy' />

    <Text>Entypo Icons</Text>
    <Entypo name='aircraft' />
</View>

If you want to see list of available icons, you can look in this directory:

Ionicons:
\node_modules\react-native-vector-icons\glyphmaps\Ionicons.json

FontAwesome:
\node_modules\react-native-vector-icons\glyphmaps\FontAwesome.json

Entypo:
\node_modules\react-native-vector-icons\glyphmaps\Entypo.json 



 REACT JS:
 For building react js app:
$ npm run build

To deploy on github:
1)add project to github

2)In package.json add homepage
  "homepage": "https://fareen341.github.io/online-shop-deploy",

3)add two line in script
  "scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build",
    
4)run the command:
$ npm install gh-pages --save-dev

5)run:
$ npm run deploy

 
</pre>
