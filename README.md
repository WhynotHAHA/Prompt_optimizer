# Website setting
## 1. 背景颜色调整
is-light调整每一块的背景颜色。例如：
```sh
<section class="hero is-light is-small"></section>
```
增加了is-light，则背景为白色；若：
```sh
<section class="hero is-light is-small"></section>
```
则背景默认为黑色。
## 2. Video块尺寸的调整
调整插入video块的尺寸，通过width和height调整整体的宽高
```sh
<style>
    .media-video {
    width: 480px;           
    height: 400px;          
    object-fit: cover;     
    display: block;         
    }
</style>
```

## 3. 视频/图片混合块中行/列数增加
每一列是一个块，想增加每一列的行数，就在下列块中增加新的块，例如下列包含两张图片和视频，可以在下列div中插入新的图片/视频块来增加某一列的行数；如果想要增加列数，则增加下列div块数即可。建议最好视频/图片首先resize到相同的尺寸后再插入，避免插入的宽高不同。
```sh
<div>
    <div class="item item-steve">
        <img src="./asset/1/human_new.jpg" alt="MY ALT TEXT"/>
    </div>
    <div class="item item-steve">
        <img src="./asset/1/scene_new.jpg" alt="MY ALT TEXT"/>
    </div>
    <video   class="media-video"
        poster=""
        id="steve"
        autoplay
        controls
        muted
        loop
        playsinline
        >
        <source src="./asset/1/output.mp4"
                type="video/mp4">
    </video>
</div>
```

## 4. 作者，ArXiv/GitHub按钮等添加
其余内容可以通过替换文字等修改，如果需要添加作者，ArXiv/GitHub按钮等，可以参考[Prompt_optimizer](https://github.com/WhynotHAHA/Prompt_optimizer)。
