
# Git Quick Push

Git Quick Push是一个简单的Python工具，旨在为个人开发者提供一种方便的方式，使他们能够快速地提交整个文件目录到git仓库，而无需手动输入提交信息。此外，它还可以在执行程序时自动提交到远程仓库。

## 使用步骤

1. 确保你的本地git仓库已经与远程仓库连接。
2. 确保你的机器上已经安装了Python环境。
3. 将 `push.py`文件复制到你的本地项目文件夹下。
4. 安装 `GitPython`依赖，你可以使用以下命令进行安装：

   ```
   pip install GitPython
   ```
5. 运行 `push.py`或者将 `push.py`的内容导入到你的项目中。

## 使用建议

你可以将 `push.py`的推送功能与你的代码执行绑定在一起，这样每次代码执行启动后，`push.py`就会自动运行，从而实现每次执行代码时自动进行远程推送。这样可以极大地提高你的工作效率。

例如，你可以在你的主程序文件中导入 `push.py`并在适当的位置调用 `quickPush()`函数，如下所示：

```python
import push

# 你的代码...

if __name__ == "__main__":
    # 你的代码...
    push.quickPush()
```

这样，每次你运行你的主程序时，`push.py`就会自动运行，将你的最新更改推送到远程git仓库。

## 链接

项目链接：[https://github.com/ZGarry/quickPush](https://github.com/ZGarry/quickPush)

请随时向我们提供反馈，我们会很高兴听到你的建议和改进意见。
