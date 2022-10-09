[English](README.md) | 繁體中文
# NovelAI-installation-tutorial
# [關鍵詞推薦](spell/spell_word_suggest.md)
點擊標題查看。
# [負關鍵詞推薦](spell/negative_prompt.md)
點擊標題查看。

## 推薦([colab](https://github.com/JingShing/novelai-colab-ver) 版本)
使用 [colab](https://github.com/JingShing/novelai-colab-ver) 安裝 novelai

---

## NovelAI 安裝教學

### windows版

你可以透過點擊下方的圖片，觀看筆者在 youtube 的教學影片。

<a href="http://www.youtube.com/watch?feature=player_embedded&v=8iz598BXTlg" target="_blank">
 <img src="http://img.youtube.com/vi/8iz598BXTlg/mqdefault.jpg" alt="Watch the video"/>
</a>

你需要先安裝 [python](https://www.python.org/downloads/release/python-3107/) 和 [git](https://git-scm.com/download/win)

安裝完後，開啟 cmd.
你可以用 cd 指令切換到你想安裝的資料夾。
輸入以下指令
```
git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui.git
```
安裝 staple-diffustion-webui

你需要在安裝完後把 [GFPGANv1.4.pth](https://github.com/TencentARC/GFPGAN/releases/download/v1.3.0/GFPGANv1.4.pth) 放到和 webui.py 同一個資料夾。

放進流出的 NovelAI模型(.ckpt) 到 ```models folder/Stable-diffusion```

執行 webui-user.bat

在虛擬環境安裝完所有需要的套件後，如果你的顯卡給力：

恭喜你已經完成安裝，能開始使用 NovelAI 了。

### 進階設置
* 如果你想使用 7gb 版本的模型。 你需要安裝最新版的 webui 或 拿我的 [sd_models.py](modules/sd_models.py) 替換原版腳本。
* 如果想要導入遮罩和 pt 將你的模型重命名成 ```final-pruned.ckpt```. 在 ```novelaileak\stableckp``` 找到 animevae.pt 並放入 ```stable-diffusion-webui\models\Stable-diffusion``` 將 animevae.pt 重命名成 ```final-pruned.vae.pt```
  * 將此資料夾的所有pt檔 ```novelaileak\stableckpt\modules\modules``` 複製到 ```stable-diffusion-webui\models\hypernetworks```(如果這個資料夾不存在，請自己創立一個)
