# Campaign Builder

Email template framework which allows for the segregation of content management & config from html editing and build by using json data source file

## ABOUT
Runs sequence of tasks to generate template: 
- Data compilation of campaign and config data;
- Compile sass —> css
- Compile template and inject content
- inject inline CSS 
- inject CSS resets  & media Queries
- Generate readable and minified html  templates to dist folder

## REQUIREMENTS
Requires gulp-cli installed globally:
`npm install --global gulp-cli`

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
Outputs a standard and minified html template file in the 'dist' folder

## OUTPUT LOCATION
`dist/`

## TROUBLESHOOTING
If build throws the following error: 
Error: Node Sass does not yet support your current environment:

Then try:
`npm rebuild node-sass`


## CLEAR FOLDERS 
Command: `gulp clear`
