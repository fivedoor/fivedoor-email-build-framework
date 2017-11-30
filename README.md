# fivedoor-email-build-framework


BUILD CHAIN
--------------------------------------------------
gulp build
runSequence('folders:clean', 'data', 'sass', 'template', callback);

TEMPLATE CHAIN
--------------------------------------------------
gulp template
runSequence('template:comp', 'links:inject', 'css:inline','css:inject', 'html:tidy', 'html:min', 'watch', callback);

 CLEAR CHAIN
--------------------------------------------------
gulp clear
runSequence('folders:clean','data_src:clean', callback);

DATA CHAIN BASIC
--------------------------------------------------
gulp data
runSequence('data:comp', callback);


COMPILE DATA 
--------------------------------------------------
Merge config json and campaign json
gulp data:comp

COMPILE SASS
--------------------------------------------------
gulp sass 

CREATE TEMPLATE
--------------------------------------------------
template:comp

INJECT LINKS
--------------------------------------------------
links:inject

INLINE CSS
--------------------------------------------------
css:inline

INJECT CSS RESETS & MEDIA QUERIES
--------------------------------------------------
css:inject

TIDY HTML
--------------------------------------------------
html:tidy

MINIFY HTML & CSS
--------------------------------------------------
html:min
