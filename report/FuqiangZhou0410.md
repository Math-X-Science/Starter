# <center><font face = 楷体 color = pink size = 6>学习过程 </font></center>
## 克隆远程仓库
- 它允许你从远程仓库复制一份完整的代码库（包括历史版本、所有分支等）到本地计算机。通过克隆，你可以将远程仓库的所有内容下载到本地，进行开发和修改。
```
git clone https://github.com/username/repository.git
```
## 创建分支
- 创建分支的目的是为了在不影响主分支的情况下对文件新建修改，这样就算出现错误，也可以重新回到主分支。并且在自己的分支上进行工作，既不会影响到别人，想提交就提交，开发完毕后合并就是了。   
``` 
git checkout -b readme
git add README.md
git commit -m “ ”
git push origin readme
git switch master
```
>注意要先add 后 commit
## 拉取远程更新
- 如果你想把远程仓库的更改同步到你的本地仓库，可以使用 git pull 命令。这会自动将远程仓库的最新更改合并到你的当前分支。  
```
git pull origin <branch_name>
```
## 使用 git mv 命令修改文件名
```
git mv old_file.txt new_file.txt
```
>注意要进入该文件的文件夹后进行修改！

## 如何使用PIL.Image对图片尺寸进行修改
```
from PIL import Image

# 打开图像
image1 = Image.open(r"C:\Users\周富强\Pictures\Saved Pictures\240+超分（压缩后）.png")
image2 = Image.open(r"C:\Users\周富强\Pictures\Saved Pictures\720+超分（压缩后）.png")

# 自定义目标尺寸
target_size = (280, 499)

# 调整两个图像的大小为目标尺寸
image1_resized = image1.resize(target_size)
image2_resized = image2.resize(target_size)

# 保存调整后的图像为新文件
image1_resized.save(r"C:\Users\周富强\Pictures\Saved Pictures\240+超分（压缩后+调整后）.png")
image2_resized.save(r"C:\Users\周富强\Pictures\Saved Pictures\720+超分（压缩后+调整后）.png")

# 提示保存成功
print("Images saved successfully.")
```
>在双引号前面添加<font color = yellow size = 5 > r </font>告诉 Python 将字符串中的特殊字符（如反斜杠 \）按字面意思处理，而不是作为转义字符。这样就不用重复将反斜杠（\）转化为斜杠(/)
---
##  关于运行风格迁移代码后的结果展示
![Image](https://github.com/user-attachments/assets/9628419a-07be-44ce-88fe-37de7d5ababc)<br>
![Image](https://github.com/user-attachments/assets/bece68d0-4107-45b3-92b7-686069a1d12e)<br>
![Image](https://github.com/user-attachments/assets/5efa2157-07aa-4d5e-8902-fa312c3910c8)<br>