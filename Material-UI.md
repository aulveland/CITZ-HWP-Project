The HWP project has adopted the use of Material-UI as the UX design framework as identified in the [Architectural Decision Log](https://github.com/bcgov/CITZ-HybridWorkplace/wiki/Architectural-Decision-Log#materialui). Start your journey by understanding the [importance of Material-UI](https://info.keylimeinteractive.com/10-things-you-need-to-know-about-material-design).

## Core Principles:

1) pick & choose your UX concepts - themes, paper & cards and translate into implementation (grid system)
2) usability comes first - make it clean and simple
3) listen to users - solicit feedback, adapt as required
4) adopt BCSans typography

Follow these [material design rules](https://www.uxpin.com/studio/blog/material-design-rules/) and 
[guidelines](https://material.io/design/guidelines-overview)

# Usage Tips
Material UI [MUI]
Updated version MUI5 
Link: https://mui.com/
#### Add to local machine 
To implement it (add) to code:  npm install @mui/material @emotion/react @emotion/styled
-	The above step has already been implemented in our project
# Components Used
### Grid
https://mui.com/components/grid/ 
-	Helps style components in a grid structure. 
-	12 column spaces (each block can have more than 1 space though)
-	Adjust spacing between columns
-	Fluid – scale and resize content  

-	Import statement: import Grid from '@mui/material/Grid';
-	Example: of use  
            < Grid container spacing={2}>  
           &nbsp;     < Grid item xs={7}>  
	&nbsp;	&nbsp; < p> hello < p>  
        &nbsp;        </ Grid>  
        &nbsp;        < Grid item xs={5}>  
        &nbsp;   &nbsp;             < h1> Profile </ h1>  
        &nbsp;        </ Grid>   
</ Grid>    
 ### Container
 https://mui.com/components/container/
-	Wraps code in the center of the webpage 
-	Fluid or fixed.    
  
-	Import statement: import Container from '@mui/material/Container';
-	Example of use:    
&nbsp;< Container>  
&nbsp;  &nbsp;  < Routes />  
&nbsp;    	< /Container>  
Basically, wrap entire App.js block in a container (as an option)


### Paper
 https://mui.com/components/paper/
-	Paper like sheet
-	Bind pages together, resize 
-	Multiple sheets
-	Basically, acts like a piece of paper  

-	Import statement: import Paper from '@mui/material/Paper';
-	Example of use: 
&nbsp; < Paper>  
&nbsp; &nbsp;    < h3> Title < h3>  
&nbsp; &nbsp;	 < p> Hello world </ p>   
&nbsp; </Paper>  
### Card 
 https://mui.com/components/cards/ 
-	Similar functionality as paper
-	Contain content on single topic 
-	Display a hierarchy     
  
-	Import Statement: import Card from '@mui/material/Card';
-	Example of use:   
&nbsp; < Card>  
&nbsp; &nbsp; < CardActionArea>  
&nbsp; &nbsp; &nbsp; …  
&nbsp; &nbsp; &nbsp; < CardContent>  
&nbsp; &nbsp; &nbsp; < p> Yo </ p>  
&nbsp; &nbsp; &nbsp; </ CardContent>  
&nbsp; &nbsp;  </ CardActionArea>  
&nbsp; </ Card>   
-	This example also includes imports from CardActionAria, CardContent all from MUI

### Typography
https://mui.com/components/typography/ 
- make fonts and sizes easy to apply
- customize text for your own application  
  
- below is an example of the government typography class that contains BS sans font  
  
include /app/client/src/topography.js file

/*  
&nbsp;  Typography  
&nbsp;  @author Jason C. Leach from [platform-service-registry](https://github.com/bcgov/platform-services-registry)  
*/  
  
import '@bcgov/bc-sans/css/BCSans.css';  
import Typography from 'typography';  
  
const typography = new Typography({  
&nbsp;  baseFontSize: '16px',  
&nbsp;  baseLineHeight: 1.25,  
&nbsp;  headerFontFamily: ['BCSans', 'Noto Sans', 'Verdana', 'Arial', 'sans-serif'],  
&nbsp;  bodyFontFamily: ['BCSans', 'Noto Sans', 'Verdana', 'Arial', 'sans-serif'],  
&nbsp;  scaleRatio: 2.074,  
});  
  
typography.injectStyles();  
export default typography; 

### Button
https://mui.com/components/buttons/ 
- simple user actions
- three variants; text, contained, outlined
- can have onClick actions for handling actions when the button is pressed

- import statement: import Button from '@mui/material/Button';
- Example of use:  
 &nbsp; < Button variant="outlined">Primary</ Button>


### Custom Color 
https://mui.com/customization/color/
- use colours by materialUI in mui components
- choose shading and color scheme
- import the main theme colour in then can use any shade in that colour
- set primary and secondary colours with theme option 

- example in code (including theme)    
import { createTheme } from '@mui/material/styles';  
import { purple } from '@mui/material/colors';  

 const theme = createTheme({  
 &nbsp;  palette: {  
  &nbsp; &nbsp;   primary: {  
&nbsp; &nbsp; &nbsp;       main: purple[500],  
 &nbsp; &nbsp;    },  
 &nbsp; &nbsp;    secondary: {  
 &nbsp; &nbsp; &nbsp;      main: '#f44336',  
 &nbsp; &nbsp;    },  
&nbsp;   },  
});  

### Box 
https://mui.com/components/box/
- acts like a div component (wrapper)
- can style it using all of mui styles
- use sx prop to specify any CSS rules you want to apply to the box

- import statement: import Box from '@mui/material/Box';  
- Example of use:   
< Box  
 &nbsp;      sx={{  
  &nbsp;       width: 300,  
 &nbsp;        height: 300,  
  &nbsp;       backgroundColor: 'primary.dark',  
  &nbsp;     }}  
    />  
