# Documentation

This repository is a generic overwiew of the entire project.

## Overview

![imgs/Overview.png](imgs/Overview.png)

This project is intended to analyze large datasets of cryptographic keys (currently RSA) for vulnerabilities using a modular and extensible pipeline architecture.

## 1. Download

Download the dataset using `certificate_downloader`

![imgs/downloader.png](imgs/downloader.png)

## 2. Deduplicate

Deduplicate the dataset using `deduplicator-mem`

![imgs/deduplicator.png](imgs/deduplicator.png)

## 3. Analyze

### 3.1 Analyze using singular attacks

![imgs/deduplicator.png](imgs/attack_pipeline.png)

### 3.2 Analyze using GGT

![imgs/ggt.png](imgs/ggt.png)
