# Frame-Recurrent Video Super-Resolution

This is the official repository for the Frame-Recurrent Video Super-Resolution project by Mehdi S. M. Sajjadi, Raviteja Vemulapalli and Matthew Brown, presented at CVPR 2018.


## Results
![demo](demo.gif)
(left: low-resolution input, middle: FRVSR output, right: high-resolution ground truth)

### More videos
<https://vimeo.com/album/5053944>

### Vid4
(link coming soon)

For download: These are the original HR frames of the Vid4 dataset, our downscaled LR frames and the estimated HR frames by FRVSR 10-128. Please note that the blur kernel size for downscaling was chosen to maximize Video-PSNR rather than perceptual quality and as such, the input videos may be slightly aliased (not enough blur), leading to perceptually unoptimal results. As we show in the paper, FRVSR beats the sliding-window baseline for all blur sizes and the the results of FRVSR are significantly more temporally consistent.

## Paper and Poster
- Paper (arXiv link): <https://arxiv.org/abs/1801.04590>
- Poster (in this repository): [poster.pdf](poster.pdf)

## Training dataset
1. Download the source file [dataset_train.txt](dataset_train.txt)
2. Install [youtube-dl](https://rg3.github.io/youtube-dl/)
3. Run `youtube-dl -civ --batch-file=dataset_train.txt`

## BibTex citation
```
@inproceedings{frvsr,
  title={{Frame-Recurrent Video Super-Resolution}},
  author={Sajjadi, Mehdi S. M. and Vemulapalli, Raviteja and Brown, Matthew},
  booktitle = {{The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)}},
  month = {June},
  year={2018}
}
```

For any questions, comments or help to get it to run, please don't hesitate to mail us: <msajjadi@tue.mpg.de>
