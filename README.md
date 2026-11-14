# Tiny Word Brain 3.0 🧠

A browser-based AI translator between plain English and Gen Z / Gen Alpha internet slang.

## Current mobile-friendly model

- **Model:** SmolLM2-135M-Instruct ONNX (4-bit)
- **Runtime:** Transformers.js
- **Phone mode:** CPU/WASM to reduce GPU memory pressure
- **Desktop mode:** WebGPU when available
- The inference library is loaded only after the user taps the load button.
- Model files are cached by the browser after first download.

We moved from Qwen3-0.6B to the smaller 135M model after an Android browser tab crashed during model startup. This smaller model is a compromise: it is more likely to fit on a phone, but it is less capable than the 0.6B model and may struggle with nuanced slang, sarcasm, and context.

## Use it

Open the GitHub Pages site and tap **Load tiny AI model**. Keep the tab open while the model downloads and initializes. First load needs an internet connection; later visits may reuse the browser cache.

## Privacy and limitations

- Inference happens in the browser after the model is downloaded.
- No app backend or paid inference API is used.
- The model download comes from Hugging Face via Transformers.js.
- This is a small general-purpose language model prompted for slang translation; it is not fine-tuned specifically for slang.
- Device compatibility and speed vary. If the browser still closes, the phone may not have enough available memory for local inference.

## Technology

- HTML, CSS and JavaScript
- [Transformers.js](https://huggingface.co/docs/transformers.js)
- [SmolLM2-135M-Instruct ONNX](https://huggingface.co/onnx-community/SmolLM2-135M-Instruct-ONNX)
- GitHub Pages

