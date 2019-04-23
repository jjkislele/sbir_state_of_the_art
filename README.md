# Sketch-based Image Retrieval Algorithm

Collection of subarasii and reproducible SBIR works.

Criteria: works must have codes available, and the reproducible results demonstrate state-of-the-art.

This collection is inspired by [the image denoising collection](https://github.com/wenbihan/reproducible-image-denoising-state-of-the-art). It makes me have an idea, why don't I summarize the SBIR works just like he did. 

# Feature descriptor
## Global
- GF-HoG ~~[[Web]](http://personal.ee.surrey.ac.uk/Personal/R.Hu/SBIR.html)~~ [[Web]](http://stuartjames.info/gradient-field-hog.aspx) [[Code]](http://stuartjames.info/SharedFiles/Download.aspx?pageid=105&mid=234&fileid=28) [[PDF]](http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=5649331&isnumber=5648792)
	- Gradient field descriptor for sketch based retrieval and localization (ICIP, 2010), Rui Hu et al.
	- A Bag-of-Regions Approach to Sketch Based Image Retrieval (ICIP, 2011), Rui Hu et al.
	- A Performance Evaluation of Gradient Field HOG Descriptor for Sketch Based Image Retrieval (COMPUT VIS IMAGE UND, 2013), Rui Hu et al.
- Color GF-HoG [[Web]](https://github.com/TuBui/color-GFHoG) [[Code]](https://github.com/TuBui/color-GFHoG)  [[PDF]](http://openaccess.thecvf.com/content_iccv_2015_workshops/w27/papers/Bui_Scalable_Sketch-Based_Image_ICCV_2015_paper.pdf)
	- Scalable Sketch-based Image Retrieval using Color Gradient Features (ICIP, 2015), Tu Bui et al.
## Local
- SHOG [[Code(msvs)]](https://github.com/jjkislele/imdb_framework_msvs) [[Code(origin)]](https://github.com/mathiaseitz/imdb_framework)
    - Sketch-based image retrieval: Benchmark and bag-of-features descriptors (IEEE T VIS COMPUT GR， 2011), Eitz M et al.
    - A descriptor for large scale image retrieval based on sketched feature lines (SBM, 2009), Eitz M et al.
    - How do humans sketch objects? (TOG, 2012), Eitz M et al.

# Deep Learning
## Modelling
- Triplet loss CNN
	- Compact Descriptors for Sketch-based Image Retrieval using a Triplet loss Convolutional Neural Network (CVIU 2017), Tu Bui et al. [[Web]](http://www.cvssp.org/data/Flickr25K/CVIU16.html) [[Code(Caffe)]](https://github.com/TuBui/Triplet_Loss_SBIR) [[Code(Pytorch)]](https://github.com/jjkislele/SketchTriplet) [[PDF]](http://www.cvssp.org/data/Flickr25K/CVIU16_files/CVIU16_published.pdf)
    - Sketch Me That Shoe[^1] (CVPR, 2016), Yu Q et al. [[Web]](http://www.eecs.qmul.ac.uk/~qian/Project_cvpr16.html) [[Code(Caffe)]](https://github.com/seuliufeng/DeepSBIR) [[Code(Tensorflow)]](https://github.com/yuchuochuo1023/Deep_SBIR_tf/tree/master) [[PDF]](http://www.eecs.qmul.ac.uk/~qian/Qian's%20Materials/paper/SketchMeThatShoe_cvpr2016.pdf) [[Dataset]](http://www.eecs.qmul.ac.uk/~qian/Qian's%20Materials/ShoeV2.zip) 
    - Deep Spatial-Semantic Attention for Fine-grained Sketch-based Image Retrieval[^1] (ICCV, 2017) Song J et al. [[Web]](http://www.eecs.qmul.ac.uk/~js327/Project_pages/Project_iccv2017.html) [[Code(Tensorflow)]](https://github.com/yuchuochuo1023/Deep_SBIR_tf/tree/master) [[PDF]](http://www.eecs.qmul.ac.uk/~qian/Qian's%20Materials/paper/SketchMeThatShoe_cvpr2016.pdf) [[Dataset]](https://drive.google.com/open?id=0BwXZSv_g6pw3ejZCTHI4NTZxUFU)

- DPM
    - Fine-grained sketch-based image retrieval by matching DPM[^1] (unpublished) Yi L et al. [[Web]](https://qmro.qmul.ac.uk/xmlui/handle/123456789/6440) [[Code(Matlab)]](https://github.com/panly099/fine-graind-SBIR) [[PDF]](https://qmro.qmul.ac.uk/xmlui/bitstream/handle/123456789/6440/GONGFine-grained2014.pdf?sequence=2&isAllowed=y)

[^1]: Fine-grained retrieval

## Hash Coding
- Deep Sketch Hashing


# Benchmark and Dataset
- Flickr15K ~~[[Web]](http://personal.ee.surrey.ac.uk/Personal/R.Hu/SBIR.html) [[Image(source and groundtruth)]](http://personal.ee.surrey.ac.uk/Personal/R.Hu/index_files/images.zip) [[Image(resized)]](http://personal.ee.surrey.ac.uk/Personal/R.Hu/index_files/resize_img.zip) [[Sketch]](http://personal.ee.surrey.ac.uk/Personal/R.Hu/330sketches.zip)~~ [[Image(source and groundtruth)]](https://drive.google.com/open?id=13AFiwNh4FMks_jGfL4UDntMf0lHL6BTQ) [[Image(resized)]](https://drive.google.com/open?id=1PqzIO-OWTeEAl3Hs5tRavRs6-qZ8OmXb) [[Sketch]](https://drive.google.com/open?id=16SOyCbC1H6HYJ2uT9ECDRRMj70_zbvmb) [[groundtruth]](https://drive.google.com/open?id=14GEGBW9QgAqAC9_Jh6A5XMeTLWVE9xY2) [[PDF]](http://personal.ee.surrey.ac.uk/Personal/J.Collomosse/pubs/Hu-CVIU-2013.pdf)
	- A Performance Evaluation of Gradient Field HOG Descriptor for Sketch Based Image Retrieval (CVIU 2013), Rui Hu et al.
	- 14,660 images labelled into 33 categories based on shape only
	- 10 non-expert sketchers(5 males, 5 females)
	- 330 free-hand sketches
- Flickr25K [[Web]](http://www.cvssp.org/data/Flickr25K/CVIU16.html) [[Image]](http://www.cvssp.org/data/Flickr25K/Flickr25K.zip) [[PDF]](http://www.cvssp.org/data/Flickr25K/CVIU16_files/CVIU16_published.pdf)
	- Compact Descriptors for Sketch-based Image Retrieval using a Triplet loss Convolutional Neural Network (CVIU 2017), Tu Bui et al.
	- 25,000 images labelled into 250 categories
	- **images only**
	- can be used associated with TU-Berlin, shown as follows
- TU-Berlin [[Web]](http://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/) [[Sketch]](http://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/sketches_png.zip) [[PDF]](http://cybertron.cg.tu-berlin.de/eitz/pdf/2012_siggraph_classifysketch.pdf)
	- How Do Humans Sketch Objects? (Siggraph 2012), Eitz M et al.
	- 20,000 unique sketches evenly distributed over 250 object categories
	- **sketch only**
- Image100k [[Web]](http://cybertron.cg.tu-berlin.de/eitz/tvcg_benchmark/) [[Image]](http://cybertron.cg.tu-berlin.de/eitz/tvcg_benchmark/imagedb_100k.tar) [[Benchmark/Sketch]](http://cybertron.cg.tu-berlin.de/eitz/tvcg_benchmark/benchmark.zip) [[PDF]](http://cybertron.cg.tu-berlin.de/eitz/pdf/2010_tvcg_prelim.pdf)
	- Sketch-Based Image Retrieval: Benchmark and Bag-of-Features Descriptors (IEEE T VIS COMPUT GR 2012), Eitz M et al.
	- [Benchmark] has 1,240 images labelled into 31 categories and 31 corresponding query sketches for testing
	- [Image] has 101,240 images for training
	- 28 participants(23 males, 5 females)
- GOLD [[Web]](http://smiles.xjtu.edu.cn/Download/Download_gold.html) [[Image(resized)]](http://image.ntua.gr/iva/datasets/ec1m/ec1m_landmarks.tar.gz) [[PDF]](http://smiles.xjtu.edu.cn/Publications/Our%20Paper/Sketch-Based%20Image%20Retrieval%20by%20Salient%20Contour%20Reinforcement.pdf)
	- Sketch-Based Image Retrieval by Salient Contour Reinforcement (IEEE T MULTIMEDIA 2016), Zhang Y et al.
	- contains more than 22,000 Flickr Crawled images together with their Geotags
	- extend image set, **image only**