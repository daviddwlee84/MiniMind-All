# MiniMind All

Gather all MiniMind projects at one place

## Getting Started

```bash
GIT_LFS_SKIP_SMUDGE=1 git submodule update --init --recursive
```

```bash
uv install
```

## MiniMind

- [website](https://jingyaogong.github.io/minimind/)
- [code](https://github.com/jingyaogong/minimind)
- [model](https://huggingface.co/jingyaogong/MiniMind2)
- [dataset](https://huggingface.co/datasets/jingyaogong/minimind_dataset) / [dataset (modelscope)](https://www.modelscope.cn/datasets/gongjy/minimind_dataset)
- demo
  - [normal model](https://www.modelscope.cn/studios/gongjy/MiniMind)
  - [reasoning model](https://huggingface.co/spaces/jingyaogong/MiniMind) / [reasoning model (modelscope)](https://www.modelscope.cn/studios/gongjy/MiniMind-Reasoning)

> ```bash
> GIT_LFS_SKIP_SMUDGE=1 git submodule add https://github.com/jingyaogong/minimind.git MiniMind/code
> GIT_LFS_SKIP_SMUDGE=1 git submodule add https://huggingface.co/jingyaogong/MiniMind2 MiniMind/model
> GIT_LFS_SKIP_SMUDGE=1 git submodule add https://huggingface.co/datasets/jingyaogong/minimind_dataset MiniMind/dataset
> ```

## MiniMind-V

- [website](https://jingyaogong.github.io/minimind-v/)
- [code](https://github.com/jingyaogong/minimind-v)
- [model](https://huggingface.co/jingyaogong/MiniMind2-V)
- [dataset](https://huggingface.co/datasets/jingyaogong/minimind-v_dataset)
- [demo](https://www.modelscope.cn/studios/gongjy/MiniMind-V)

> ```bash
> GIT_LFS_SKIP_SMUDGE=1 git submodule add https://github.com/jingyaogong/minimind-v.git MiniMind-V/code
> GIT_LFS_SKIP_SMUDGE=1 git submodule add https://huggingface.co/jingyaogong/MiniMind2-V MiniMind-V/model
> GIT_LFS_SKIP_SMUDGE=1 git submodule add https://huggingface.co/datasets/jingyaogong/minimind-v_dataset MiniMind-V/dataset
> ```

---

```bash
# sudo snap install astral-uv
# This is simpler
curl -LsSf https://astral.sh/uv/install.sh | sh
uv python install 3.10
uv init --python 3.10
# uv python pin 3.10
# Should manually solve gradio version limit
uv add -r MiniMind-V/code/requirements.txt
```

TODO: if I want to change code, use [`git submodule set-url`](https://git-scm.com/docs/git-submodule#Documentation/git-submodule.txt-set-url--ltpathgtltnewurlgt) to change to my fork
