# audioWhisper
Listen to any audio stream on your machine and print out the transcribed or translated audio. 

## Setup
1. choose envs of your choices.
2. clone this repo into your local storage.
3. run `pip install -r requirements.txt`
4. run `python audioWhisper.py`

## Command-line flags
|      --flags          |  Default Value  |      Description                                                                                       |
|:---------------------:|:---------------:|:------------------------------------------------------------------------------------------------------:|
|`--device`             | false           | To print all available devices                                                                         |
|`--model`              | small           | Select model list. refer [here](https://github.com/openai/whisper#available-models-and-languages)      |
|`--task`               | transcribe      | Choose between transcribe the audio or to translate the audio to English                               |
|`--device_index`       | 2               | Choose the output device to listen to and transcribe the audio from this device                        |
|`--channel`            | 2               | Number of channels of the output device                                                                |
|`--rate`               | 44100           | Sampling rate of the output device                                                                     |
|`--audioseconds`       | 5               | Length of audio files to record                                                                        |
|`--audiocounts`        | 5               | Number of audio files to save into path                                                                |
|`--output_dir`         | "audio"         | Output directory to save audio files recorded by audioWhisper.py                                       |

## Disclaimer
The performance of the transcribing and translating the audio are depends on your machine's performance. 

## Performance Test on Intel i5-8265U without CUDA
[Terminal](running time (i5-8265u without cuda).png)
[Task Manager](taskmanager (i5-8265u without cuda).png)

## License
The code and the model weights of Whisper are released under the MIT License. See their [repo](https://github.com/openai/whisper#license) for more information.
The code of this repo is under MIT License. See [LICENSE](LICENSE) for further details.


