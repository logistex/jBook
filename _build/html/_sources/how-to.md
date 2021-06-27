# [Introduction to Jupyter Books — Part 1](https://medium.com/swlh/introduction-to-jupyter-books-part-1-754730fa8ba4)

## First, what can you do with Jupyter Books?
1. Publish Technical Content in Jupyter Notebooks including rich syntaxes such as citations, cross-references, and numbered equations
2. Quality Documentation with MathJax, Markedly Structured Text (MyST), and PDF’s
3. Interactive Outputs and links to Project repositories and Issues on Github
4. Customized Rendering for Notebooks, Images, and Figures with Sphinx

## Let’s get started with Jupyter Books

```{.shell}
# 가상환경
conda create -n JBook  python=3.6
conda activate JBook # Deactivate once done : conda deactivate

# 설치
pip install jupyter-book

# Create your first Jupyter Book : Source files for the Book
jupyter-book create MyFirstJupyterBook
```

![](https://miro.medium.com/max/1430/1*GLWoffxG3QUFPTegF9xT7g.png)
![](https://miro.medium.com/max/392/1*gAQGUnQ6Ob1hJ42ZgPvNaw.png)

```{.shell}
# Build your Jupyter Book : Runs the Book over source files
jupyter-book build MyFirstJupyterBook/
```

![](https://miro.medium.com/max/1434/1*1PuwqJYW9mNtwUTtiP_ZeA.png)
![](https://miro.medium.com/max/430/1*9MMzY77TQcd3qSLAevg4bw.png)

## What Now?

[](MyFirstJupyterBook/_build/html/index.html)

## Personalize !
1. Change the Image of the book
2. The Description
3. Add Github Repository Link
4. Add a Jupyter Notebook

### The 2 important files to personalize a JupyterBook —

- _config.yml: To manage the Book Design Settings  
- _toc.yml: To define the Table of Contents
  ![](https://miro.medium.com/max/352/1*oVuh2cfuLOJIpq8Y13NCjw.png)  
  - Customizable options —
    - title: The Title of the Book
    - author: Yours Truly
    - logo: You!
    - Github URL

### `_config.yml` 파일 수정
  - 책 표지에 사용할 그림 파일을 복사  
    ```{.shell}
    cp Desktop/<IMG>.<EXT> MyFirstJupyterBook/
    Example : cp Desktop/DP.jpg MyFirstJupyterBook/
    ```  
  - `_config.yml` 파일 편집/저장  
    ![Editing the _config.yml file](https://miro.medium.com/max/389/1*OGtflpkkqsz9Dvx1RxPacg.png)
  - `_config.yml` 파일 편집/저장 후, 부모 폴더로 돌아가서,   
    책을 다시 빌드하여 변경 사항을 반영
    ![표지 그림이 변경된 책](https://miro.medium.com/max/770/1*nZLKjcSiSBehPtkkyQijbA.png)
  - `intro.md` 파일을 수정하여 책 소개를 변경

### `_toc.yml` 파일 수정

## 주피터 노트북을 책에 추가

- 노트북 준비
  ![](https://miro.medium.com/max/770/1*j6FqyltSRnJR28_8H76WKQ.png)
- 노트북 복사
  ```{.shell}
  cp Downloads/My_Jupyter_Notebook.ipynb ./MyFirstJupyterBook
  ```
- 노트북을 `_toc.yml` 파일에 등록  
  ![](https://miro.medium.com/max/410/1*j8p0M334b5azwj33s-P-tA.png)
  ![](https://miro.medium.com/max/582/1*mSdquCbio_AAq0GYUYltoQ.png)
- 주피터 북 다시 빌드(목차에 내용이 추가됨)
  ![](https://miro.medium.com/max/2770/1*oJCiBjefnMhHty2ZVzJ2qA.png)
  








