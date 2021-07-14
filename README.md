### Installing prerequesites

sktime

Maybe conda env?


### Calling the notebook

We are working with a lot of data. By default, the memory limit of Jupyter notebooks is limited to 0.5 GB, resulting in crashes. Increase it to 10 GB by calling the notebook with:

```bash
jupyter notebook --NotebookApp.max_buffer_size=10737418240
```
