# FEVCNNtk
Finite Element Volumes for Convolutional Neural Networks Tooklkit

## Project Announcement

<em>This project's aim is to create a FOSS toolkit that helps creating
neural net architectures that operate on spacial volumes described
in terms of finite elements livining in a 2-dimensional contractible region
that is mapped to a parameter space of arbitrary (finite) dimension.</em>

### Why?

The power of CNNs for tasks that involve object detection and classification in
rasterized and noisy image data is well-known. Clearly, digital cameras are
prominent sources of rasterized image data with noise. But there is another source
of noisy data stemming from images that does not easily fit into the setting of rasterized
volumes: OCR data. Tools like tesseract take a binarized version of a document containing text
and return an set of detected words together with their bounding boxes. Many relevant documents
in real world settings also convey information through their layout: tables are a popular part
of invoices. It is quite natural that you might want to use CNNs in order to determine
interesting segments of a document and extract data from it. But rasterizing the bounding-box data 
in order to treat it as an image volume is not without problems: just like rasterized images take up
more space than vector-images, rasterizing bounding-boxed data will increase the memory footprint dramatically.
Furthermore, it would be desirable to have one raster point per character in text, yet most fonts
are not monospace and so the character-boxes are hard to fit on a regular grid. Furthermore, documents typically
use a mix of different fonts and font sizes; -- adjusting for this would either require a high resolution
during rasterization, prohibitively increasing the memory footprint.

### What?

We aim to work out the details of using finite-element spacial descriptions in input volumes to
modified convolutional layers in neural nets, as well as to implement a free toolkit that makes
our results easily available to the public.

### Join?

We call out for anyone who wants to participate and contribute to this project to join us by
sending a [mail](mailto:fevcnn@immanuel-albrecht.de).


