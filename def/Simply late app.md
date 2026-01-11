# Directory structure

Files in the folder are html pages saved by Chrome/Brave browser from my Godaddy online web builder tool one by one. 
Alway a pair of html and directory starting with the same name. 
The directories will probably contain same code. 
The main page is src.html and src_file directory. Consider this page as the main page. 

Images are in img directory. 
They were not downloaded from the web, so paths won’t match. 

# Image structure on the main page


Order of images on the main page is the following:
1. hero.png = biggest title image on top of the main page
2. features/ directory contains 4 images showing different features 
	1. shown in the vertically scrollable image slider
3. explanation/ directory contains 2 images 
	1. shown next to each other spanning full width of the page
4. flavors/ directory contains 2. & 3. images bellow under the text "Three flavors". The 1. image is features/simply-all-0006.png 
	1. Images are cropped to fit the dedicated html area. 1. image is cropped differently. 
5. AOD web Copy.png = image to the left of "Up to 30 days of battery life" headline
6. photo.jpg = photo of the product 

# Framework images come from


The code of the Godaddy framework these html files are from uses a responsive web layout and lazy-loading. 

# Desired html concept

1. Responsive design that shows correctly on all devices with all sizes in proportions of the source layout. 
2. Clean code. Do not use code or html of the source files, but create a new, cleaner code that shows the same, but is a simple static readable html instead of that cryptic framework html. 
3. Keep dimensions of images in the layout. Zoom out the original files to fit them at the place. 


# Your goal

Create a new html page that looks the same as the main page in the new clean static code of html, js and css that is cleaner than the provided files saved from the Godaddy framework.
## Initial page main.html

1. Analyze layout of the main page: 
	1. hierarchy of headlines, text, columns and images. 
	2. proportions, dimensions and responsive breakpoints 
	3. make sure you include all text, headlines and images in exactly same visual layout
	4. ensure the same design for the components, text and headlines sizes, columns and image components proportions
	5. summarize it to the file layout.md
2. Analyze src_file javascript codes and css and inline codes and css: 
	1. summarize key principles into file named code_principles.md
3. Create the new main.html page and main.css that follow the layout of the source page you analyzed above in the same layout and principles you analyzed before. Replace images by images under the headline of "Image structure on the main page". Ensure all images, text and headlines are shown in the same layout as the original page. 
4. Review the current style of the page and replace layout.md with the styles we finalized here together so it reflects the current page and we can apply it for the new one while reusing the styles and principles. 

### Deploy

1. **Make folder dev/** and copy files of the current page and styles including images into it. Consider this folder an app ready to be deployed. 


## Other pages task

1. Analyze layout of the source page. 
	1. hierarchy of headlines, text, columns and images. 
	2. proportions, dimensions and responsive breakpoints 
	3. make sure you include all text, headlines and images in exactly same visual layout
	4. ensure the same design for the components, text and headlines sizes, columns and image components proportions
	5. summarize it to the file layout-page.md
2. Review the style of the pages we created and remember styles you added so you can reuse them when possible. 
3. Review code_principles.md and layout-page.md to so we can create a refactored page in the next step. 
4. Create the new page in dev/ folder that follow the layout of the source page you analyzed above in the same layout and principles you analyzed before and contains all content of the source page in the same order. 
	1. Do not update the current file, but recreate it from scratch by these principles we’ve done together. 
	2. Start with the content of the source page and gradually add it to the new page to ensure you won’t change direction of the text or forget some test. 
	3. Reuse styles when possible and the styles are similar. Add new styles for elements that differ. Use layout-page.md and code_principles.md as a guidance. 
	4. Make sure again that all text of the source page is also in the new page.

### Final pages

1. privacy.html
2. ToS.html
3. garmin-compatibility.html

While reusing existing styles, create the first privacy.html. 


## New styles

### Settings


1. 3 column layout that gradually decreases the number of columns to 2 and 1 on narrower screens
2. Image browser at the top that contrary to the image slider shows only one image at time fully and dims the other and have arrows to navigate to the next and previous image. 


## Corrections

### Calendar

1. Update images in the page so they match same images in img/ folder. When unsure, ask about any image you can’t find there. 
	1. If you can not find the first image, change it to settings/guidance/explanation-0004.png

### Settings

1. Update the style of the image slider, so it shows all images at once in the horizontal image slider, but the other files than the current are dimmed to 50 %. 
2. The image slider spans full width. 
3. Ensure arrows to go back and forth are big on the sides of the screen. 
4. Disable buttons from cycling around from back to start and vice versa.
5. When user scrolls by mouse, highlight the image that is at the center of the destination he scrolled to. When the scrolled area is at the very end or start, the first or last image is highlighted. 

