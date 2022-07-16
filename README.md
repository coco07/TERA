The toolkit has **three major usages**:

### Pretrain

- Pretrain upstream models, including Mockingjay, Audio ALBERT and TERA.
- Document: [**pretrain/README.md**](./s3prl/pretrain/README.md)

### Upstream

- Easily load most of the existing upstream models with pretrained weights in a unified I/O interface.
- Pretrained models are registered through **torch.hub**, which means you can use these models in your own project by one-line plug-and-play without depending on this toolkit's coding style.
- Document: [**upstream/README.md**](./s3prl/upstream/README.md)

### Downstream

- Utilize upstream models in lots of downstream tasks
- Benchmark upstream models with [**SUPERB Benchmark**](./s3prl/downstream/docs/superb.md)
- Document: [**downstream/README.md**](./s3prl/downstream/README.md)

Below is an **intuitive illustration** on how this toolkit may help you:
\
\
<img src="./file/S3PRL-interface.png" width="900"/>
\
\
Feel free to use or modify our toolkit in your research. Here is a [list of papers using our toolkit](#used-by). Any question, bug report or improvement suggestion is welcome through [opening up a new issue](https://github.com/s3prl/s3prl/issues). 

If you find this toolkit helpful to your research, please do consider citing [our papers](#citation), thanks!

## Installation

1. **Python** >= 3.6
2. Install **sox** on your OS
3. Install s3prl

```sh
pip install -e ./
```

4. Some upstream models require special dependencies. If you encounter error with a specific upstream model, you can look into the `README.md` under each `upstream` folder. E.g., `upstream/pase/README.md`
