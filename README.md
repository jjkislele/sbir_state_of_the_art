# Sketch-based Image Retrieval Algorithm

Collection of subarasii and reproducible SBIR works.

Criteria: works must have codes available, and the reproducible results demonstrate state-of-the-art.

This collection is inspired by [the image denoising collection](https://github.com/wenbihan/reproducible-image-denoising-state-of-the-art). It makes me have an idea, why don't I summarize the SBIR works just like he did. 

# Feature descriptor
## Global

## Local

# Deep Learning
## Fine Grain


# Benchmark and Dataset
- Flickr15K ~~[[Web]](http://personal.ee.surrey.ac.uk/Personal/R.Hu) [[Image(source and groundtruth)]](http://personal.ee.surrey.ac.uk/Personal/R.Hu/index_files/images.zip) [[Image(resized)]](http://personal.ee.surrey.ac.uk/Personal/R.Hu/index_files/resize_img.zip) [[Sketch]](http://personal.ee.surrey.ac.uk/Personal/R.Hu/330sketches.zip)~~ [[Image(source and groundtruth)]](https://drive.google.com/open?id=13AFiwNh4FMks_jGfL4UDntMf0lHL6BTQ) [[Image(resized)]](https://drive.google.com/open?id=1PqzIO-OWTeEAl3Hs5tRavRs6-qZ8OmXb) [[Sketch]](https://drive.google.com/open?id=16SOyCbC1H6HYJ2uT9ECDRRMj70_zbvmb) [[groundtruth]](https://drive.google.com/open?id=14GEGBW9QgAqAC9_Jh6A5XMeTLWVE9xY2) [[PDF]](http://personal.ee.surrey.ac.uk/Personal/J.Collomosse/pubs/Hu-CVIU-2013.pdf)
	- A Performance Evaluation of Gradient Field HOG Descriptor for Sketch Based Image Retrieval (CVIU 2013), R Hu et al.
	- 14,660 images labelled into 33 categories based on shape only
	- 10 non-expert sketchers(5 males, 5 females)
	- 330 free-hand sketches
- TU-Berlin [[Web]](http://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/) [[Sketch]](http://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/sketches_png.zip) [[PDF]](http://cybertron.cg.tu-berlin.de/eitz/pdf/2012_siggraph_classifysketch.pdf)
	- How Do Humans Sketch Objects? (Siggraph 2012), Eitz M et al.
	- 20,000 unique sketches evenly distributed over 250 object categories
	- **sketch only**
- Image100k [[Web]](http://cybertron.cg.tu-berlin.de/eitz/tvcg_benchmark/) [[Image]](http://cybertron.cg.tu-berlin.de/eitz/tvcg_benchmark/imagedb_100k.tar) [[Benchmark/Sketch]](http://cybertron.cg.tu-berlin.de/eitz/tvcg_benchmark/benchmark.zip) [[PDF]](http://cybertron.cg.tu-berlin.de/eitz/pdf/2010_tvcg_prelim.pdf)
	- Sketch-Based Image Retrieval: Benchmark and Bag-of-Features Descriptors (IEEE T VIS COMPUT GR 2012), Eitz M et al.
	- [Benchmark] has 1,240 images labelled into 31 categories and 31 corresponding sketches for testing
	- [Image] has 101,240 images for training
	- 28 participants(23 males, 5 females)