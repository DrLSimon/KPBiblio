# Papers on Detectors only
**[IJCV'11]** Aanæs et al. *Interesting interest points.*  
http://roboimagedata.imm.dtu.dk/papers/IJCV_2011.pdf  
> This article compares several detectors () but not the descriptors. It is associated with
> a dataset with accurate ground-truth that coud be very interesting: http://roboimagedata.compute.dtu.dk/?page_id=24.

**[ECCV'08]** Agrawal et al. *CenSurE: Center Surround Extremas for Realtime Feature Detection and Matching*  
http://link.springer.com/chapter/10.1007%2F978-3-540-88693-8_8

**List of other articles to be gathered here** 
* FAST
* OFAST (ORB detector ?)
* AGAST
* KAZE (non linear scale space)


----

# Papers on descriptors (and possibly detectors)
**[PAMI'11]** Calonder et al. *BRIEF: Computing a local binary descriptor very fast.*  
http://cvlabwww.epfl.ch/~lepetit/papers/calonder_pami11.pdf
> This is the (more complete) journal version of BRIEF.

**[CVPR'12]** Alahi et al. FREAK: Fast REtinA Keypoints
http://infoscience.epfl.ch/record/175537/files/2069.pdf

**[NIPS'12, CVPR'13]** Le Petit et al. *Bin Boost.*  
http://cvlab.epfl.ch/research/detect/binboost

**[PAMI'14]** Simonyan et al. *Learning Local Feature Descriptors Using Convex Optimisation.*  
http://www.robots.ox.ac.uk/~vgg/publications/2014/Simonyan14/simonyan13a.pdf

**[CVPR'15]** Balntas et al.  *BOLD.*  
http://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Balntas_BOLD_-_Binary_2015_CVPR_paper.pdf

**[CVPR'15]** Han et al. *MatchNet (CNN).*  
http://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Han_MatchNet_Unifying_Feature_2015_CVPR_paper.pdf

**[CVPR'15]** Zagoruyko *DeepCompare (Komodakis).*  
http://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Zagoruyko_Learning_to_Compare_2015_CVPR_paper.pdf

**[ICCV'15]** Simo-Serra et al. *Discriminative Learning of Deep Convolutional Feature Point Descriptors*  
http://www.iri.upc.edu/files/scidoc/1694-Discriminative-Learning-of-Deep-Convolutional-Feature-Point-Descriptors.pdf

**[ARXIV'16]** Balntas et al. *PN-Net: Conjoined triple deep network for learning local image descriptors.*  
http://arxiv.org/pdf/1601.05030v1.pdf

**[ARXIV'16]** Moo Yi et al. *LIFT: Learned Invariant Feature Transform*  
http://arxiv.org/pdf/1603.09114v1.pdf
> Mirror the SIFT construction but with a network per module (detection,
> orientation, description). Only the whole pipeline is applied to a 
> precomputed scale-space pyramid.

**List of other descriptors to be gathered here**
* BRISK
* ORB https://www.willowgarage.com/sites/default/files/orb_final.pdf
* bit-plane http://arxiv.org/pdf/1602.00307v1.pdf
* SIFT
* ASIFT
* SURF
* LATCH http://www.openu.ac.il/home/hassner/projects/LATCH/
* LDB http://lbmedia.ece.ucsb.edu/research/binaryDescriptor/ISMAR2012-LDP-final.pdf
* AKAZE http://isit.u-clermont1.fr/~ab/Publications/Alcantarilla_etal_BMVC13.pdf (Accelarated KAZE detector and modified LDB descriptor for rotation and scale invariance)
* A tutorial sequence https://gilscvblog.com/2013/08/26/tutorial-on-binary-descriptors-part-1/
* A 2014 survey:  
http://www.embedded-vision.com/sites/default/files/apress/computervisionmetrics/chapter6/9781430259299_Ch06.pdf
* A 2016 survey:
http://arxiv.org/pdf/1607.08368v1.pdf


## benchmarking papers
**[IJCV'04]** Mikolajczyk et al. *A Comparison of Affine Region Detectors.*  
http://www.robots.ox.ac.uk/~vgg/research/affine/det_eval_files/vibes_ijcv2004.pdf

http://www.robots.ox.ac.uk/~vgg/research/affine/

**[ECCV'12]** Heinly et al. *Comparative evaluation of binary features.*  
https://www.cs.unc.edu/~jheinly/publications/eccv2012-heinly.pdf

**[ICIP'14]** Rey-Otero et al. *Comparing Feature Detectors: A bias in the repeatability criteria, and how to correct it*
https://arxiv.org/pdf/1409.2465v2.pdf

**[ARXIV'16]** Fan et al. *Do We Need Binary Features for 3D Reconstruction?*  
http://arxiv.org/pdf/1602.04502v1.pdf
> This paper advocates that SIFT+ANN is better than binary descriptor+brute
> force. But this is a paper in the context of multiview reconstruction, which
> per se is meant offline (real-time is not needed). Among 3 binary descriptors
> (ORB, BRISK, and FRIF), FRIF is considered the best.

----

# Nearest Neighbor and Hashing
## Nearest Neighbor
**[ECCV'08]** Kumar et al. *What is a Good Nearest Neighbors Algorithm for Finding Similar Patches in Images?*  
http://www1.cs.columbia.edu/CAVE/publications/pdfs/Kumar_ECCV08_2.pdf

**[PAMI'11]** Jegou et al. *Product quantization for nearest neighbor search.*  
http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.164.8334&rep=rep1&type=pdf

**[CRV'12]** Muja et Lowe. *Fast Matching of Binary Features*  
http://www.cs.ubc.ca/~lowe/papers/12mujaCRV.pdf

## Hashing without supervision
**[NIPS'09]** Weiss et al. *Spectral Hashing.*  
http://papers.nips.cc/paper/3383-spectral-hashing.pdf

**[NIPS'09]** Raginsky et al. *Locality-Sensitive Binary Codes from Shift-Invariant Kernels.*  
https://www.robots.ox.ac.uk/~vgg/rg/papers/binarycodes.pdf

**[NIPS'13]** Neyshabur et al. *The Power of Asymmetry in Binary Hashing*  
http://ttic.uchicago.edu/~yury/papers/nips2013_asym.pdf

**[TOM'15]** Nv et al. *Asymmetric Cyclical Hashing for Large Scale Image Retrieval*  
https://www.researchgate.net/profile/Wing_Ng8/publication/277667147_Asymmetric_Cyclical_Hashing_for_Large_Scale_Image_Retrieval/links/55ae125508aed614b097f3d1.pdf

**[CVPR'15]**  Carreira-Perpinan et al. *Hashing with Binary Autoencoders*  
http://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Carreira-Perpinan_Hashing_With_Binary_2015_CVPR_paper.pdf


**[CVPR'15]** Liong et al. *Deep Hashing for Compact Binary Codes Learning*  
http://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Liong_Deep_Hashing_for_2015_CVPR_paper.pdf
> I like the related work section of this one. Other than that it is a deep
> net (which architecture is not really clear)

**[CVPR'15]** Shen et al. *Supervised discrete hashing.*  
http://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Shen_Supervised_Discrete_Hashing_2015_CVPR_paper.pdf

**[ARXIV'15]** Do et al. *Discrete Hashing with Deep Neural Network.*  
http://arxiv.org/pdf/1508.07148v1.pdf

**[CVPR'15]** Lai et al. *Simultaneous Feature Learning and Hash Coding with Deep Neural Networks.*  
http://arxiv.org/pdf/1504.03410.pdf
> This is a deep conv net, implementing *triplet ranking loss*, where the triplet
> is made of two positive image and a negative one. It's a hinge loss, between
> the positive distance and negative distance. It is probably classical in
> metric learning but it was introduced in Hashing only in 2012 by
> > **[NIPS'12]** M. Norouzi, D. J. Fleet, and R. Salakhutdinov. *Hamming distance metric learning.* http://papers.nips.cc/paper/4808-hamming-distance-metric-learning.pdf
>
> This is related to networks  known as tripletNets: http://tce.webee.eedev.technion.ac.il/wp-content/uploads/sites/8/2016/01/Elad-Hofer.pdf
> Implemented in torch on github: https://github.com/eladhoffer/TripletNet
> This kind of networks were used also in face recognition systems such as
> Google FaceNet: http://arxiv.org/pdf/1503.03832v1.pdf 
> github implementation in torch: https://github.com/Atcold/torch-TripletEmbedding

**[CVPR'15]** Zhao et al. *Deep Semantic Ranking Based Hashing for Multi-Label
Image Retrieval*  
http://arxiv.org/pdf/1501.06272.pdf

**[IEEE'16]** Wang et al. *Learning to Hash for Indexing Big Data—A Survey*  
http://arxiv.org/pdf/1509.05472.pdf
> This is a recent survey on hashing. Sec 5 is on deep net and hashing. As
> pointed out by the authors, deep net can yield good performance, but the hash
> generation is probably costly, which might interfere with the original goal.
> Sec 5 is also available separately (but  outdated) here: http://www.ee.columbia.edu/~wliu/WeiLiu_DLHash.pdf


## Hashing with supervision
**[IJAR'09]** Salakhutdinov and Hinton. *Semantic Hashing.*
http://nuyoo.utm.mx/~jjf/rna/A15%20Semantic%20Hashing.pdf

**[CVPR'11]** Gong et al. *Iterative Quantization: A Procrustean Approach to Learning Binary Codes.*  
http://slazebni.cs.illinois.edu/publications/cvpr11_small_code.pdf

**[CVPR'10]** Wang et al. *Semi-Supervised Hashing for Scalable Image Retrieval (SSH)*  
http://www.sanjivk.com/SSH_CVPR10.pdf
> This paper is close to our settings, since the supervision is given by positive and negative
> image pairs (although it is only semi-supervised because only a fraction of the pairs are labelled).
> In essence, it implements a modified PCA where the plain variance is replaced by a reduced variance (which is
> the difference of variance in negative pairs and that of positive pairs, or inter-class variance) -- see eq 16 in the paper.
> Also the performance are improved by relaxing the independance conditions on
> the principal directions.

**[CVPR12]** Liu et al. *Supervised Hashing with Kernels.*  
http://www.ee.columbia.edu/~wliu/CVPR12_ksh.pdf
> Another one with positive / negative pairs supervision.

**[CVPR'15]** Shen et al. *Supervised Discrete Hashing*  
http://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Shen_Supervised_Discrete_Hashing_2015_CVPR_paper.pdf
> Code: https://github.com/bd622/DiscretHashing

----
# Theoretical papers
[JMIV'15] Lindeberg. *Image Matching Using Generalized Scale-Space Interest Points*  
ftp://ftp.nada.kth.se/CB/papers/Lin15-JMIV.pdf
> A part from many interesting stuff, there is a useful tip: Perform
> detection and description on the log(I) so that multiplicative constant
>  (e.g f-number, illumination) become additive and are removed thanks to 
>  derivative (or  difference)

# Some code and datatsets
**VLBenchmarks** http://www.vlfeat.org/benchmarks/index.html

**DTU robot dataset** http://roboimagedata.compute.dtu.dk 
* **2014**  http://roboimagedata.compute.dtu.dk/?page_id=36
* **2010** http://roboimagedata.compute.dtu.dk/?page_id=24

**Deep Binary Hashing** https://github.com/kevinlin311tw/caffe-cvprw15

----
# Some slides
Luca Ricci: visual odometry vs slam, PTAM
http://www.dis.uniroma1.it/~venditt/didattica/eir/04_VisualOdometry.pdf

Anonymous: CenSurE (and other stuff)
https://www.scss.tcd.ie/Gerard.Lacey/Gerard_Lacey_Homepage/CS4053_Course_files/Lecture%20011%20SURF%20Censure%20Photosynth%20CBIR.pdf

Tomasz Malisiewicz Blog
http://www.computervisionblog.com/2016/01/why-slam-matters-future-of-real-time.html

CVPR'16 tutorial on hashing
http://sglab.kaist.ac.kr/~sungeui/image_tutorial/P2_Lin16.pdf

----
**Markdown Cheat-sheet**
https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

