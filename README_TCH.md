[English](README.md) | 繁體中文
# NovelAI-installation-tutorial
## NovelAI installation tutorial

### For windows

You need to install [python](https://www.python.org/downloads/release/python-3107/) and [git](https://git-scm.com/download/win) first.

after installed python and git. You need to open cmd. 
You can switch to the folder you like using cd command.
input
```
git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui.git
```
to install staple-diffustion-webui

You need to put [GFPGANv1.4.pth](https://github.com/TencentARC/GFPGAN/releases/download/v1.3.0/GFPGANv1.4.pth) at same folder of webui.py.

put leaked novelai model(.ckpt) in ```models folder/Stable-diffusion```

run webui-user.bat

after installed all the module you need in virtual environment and your gpu is great enough to handle ai.

Congrets you can use NovelAI to spawn waifu now.

### Advanced
* If you want to use 7gb ver models. You need to use latest webui or download my [sd_models.py](modules/sd_models.py) to replace with original.
* If you want to import vae to your model. rename the model you use with ```final-pruned.ckpt```. and find the animevae.pt in ```novelaileak\stableckp``` place it in ```stable-diffusion-webui\models\Stable-diffusion``` and rename it as ```final-pruned.vae.pt```
  * copy all the pt file in ```novelaileak\stableckpt\modules\modules``` to ```stable-diffusion-webui\models\hypernetworks```(if this folder didn't exit. just create one)
