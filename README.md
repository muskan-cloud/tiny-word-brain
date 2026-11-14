# Tiny Word Brain 3.0 🧠

A tiny, browser-based AI translator between plain English and Gen Z / Gen Alpha internet slang.

## What changed in 3.0

- Uses the pretrained **Qwen3-0.6B** language model through Transformers.js.
- Runs inference in the browser using WebGPU when available, with a CPU/WASM fallback.
- Uses 4-bit quantized model weights to reduce download and memory requirements.
- Supports English → slang and slang → English.
- Offers Gen Z, Gen Alpha, mixed, and natural internet styles with 10 intensity levels.
- Model files are cached by the browser after the first download.
- No application backend or paid inference API is used.

## Run it

Open the GitHub Pages site and tap **Load tiny AI model**. On first use, the browser downloads the model from Hugging Face. Keep the tab open until loading completes. Later visits should reuse the browser cache.

## Important limitations

- This is a small general-purpose language model prompted for slang translation; it is not fine-tuned specifically for slang.
- It can misunderstand sarcasm, cultural references, or ambiguous phrases.
- First-time model download can be substantial, and performance depends on the device. WebGPU is preferred; CPU/WASM fallback may be slower.
- Model files are fetched from Hugging Face. The text entered for translation is processed locally in the browser after the model loads.

## Technology

- HTML, CSS and JavaScript
- [Transformers.js](https://huggingface.co/docs/transformers.js)
- [Qwen3-0.6B ONNX](https://huggingface.co/onnx-community/Qwen3-0.6B-ONNX)
- GitHub Pages

## Model license

Check the model card and its license before redistributing or using the model commercially.
