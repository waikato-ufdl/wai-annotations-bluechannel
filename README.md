# wai-annotations-bluechannel
wai.annotations module for dealing with image segmentation images that use the blue channel.

## Plugins
### FROM-BLUE-CHANNEL-IS
Reads image segmentation files in the blue-channel format

#### Domain(s):
- **Image Segmentation Domain**

#### Options:
```
usage: from-blue-channel-is [-I FILENAME] [-i FILENAME] [-N FILENAME] [-n FILENAME] [--seed SEED] [--image-path-rel PATH] --labels LABEL [LABEL ...]

optional arguments:
  -I FILENAME, --inputs-file FILENAME
                        Files containing lists of input files (can use glob syntax)
  -i FILENAME, --input FILENAME
                        Input files (can use glob syntax)
  -N FILENAME, --negatives-file FILENAME
                        Files containing lists of negative files (can use glob syntax)
  -n FILENAME, --negative FILENAME
                        Files that have no annotations (can use glob syntax)
  --seed SEED           the seed to use for randomisation
  --image-path-rel PATH
                        Relative path to image files from annotations
  --labels LABEL [LABEL ...]
                        specifies the labels for each index
```

### TO-BLUE-CHANNEL-IS
Writes image segmentation files in the blue-channel format

#### Domain(s):
- **Image Segmentation Domain**

#### Options:
```
usage: to-blue-channel-is [--annotations-only] -o PATH [--split-names SPLIT NAME [SPLIT NAME ...]] [--split-ratios RATIO [RATIO ...]]

optional arguments:
  --annotations-only    skip the writing of data files, outputting only the annotation files
  -o PATH, --output PATH
                        the directory to write the annotation images to
  --split-names SPLIT NAME [SPLIT NAME ...]
                        the names to use for the splits
  --split-ratios RATIO [RATIO ...]
                        the ratios to use for the splits
```
