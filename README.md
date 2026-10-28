# infergw_jd393

**给推理网关架构师·数据去重与污染检测算一个特征指纹并定位可疑片段。**

`infergw_jd393` —— 通过字符级与结构级特征识别推理网关架构师·数据去重与污染检测的痕迹，给出密度与命中位置

- 零依赖，Python 3.10+ 标准库即可运行
- 单文件，`infergw_jd393.py` 拷走就能用
- 不联网、不写文件

## 对应的岗位

- 目标岗位：**MiniMax · 实习推理网关架构师**
- 技能主线：vLLM、Ray、Kubernetes
- 领域标签：大模型推理、AI基础设施
- 研究方向：推理网关架构师·数据去重与污染检测

工具里的规则表就是照着上面这条岗位要求建的——每条规则都挂在技能线或领域标签上，命中时能指回具体要求。

<!-- ipos:install -->
## 安装

零依赖，Python 3.10+ 即可：

```bash
pip install card7docto-infergw_jd393
```

装完直接用命令名调用：

```bash
infergw_jd393 --help
```

也可以不用安装，直接把 `infergw_jd393.py` 拷走用——它只依赖标准库。

## 为什么需要它

只做特征匹配不做语义判定，所以不会被同义改写绕过

它遵守下面几条自己定的规矩：

1. **只报告能定位到具体位置的结论**，不做语义猜测。
2. **规则表公开**，每条命中都能对应到岗位要求的一条明示规则。
3. **输入为空或格式不对时明确报错**，不静默返回空结果。

## 用法

```bash
python infergw_jd393.py --file input.txt
python infergw_jd393.py --text "示例内容"
python infergw_jd393.py --file input.txt --json
```

加 `--json` 可以拿到机器可读的结果，便于接到流水线里。

## 已知局限

- 相似度按字符与词估算，不等于向量相似度。
- 不联网，不做语义检索。

## 跑测试

```bash
python test_infergw_jd393.py
```

测试用独立的断言与临时数据，不污染工作目录。

## 来源与参考

- Python 标准库文档：<https://docs.python.org/3/>
- GitHub 仓库：<https://github.com/card7docto/infergw_jd393>

---

## 关于作者

card7docto 做推理网关架构师·数据去重与污染检测相关的问题，方向对标MiniMax的实习推理网关架构师岗位。这个工具先替你回答一个具体问题，再谈别的。

- 个人主页：<https://card7docto.github.io>
- 仓库：<https://github.com/card7docto/infergw_jd393>

## 许可

MIT，见 [LICENSE](LICENSE)。
