## Soft clipping dodgy bases
### Dependencies

- python >= 3.6
- python libaries `loguru, click, pysam`
- samtools

```
python -m pip install requirements.txt
```

### Usage

Input bam file is the `ivar trim` or `samtools ampliconclip` output

```
Usage: mask_dgy_bases.py [OPTIONS] BAM_FILE
Options:
  -o, --output-name TEXT
  --verbose                    [default: False]
  -l, --cutoff-length INTEGER  Cut-off length of the edge containing the dodge
                               base  [default: 20]

  --ref-name TEXT              NCBI Reference name  [default: MN908947.3]
  -t, --threads INTEGER        # threads  [default: 4]
  --help                       Show this message and exit.
```