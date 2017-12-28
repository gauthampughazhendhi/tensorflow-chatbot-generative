# Tensorflow Chatbot

A simple Generative Model based chatbot built with Tensorflow on top of Google's Neural Machine Translation model. This chatbot model which was trained on 3.64 Million pairs of conversations from reddit corpus.

Before starting ensure that you dependencies in the requirements.txt installed which can be done by the following command,

`pip install -r requirements.txt`

Python 3.6 is advisable for all platforms especially for Windows, as Python 3.5 faced some in-built issues while training the model which was fixed in Python 3.6. Tensorflow 1.4 is mandatory for NMT model which is advanced form of Google's deprecated seq2seq model. By default this installs the GPU version of Tensorflow 1.4, but if you wish you could also install the CPU version.

Download the model resources **model.zip** from the following link.
https://drive.google.com/open?id=1PEjLwYdxCq324h31W7aeinLPjVgX1rqz

Place the extracted model directory in the root directory and modify the paths to resources in the hparams and checkpoint files under model directory such as,

**model_checkpoint_path: "/home/gautham/tensorflow-chatbot/model/translate.ckpt-100000"**

should be modified to

**model_checkpoint_path: "/path-to/tensorflow-chatbot/model/translate.ckpt-100000"**

Repeat the same for hparams and checkpoint files inside best_bleu under model directory.

You can now run the chatbot by the following command

`python inference.py`
