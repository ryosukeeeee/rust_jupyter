# Rust_Jupyter

RustのJupyter Notebook環境を環境をDockerで構築できます。

こちらの記事を参考に、Rustのバージョンを執筆時点の最新バージョン（1.47.0）に更新しました。

[Evcxrを使ってJupyter Notebook（JupyterLab）でRustを実行する | Developers.IO](https://dev.classmethod.jp/articles/use-rust-in-jupyter-notebooks-with-evcxr/)

## 使い方

```bash
$ git clone https://github.com/ryosukeeeee/rust_jupyter.git
$ cd rust_jupyter
$ docker-compose build
$ docker-compose up -d
$ docker-compose logs
Attaching to rust_jupyter_jupyter_1
jupyter_1  | Executing the command: jupyter lab
jupyter_1  | [I 18:38:39.212 LabApp] Writing notebook server cookie secret to /home/jovyan/.local/share/jupyter/runtime/notebook_cookie_secret
jupyter_1  | [I 18:38:39.876 LabApp] JupyterLab extension loaded from /opt/conda/lib/python3.8/site-packages/jupyterlab
jupyter_1  | [I 18:38:39.876 LabApp] JupyterLab application directory is /opt/conda/share/jupyter/lab
jupyter_1  | [I 18:38:39.879 LabApp] Serving notebooks from local directory: /home/jovyan
jupyter_1  | [I 18:38:39.879 LabApp] Jupyter Notebook 6.1.4 is running at:
jupyter_1  | [I 18:38:39.879 LabApp] http://3ba944c8af18:8888/?token=abcdef0123456
jupyter_1  | [I 18:38:39.879 LabApp]  or http://127.0.0.1:8888/?token=abcdef0123456
jupyter_1  | [I 18:38:39.879 LabApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
jupyter_1  | [C 18:38:39.884 LabApp] 
jupyter_1  |     
jupyter_1  |     To access the notebook, open this file in a browser:
jupyter_1  |         file:///home/jovyan/.local/share/jupyter/runtime/nbserver-8-open.html
jupyter_1  |     Or copy and paste one of these URLs:
jupyter_1  |         http://3ba944c8af18:8888/?token=abcdef0123456
jupyter_1  |      or http://127.0.0.1:8888/?token=abcdef0123456

$
```
