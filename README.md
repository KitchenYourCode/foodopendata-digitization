# foodopendata-digitization
Automated extraction of data from food labels pictures

## Scope and process
- INPUT: food label picture
- PROCESS: identify the textual data areas from the picture
  - AI semantic segmentation problem here, ingredients and nutrition facts datasets exists for machine learning:
    - https://www.crowdai.org/challenges/openfood-nutrition-table-challenge#resources
    - https://www.crowdai.org/challenges/openfood-ingredients-list-challenge#resources
- PROCESS: clean the cropped data area of the picture to make them OCRable (rotation, brightness/contrast, ...)
- PROCESS: OCR and parse the text stream
- OUTPUT: structured data, that should ideally be storable

## Legacy resources
- This guy made a prototype for OCRing text on an image with noise
  http://francescopochetti.com/text-recognition-natural-scenes/#second
- A ridiculously basic OCR prototype (might not be always accessible, this is a dev server)
  http://mien.ch:5555/fod/
