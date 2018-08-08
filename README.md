# FormatJobListPosting

## Convert pdf to tiff 
* Allow to segment and pdf file 

convert -density 600 -depth 4 -monochrome -background white -blur '0x2' -shave '0x200' CE.pdf CE.tiff 

## tesseract to recognize text 

tesseract CE.tiff outputbase.txt 

## Take all unessessary spaces from text file 

grep -v -e '^$' outputbase.txt >> final.txt

## Python script to create csv format 
file.py 
