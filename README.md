# JARVIS

<p align="center">
  <img src="media/cqb_conv.png" alt="JARVIS helping me choose a firearm" width="100%"/>
</p>

# Your Own Voice Personal Assistant: Voice to Text to LLM to Speech

This project creates a personal assistant that converts voice input to text, processes it with an LLM (like GPT-3), and outputs speech—all within a web interface.

## How It Works

1. 🎤 The user speaks into the microphone.
2. ⌨️ Voice is converted to text using Deepgram.
3. 🤖 Text is sent to OpenAI's GPT-3 API to generate a response.
4. 📢 Response is converted to speech using ElevenLabs.
5. 🔊 Speech is played using Pygame.
6. 💻 The conversation is displayed on a webpage using Taipy.

## Requirements

**Python 3.8 - 3.11**

Ensure you have the following API keys:
- Deepgram
- OpenAI
- ElevenLabs

## How to Install

1. Clone the repository:
   ```bash
   git clone https://github.com/kunal7216/JARVIS.git
   ```

2. Install the requirements:
   ```bash
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the root directory and add the following variables:
   ```bash
   DEEPGRAM_API_KEY=XXX...XXX
   OPENAI_API_KEY=sk-XXX...XXX
   ELEVENLABS_API_KEY=XXX...XXX
   ```

## How to Use

1. Run `display.py` to start the web interface:
   ```bash
   python display.py
   ```

2. In another terminal, run `jarvis.py` to start the voice assistant:
   ```bash
   python main.py
   ```

- Once ready, both the web interface and the terminal will show `Listening...`.
- You can now speak into the microphone.
- Once you stop speaking, it will show `Stopped listening`.
- It will then start processing your request.
- When the response is ready, it will show `Speaking...`.
- The response will be played and displayed on the web interface.

### Example:

``` 
Listening...
Done listening
Finished transcribing in 1.21 seconds.
Finished generating response in 0.72 seconds.
Finished generating audio in 1.85 seconds.
Speaking...
--- USER: good morning jarvis ---
--- JARVIS: Good morning, Alex! How can I assist you today? ---
Listening...
...
``` 

--- 

This layout makes the instructions clearer and easier to follow.

<p align="center">
  <img src="media/good_morning.png" alt="Saying good morning" width="80%"/>
</p>#   J a r v i s 
 
 
