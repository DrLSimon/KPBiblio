# Papers on Detectors only
**[IJCV'11]** Aanæs et al. *Interesting interest points.*  
http://roboimagedata.imm.dtu.dk/papers/IJCV_2011.pdf  
> This article compares several detectors () but not the descriptors. It is associated with
> a dataset with accurate ground-truth that coud be very interesting: http://roboimagedata.compute.dtu.dk/?page_id=24.

**[ECCV'08]** Agrawal et al. *CenSurE: Center Surround Extremas for Realtime Feature Detection and Matching*  
http://link.springer.com/chapter/10.1007%2F978-3-540-88693-8_8

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

## benchmarking papers
**[IJCV'04]** Mikolajczyk et al. *A Comparison of Affine Region Detectors.*  
http://www.robots.ox.ac.uk/~vgg/research/affine/det_eval_files/vibes_ijcv2004.pdf

http://www.robots.ox.ac.uk/~vgg/research/affine/

**[ECCV'12]** Heinly et al. *Comparative evaluation of binary features.*  
https://www.cs.unc.edu/~jheinly/publications/eccv2012-heinly.pdf

----

# Nearest Neighbor and Hashing
## Nearest Neighbor
**[ECCV'08]** Kumar et al. *What is a Good Nearest Neighbors Algorithm for Finding Similar Patches in Images?*  
http://www1.cs.columbia.edu/CAVE/publications/pdfs/Kumar_ECCV08_2.pdf

**[PAMI'11]** Jegou et al. *Product quantization for nearest neighbor search.*  
http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.164.8334&rep=rep1&type=pdf

## Hashing without supervision
**[NIPS'09]** Weiss et al. *Spectral Hashing.*  
http://papers.nips.cc/paper/3383-spectral-hashing.pdf

**[NIPS'09]** Raginsky et al. *Locality-Sensitive Binary Codes from Shift-Invariant Kernels.*  
https://www.robots.ox.ac.uk/~vgg/rg/papers/binarycodes.pdf


## Hashing with supervision
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

----
# Some slides
Luca Ricci: visual odometry vs slam, PTAM
http://www.dis.uniroma1.it/~venditt/didattica/eir/04_VisualOdometry.pdf

Anonymous: CenSurE (and other stuff)
https://www.scss.tcd.ie/Gerard.Lacey/Gerard_Lacey_Homepage/CS4053_Course_files/Lecture%20011%20SURF%20Censure%20Photosynth%20CBIR.pdf

