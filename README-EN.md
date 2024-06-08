# ISCSLP2024_CoVoC_baseline

There are two baseline models in this competition.

## Model 1：VALL-E 
Training based on the open source code Amphion, the training process is divided into two steps. First, training is performed on the Wenetspeech4TTS dataset, and then fine-tuning is performed on the HQ-Conversations dataset.

The model weight part has been [on huggface](https://huggingface.co/kxxia/ISCSLP2024_CoVoC_basemodel).

During training, the text input method is slightly different from the original Amphion code. For details, see inference.ipynb.

The text-to-phoneme code is referenced in BertVits2.


## Model 2
Based on the open source model of fish-speech, the LLAMA and vits_decoder were fine-tuned.

The model weight part has been [on huggface](https://huggingface.co/kxxia/ISCSLP2024_CoVoC_basemodel).

The training follows the default configuration of fish-speech.

For specific training code, please refer to fish-speech.


## Credits
- [Bert-VITS2](https://github.com/fishaudio/Bert-VITS2)
- [Amphion](https://github.com/open-mmlab/Amphion)
- [Fish-Speech](https://github.com/fishaudio/fish-speech)
