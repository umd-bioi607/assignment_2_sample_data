# Sample data for global alingment assignment

The `sample_data` folder contains two files, `input.sp` and `input.aln`. The 
`input.sp` file contains several alignment problem records, as described in the 
specification, and `input.aln` contains the corresponding outputs.

The ouput was generated from the input via the command:

```bash
saligner sample_data/input.sp 2 5 sample_data/input.aln
```

So, the values passed to `saligner` for the mismatch penalty and gap penalty are 2 and 5 respectively,
but recall that we set the internal score in the aligner to `-2` and `-5`.  A match implicitly has 
penalty 0, and the scores for  each probelm in the sample ouput represent the *maximum* achievable
score.


