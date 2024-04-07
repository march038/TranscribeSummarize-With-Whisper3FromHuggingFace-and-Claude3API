Hi!

This script is designed to transcribe a local MP3 file using the Whisper 3 Large model from HuggingFace and then summarize the transcription result with Claude 3 Sonnet. 
For this example, I used a YouTube video converted from MP4 to MP3, in which Greg Kamradt explains the key aspects of Langchain (https://www.youtube.com/watch?v=vGP4pQdCocw).
The prompt for Claude 3 then requests the model to summarize the key concepts of the transcription and to use headlines for each concept.

The following libraries are required to run the script:

-os (for handling environment variables to conceal sensitive information)

-torch (to configure the device for GPU or CPU usage)

-transformers (to load and utilize the Whisper 3 Large model for inference)

-dotenv with load_dotenv (to manage environment variables and use directory paths)

-anthropic with Anthropic (to interact with the Claude 3 API/SDK)

As is common practice, I utilized a Jupyter Notebook environment with Conda as the package manager and provided explanations for each line of code using comments within the script.

Hint: There's a known issue when using the anthropic SDK if one doesn't utilize the latest version of anthropic. I opted for version 0.21.3 and installed the package using pip into the Conda environment.
