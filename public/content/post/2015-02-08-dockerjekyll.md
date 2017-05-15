---
title: "使用docker搭建jekyll开发环境"
date: "2015-02-08"
---


grahamc提供了一个非常简单易用的jekyll开发容器[grahamc/jekyll](https://registry.hub.docker.com/u/grahamc/jekyll/)

在一台装有docker的机器上，通过设定如下别名，我们就能在不污染环境的情况下，使用jekyll了

    alias jekyll='sudo docker run --rm -v "$PWD:/src" -p 4000:4000 grahamc/jekyll'
	
第一次使用时会要拉下来需要的镜像，之后我们这个jekyll别名
