# Vinh H. Pham

Open-source AI engineer in Ho Chi Minh City, working on diffusion/video generation, LLM/VLM quantization, model serving, and practical ML infrastructure.

[GitHub](https://github.com/rootonchair) | [Hugging Face](https://huggingface.co/rootonchair) | [Website](https://rootonchair.github.io/)

`Diffusion` · `Video generation` · `LLM/VLM quantization` · `Model serving` · `Open-source ML`

## Open-source impact

| Project | ✓ Merged PRs | Representative merged work |
| --- | ---: | --- |
| [huggingface/diffusers](https://github.com/huggingface/diffusers)<br><sub>★ 33,746 / forks 7,011</sub> | [22](https://github.com/huggingface/diffusers/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | [LTX2 distilled checkpoint support](https://github.com/huggingface/diffusers/pull/12934), [framewise LTX Video VAE encoding/decoding](https://github.com/huggingface/diffusers/pull/10488) |
| [huggingface/transformers](https://github.com/huggingface/transformers)<br><sub>★ 161,148 / forks 33,378</sub> | [8](https://github.com/huggingface/transformers/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | [PoolFormer fast image processor](https://github.com/huggingface/transformers/pull/37182), [BridgeTower fast image processor](https://github.com/huggingface/transformers/pull/37373) |
| [sgl-project/sglang](https://github.com/sgl-project/sglang)<br><sub>★ 28,869 / forks 6,257</sub> | [1](https://github.com/sgl-project/sglang/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | [Z-Image text encoder config fix](https://github.com/sgl-project/sglang/pull/18560) |
| [d2l-ai/d2l-vi](https://github.com/d2l-ai/d2l-vi)<br><sub>★ 659 / forks 255</sub> | [108](https://github.com/d2l-ai/d2l-vi/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | Vietnamese ML education translation/revision |
| [mlbvn/ml-yearning-vi](https://github.com/mlbvn/ml-yearning-vi)<br><sub>★ 1,089 / forks 374</sub> | [23](https://github.com/mlbvn/ml-yearning-vi/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | Vietnamese ML education translation/revision |
| [d2l-ai/d2l-en](https://github.com/d2l-ai/d2l-en)<br><sub>★ 28,941 / forks 5,069</sub> | [7](https://github.com/d2l-ai/d2l-en/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | Documentation fixes |

Selected upstream work includes LTX2 distilled checkpoint support, LTX Video VAE framewise encoding/decoding, Diffusers pipeline/test improvements, a Z-Image fix in SGLang, and Vietnamese ML education work across Dive into Deep Learning and Machine Learning Yearning.

## Adopted work

| Project | Integration evidence | Adopting project scale |
| --- | --- | ---: |
| [rootonchair/LTX-2-19b-distilled](https://huggingface.co/rootonchair/LTX-2-19b-distilled) | Listed in vLLM Omni's supported-model table for [`LTX2TwoStagesPipeline` and `LTX2ImageToVideoTwoStagesPipeline`](https://github.com/vllm-project/vllm-omni/blob/main/docs/models/supported_models.md#L40-L41) | [★ 4,858 / forks 1,028](https://github.com/vllm-project/vllm-omni) |
| [rootonchair/diffuser_layerdiffuse](https://github.com/rootonchair/diffuser_layerdiffuse) | SD.Next includes a [`LayerDiffuse: Transparent Image` extension](https://github.com/vladmandic/sdnext/blob/master/scripts/layerdiffuse_ext.py#L6-L25) and links back to this project in the extension UI | [★ 7,113 / forks 558](https://github.com/vladmandic/sdnext) |

## Selected AI systems work

- Video: Diffusers integrations, LTX video support, transparent image generation, and model execution workflows.
- Quantization: GGUF and AWQ releases for image-text models such as [Vintern-3B](https://huggingface.co/rootonchair/Vintern-3B-beta-GGUF), [Vintern-1B](https://huggingface.co/rootonchair/Vintern-1B-v3_5-GGUF-ext), [EraX-VL-7B](https://huggingface.co/rootonchair/EraX-VL-7B-V1.0-GGUF), and [InternVL2.5-4B](https://huggingface.co/rootonchair/InternVL2_5-4B-AWQ).
- Serving: quantized/GGUF model artifacts, runtime tooling, and diffusion model compression experiments.
- Tooling: practical patches across Hugging Face Diffusers/Transformers and related open-source ML projects.

## Current focus

I am mostly interested in making generative models easier to run, adapt, compress, and serve in real systems.
