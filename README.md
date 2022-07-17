# Duplicate_filter
## Algorithm Introduction
This code is used to eliminate duplicate data in the IGCT database using computer vision. The input of this algorithm is a list of video clips that are processed by IGCT tool. The output is the number of distinct tresspassers (vechile or person) in that video clip. Here is an example:

Input: 
"https://igct.s3.amazonaws.com/5fee675583dbb051a5aa4b16_1626185723.mp4"

Output:

Total number of objects:  3

image name: A_1.jpg  trajectory:  [(457, 293), (457, 293), (457, 293), (443, 294), (438, 294), (436, 294), (436, 294), (436, 294), (436, 295), (436, 295), (416, 292), (409, 290), (407, 290), (405, 291), (406, 291), (406, 291), (405, 291), (406, 291), (406, 291), (406, 291), (397, 289), (393, 287), (392, 287), (392, 287), (392, 287), (392, 287), (371, 285), (364, 284), (360, 284), (359, 284), (359, 284), (359, 284), (346, 283), (343, 282), (341, 282), (340, 282), (340, 283), (340, 283), (334, 280), (332, 279), (331, 279), (332, 278), (332, 278)] Appearance:  0-42 label: car

image name: A_2.jpg  trajectory:  [(236, 262), (236, 262), (236, 262), (236, 262), (246, 264), (250, 265), (250, 264), (251, 265), (251, 265), (251, 265), (251, 265), (261, 266), (265, 267), (266, 267), (267, 267), (267, 267), (267, 266), (267, 266), (267, 266), (279, 267), (285, 267), (286, 268), (287, 268), (287, 268), (287, 268), (286, 268), (305, 270), (313, 270), (315, 270), (317, 270), (317, 271), (316, 271), (316, 271), (328, 273), (333, 274), (334, 275), (335, 275), (334, 275), (334, 275), (377, 277), (392, 276)] Appearance:  65-105 label: truck

image name: A_3.jpg  trajectory:  [(398, 277), (400, 277), (400, 276), (401, 276), (396, 276), (394, 277), (393, 276), (392, 276), (393, 276), (392, 276), (393, 276), (400, 277), (403, 276), (404, 276), (404, 276), (404, 276), (405, 276), (404, 276), (404, 276), (404, 276)] Appearance:  106-125 label: truck

## Required dependencies:

pip install textdistance

sudo apt-get update

sudo apt-get install tesseract-ocr

sudo apt-get install libtesseract-dev

pip install pytesseract
