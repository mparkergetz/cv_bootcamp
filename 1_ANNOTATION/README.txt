### HOW TO ANNOTATE IMGS ###

1. open terminal
	- if miniconda3 is not installed, install
	- if miniconda3 was just installed, create conda env for this program:
		$ conda create -n "labelImg" python=3.8
		$ conda activate labelImg
		$ pip3 install labelImg

2. activate conda environment:
	$ conda activate labelImg

3. start labelImg:
	$ labelImg

4. open dir containing imgs (cv_bootcamp/ANNOTATION/jpgs_to_annot)

5. draw bounding boxes around insects
    - use single label "insect" for all bounding boxes
	- enable 'single class mode': View > Single Class Mode
    - on left toolbar, make sure the annotation type = 'YOLO' (button between 'Save' and "create RectBox') 
    - ctrl + scroll wheel to zoom in on insect for better accuracy
    - hotkeys:
	w - create a rect box
	d - next image
	a - previous image
	del - delete selected rect box

6. Periodically save, confirm annotation txt files are being generated to img dir

7. At the end of your session, move jpgs with annotation txt files to ANNOTATION/completed