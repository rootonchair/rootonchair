# Vinh H. Pham

Open-source AI engineer in Ho Chi Minh City, working on diffusion/video generation, 4-bit diffusion inference, LLM/VLM quantization, model serving, and practical ML infrastructure.

[GitHub](https://github.com/rootonchair) | [Hugging Face](https://huggingface.co/rootonchair) | [Website](https://rootonchair.github.io/)

`Diffusion` · `Video generation` · `SVDQuant / 4-bit inference` · `LLM/VLM quantization` · `Model serving` · `Open-source ML`

## Open-source impact

| Project | ✓ Merged PRs | Representative merged work |
| --- | ---: | --- |
| [huggingface/diffusers](https://github.com/huggingface/diffusers)<br><sub>★ 34,623 / forks 7,356</sub> | [24](https://github.com/huggingface/diffusers/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | [Nunchaku Lite quantization backend](https://github.com/huggingface/diffusers/pull/14100), [LTX2 distilled checkpoint support](https://github.com/huggingface/diffusers/pull/12934), [framewise LTX Video VAE encoding/decoding](https://github.com/huggingface/diffusers/pull/10488) |
| [huggingface/transformers](https://github.com/huggingface/transformers)<br><sub>★ 166,749 / forks 34,699</sub> | [8](https://github.com/huggingface/transformers/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | [PoolFormer fast image processor](https://github.com/huggingface/transformers/pull/37182), [BridgeTower fast image processor](https://github.com/huggingface/transformers/pull/37373) |
| [huggingface/blog](https://github.com/huggingface/blog) | [1](https://github.com/huggingface/blog/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | [Bringing Nunchaku 4-bit Diffusion Inference to Diffusers](https://huggingface.co/blog/nunchaku-diffusers), co-authored with the Diffusers team |
| [sgl-project/sglang](https://github.com/sgl-project/sglang)<br><sub>★ 36,508 / forks 9,189</sub> | [1](https://github.com/sgl-project/sglang/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | [Z-Image text encoder config fix](https://github.com/sgl-project/sglang/pull/18560) |
| [d2l-ai/d2l-vi](https://github.com/d2l-ai/d2l-vi)<br><sub>★ 663 / forks 254</sub> | [108](https://github.com/d2l-ai/d2l-vi/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | Vietnamese ML education translation/revision |
| [mlbvn/ml-yearning-vi](https://github.com/mlbvn/ml-yearning-vi)<br><sub>★ 1,234 / forks 395</sub> | [23](https://github.com/mlbvn/ml-yearning-vi/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | Vietnamese ML education translation/revision |
| [d2l-ai/d2l-en](https://github.com/d2l-ai/d2l-en)<br><sub>★ 29,724 / forks 5,140</sub> | [7](https://github.com/d2l-ai/d2l-en/pulls?q=is%3Apr+author%3Arootonchair+is%3Amerged) | Documentation fixes |

Selected upstream work includes the Nunchaku Lite 4-bit quantization backend in Diffusers, LTX2 distilled checkpoint support, LTX Video VAE framewise encoding/decoding, Diffusers pipeline/test improvements, a Z-Image fix in SGLang, and Vietnamese ML education work across Dive into Deep Learning and Machine Learning Yearning.

## Projects

| Project | What it does |
| --- | --- |
| [nunchaku-lite](https://github.com/rootonchair/nunchaku-lite) | Lean runtime for SVDQuant W4A4 diffusion models in standard Diffusers pipelines, with native CUDA kernels published as [`nunchaku-lite-kernels`](https://huggingface.co/kernels/rootonchair/nunchaku-lite-kernels) on the Hub and `torch.compile` support |
| [diffuse-compressor](https://github.com/rootonchair/diffuse-compressor) | Model-agnostic SVDQuant toolkit that calibrates and quantizes diffusion transformers to INT4 / NVFP4 and exports Nunchaku-compatible checkpoints |
| [lite-infer](https://huggingface.co/lite-infer) | Hub organization with 30 prequantized Nunchaku Lite checkpoints: FLUX.1 / FLUX.2 Klein, Qwen-Image and Qwen-Image-Edit, Z-Image-Turbo, ERNIE-Image-Turbo, Krea-2-Turbo, and LTX-2.3 Distilled |
| [diffuser_layerdiffuse](https://github.com/rootonchair/diffuser_layerdiffuse) | Transparent image generation with Diffusers (LayerDiffuse) |

## Adopted work

| Project | Where it is used | Adopting project scale |
| --- | --- | ---: |
| [rootonchair/nunchaku-lite](https://github.com/rootonchair/nunchaku-lite) | Diffusers: official quantization backend with a [dedicated docs page](https://github.com/huggingface/diffusers/blob/main/docs/source/en/quantization/nunchaku.md)<br>SD.Next: built-in [Nunchaku-Lite inference engine](https://github.com/vladmandic/sdnext/blob/master/CHANGELOG.md#update-for-2026-08-07) that [installs the package](https://github.com/vladmandic/sdnext/blob/master/pipelines/minimax/minimax_nunchaku.py#L33) and ships 11 [lite-infer checkpoints](https://github.com/vladmandic/sdnext/blob/master/data/reference-nunchaku.json#L216-L293) in its model reference | [★ 34,623 / forks 7,356](https://github.com/huggingface/diffusers)<br>[★ 7,346 / forks 585](https://github.com/vladmandic/sdnext) |
| [rootonchair/LTX-2-19b-distilled](https://huggingface.co/rootonchair/LTX-2-19b-distilled) | Listed in vLLM Omni's supported-model table for [`LTX2DistilledOneStagePipeline` and `LTX2DistilledTwoStagePipeline`](https://github.com/vllm-project/vllm-omni/blob/main/docs/models/supported_models.md#L48-L49) | [★ 7,101 / forks 1,802](https://github.com/vllm-project/vllm-omni) |
| [rootonchair/diffuser_layerdiffuse](https://github.com/rootonchair/diffuser_layerdiffuse) | SD.Next includes a [`LayerDiffuse: Transparent Image` extension](https://github.com/vladmandic/sdnext/blob/master/scripts/layerdiffuse_ext.py#L6-L25) and links back to this project in the extension UI | [★ 7,346 / forks 585](https://github.com/vladmandic/sdnext) |

## Selected AI systems work

- Video: Diffusers integrations, LTX video support, [LTX-2.3 Distilled Diffusers conversions](https://huggingface.co/rootonchair/LTX-2.3-Distilled-v1.1-Diffusers), transparent image generation, and model execution workflows.
- 4-bit diffusion: SVDQuant INT4 / NVFP4 pipelines for image and video transformers, including [MiniMax-H3](https://huggingface.co/rootonchair/MiniMax-H3-nunchaku-lite-nvfp4), [Ideogram v4](https://huggingface.co/rootonchair/ideogram-v4-fast-nunchaku-lite-nvfp4), and [ERNIE-Image-Turbo](https://huggingface.co/rootonchair/ERNIE-Image-Turbo-nunchaku-lite).
- VLM quantization: GGUF and AWQ releases for image-text models such as [Lens-Turbo](https://huggingface.co/rootonchair/Lens-Turbo-GGUF), [Vintern-3B](https://huggingface.co/rootonchair/Vintern-3B-beta-GGUF), [Vintern-1B](https://huggingface.co/rootonchair/Vintern-1B-v3_5-GGUF-ext), [EraX-VL-7B](https://huggingface.co/rootonchair/EraX-VL-7B-V1.0-GGUF), and [InternVL2.5-4B](https://huggingface.co/rootonchair/InternVL2_5-4B-AWQ).
- Serving: quantized/GGUF model artifacts, runtime tooling, llama.cpp-based OCR serving, and diffusion model compression experiments.
- Tooling: practical patches across Hugging Face Diffusers/Transformers and related open-source ML projects.

## Current focus

I am mostly interested in making generative models easier to run, adapt, compress, and serve in real systems.
