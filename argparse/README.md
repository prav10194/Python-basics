## Creating a basic arg parser

```python
import argparse

if __name__ == "__main__":
    parser = argparse.ArgumentParser(usage='python3 %(prog)s -i <inputfile.json> -o <outputfile.json>', description='Arguments for Django parser.', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
    parser.add_argument('-i', '--inputfile', help='provide path for the input file to be parsed')
    parser.add_argument('-o', '--outputfile', default='scanoutputjson.json', help='provide path for the output file')
    args = parser.parse_args()
    print("args.inputfile", args.inputfile)
    print("args.outputfile", args.outputfile)
 ```
 
 #### Running help
 
 ```cmd
 python3 file.py -h
 ```
 
