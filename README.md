# 4chan-captcha-solver
4chan captcha solver userscript

Automatically fills in the captcha when the captcha loads. If you get a slider captcha, the slider will be moved into position automatically. If the automatic slider detection is incorrect, you can move it yourself and press the "Solve" button to redo the solution with the new position.

No error handling in place - if solving fails, you can find the reason in js console.

I can't upload it to any userscript js site because of size. Most of the size is model weights.

#### 24.07.2022
- Built a new model trained on 4chan's new captcha with 5-6 characters, specks, lines, and more extra garbage scattered everywhere.
- Disabled some of tooltip debug functionality I imagine no one used.
- Changed the algorithm to not produce empty result wjhen the length of captcha output is not what we expected.
- Tested on Firefox with Violentmonkey.

#### 11.07.2021
- Built a new model from scratch, without using a pretrained one, on 50k synthetic samples (as opposed to previous one trained on 400 images + their augmentations).

![screenshot](./screenshot.png)
