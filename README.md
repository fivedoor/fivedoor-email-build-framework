# fivedoor-email-build-framework

Email template framework which allows for separation of content management & editing from html templating & configuration using json data source file

## ABOUT
Runs sequence of tasks to generate template: 
- Data compilation of campaign and config data;
- Compile sass —> css
- Compile template and inject content
- inject inline CSS 
- inject CSS resets  & media Queries
- Generate readable and minified html  templates to dist folder

## SET UP
Download repository and run `npm install ` in the directory

## INPUT
Requires json campaign form data file as can be generated by campaign supernova app:
https://github.com/fivedoor/campaign-supernova

## INPUT LOCATION
Just add the json campaign file to the campaign folder: 
`src/data/campaign`

## RUN
Command:  `gulp build`

## OUTPUT
Outputs a standard and minified html template file in the list folder

## OUTPUT LOCATION
`dist/`


## CLEAR FOLDERS 
Command: `gulp clear`
