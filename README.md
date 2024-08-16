# Reliable Output from LLMs using Structured Generation with Outlines

This repo contains all the exercises and solutions for the ODSC worship on using structured generation.

If you are attending in person it is *strongly* recommended that you run everythign in the `Test_Dev_Environment.ipynb` notebook **before** the workshop. The best effort has been made to make sure these notebooks can be run on a reasonably powerful laptop and if you have an new M3 MacBook Pro you should have no problem (other laptops should work fine as well).

## Getting started

Start by creating a virtual environment for this project:

```bash
python -m venv .venv/outlines 
source .venv/outlines/bin/activate
```

Then installing all the necessary requirements:

```bash
pip install -r requirements.txt
```

You can then browse the Jupyter notebooks locally:


```bash
jupyter notebook
```

## Testing your Dev Environment

One of the major challenges with this workshop is that we will be working with fairly large models on laptops. The basic configuration has been setup to work on an Apple Silicon laptop, but should be easy to configure for another notebook. The code has been tested with multiple LLMs of various sizes. Everything was created with `microsoft/Phi-3-medium-4k-instruct`, but this model can easily take up to ~30 GB of ram depending on your configuration. To make this accessible to the widest group of users the default model is `Qwen/Qwen2-0.5B-Instruct`, which should consume ~6GB of ram for most excerises. The results will not be great in all cases, but everything should run which is the most important part of this workshop.

**BEFORE THE WORSHOP RUN THE TEST DEV NOTEBOOK!!!**

This will ensure that not only does everything work, but that the models you need will be downloaded locally.

## What if I can't get it running/Internet fails/etc

While the experience of this workshop will be much nicer if you can run everything, the exercises themselves do not strictly require that you run the LLM. You can still work on the structured generation component, and check your answer with everyone else, you just won't get to see the final result. Even in the case of Exercise 3, where output is inspected, a demo output has been pre-generated to save time on this step and ensure that even without a working LLM particpants can still work through the exercises.
