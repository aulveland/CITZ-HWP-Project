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

include /app/client/src/topography.js file

/**
 * Typography
 * @author Jason C. Leach from [platform-service-registry](https://github.com/bcgov/platform-services-registry)
 */

import '@bcgov/bc-sans/css/BCSans.css';
import Typography from 'typography';

const typography = new Typography({
  baseFontSize: '16px',
  baseLineHeight: 1.25,
  headerFontFamily: ['BCSans', 'Noto Sans', 'Verdana', 'Arial', 'sans-serif'],
  bodyFontFamily: ['BCSans', 'Noto Sans', 'Verdana', 'Arial', 'sans-serif'],
  scaleRatio: 2.074,
});

typography.injectStyles();
export default typography;