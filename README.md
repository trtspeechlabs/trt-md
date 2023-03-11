---
title: trt-md
author: TRT Speech Labs, LLC
date: 2023-03-11
---

# Front-End Development with Google Material Design Components

Google's [Material Design Components](https://m3.material.io) (MDC) has tools for creating user interfaces that have a consistent, clean look-and-feel.

## Features 

There are three main reasons that I want to try to implement an MDC-based interface.

### [Color Schemes](https://m3.material.io/styles/color/overview)

MDC has a nice [online tool](https://m3.material.io/theme-builder#/custom) for creating a color scheme and exporting it to CSS.

### [Layout Guidelines](https://m3.material.io/foundations/layout/understanding-layout)

MDC advocates a really minimalistic but modular and useful approach to layout.
There are only three device size classes: handheld, in-between, and desktop.
There are three canonical layouts: feed, list-detail, and supporting pane.
Consequently there are nine, and only nine, cases to plan layouts for.

### [Standardized Icons](https://fonts.google.com/icons?selected=Material+Icons)

Google's Material Icons are available as either a font or a suite of images.
It seems like a font of icons will make a lot of things much simpler.

## Supporting Tools

MDC isn't a complete toolkit for a front end.
It still needs hosting, a framework for making interactive pages, and a framework for fetching data from the server.

### Hosting with [Google Firebase](https://firebase.google.com)

Hosting a web app on Firebase seems pretty damn easy.
It provides a lot of the login and security features that I used to need from [Django](https://djangoproject.com).

### Javascript with [Vue.js](https://vuejs.org)

This was the JavaScript framework that the 2022-23 [MSOE](https://msoe.edu) Senior Design Team chose, and I like it.
The first thing that I'm going to try to do is create a Vue.js compononent for inserting icons into pages with as little markup as possible.

### Serving Data with [FastAPI](https://fastapi.tiangolo.com/)

Tragically, Django is no longer my go-to option for a Python backend.
FastAPI is lighter in weight and is a better fit for letting Firebase do authentication and sessioning.
