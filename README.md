# Deep_learning_skippy

### Creators:
Sághy Dániel CYFLUV

Markos Péter A09C0D
  
### Subject:
IMG3: Image to text
  
## Milestone I.
We gathered datas from: https://ai.google.com/research/ConceptualCaptions
so we got Train%2FGCC-training2.tsv and Validation%2FGCC-1.1.0-Validation.tsv. (~3.3 million data) We will use our own splitted train-valid-test datas form these tsv files.

In .tsv files we have the text, '\t', and the link of the image.

We used Image_downloader.ipynb to download the images, and write the output.txt with lines, containing the name of the image (simply numbers), '\t', and the text of the image. (We downloaded only ~15.000 images until the Milestone I. Of course, we will need more.)

After that, we feed these datas (output.txt, and the images) with the data_preprocessing.ipynb, to get tfrecords files. Firstly used 0.8-0.1-0.1 train-valid-test datarates, and we set the maximum size of one tfrecords file to 5000. So we get train.txt, valid.txt and test.txt from the output.txt. The tfrecords file generation is still in progress.
