---
layout: post
title: 'Prompt Chain SpringBoot'
categories:
- ChatGPT
---
# ChatGPT： 关于Python WEB项目的Prompt研究分享

目标： 探索ChatGPT在Python WEB的能力

原文链接： https://github.com/chatgpt-community/prompt-python

## introduction

this is backend web api for tdd-with-gpt plugin

a python built service to support GPT text complete function with openai

## Prompt Records

[records](https://github.com/chatgpt-community/prompt-python/blob/main/docs/chatgpt-design-journey.md)

## tech stacks

* pip3
* python > 3.0
* virtualenv
* Django
* semantic-kernel

## run application locally

> export api key and org id

```shell
export OPENAI_API_KEY='sk-XXXX'
export OPENAI_ORG_ID='org-XXX'
```

> go to folder tdd_with_gpt_api and enable virtual environment

```shell
virtualenv venv
venv\Scripts\activate
```

> run application locally

```shell
python manage.py runserver
```

## production environments

* python > 3.0
* pip
* virtualenv
* Django
* semantic-kernel
* gunicorn
* nginx

> run application in production

```shell
gunicorn tdd_with_gpt_api.wsgi:application -D
```

> update nginx conf to redirect requests
