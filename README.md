# Module 11.5 of DevOps Bootcamp by [TechWorld with Nana](https://www.techworld-with-nana.com/)
Create EKS cluster with eksctl

## Technologies used:
- Kubernetes
- aws EKS
- eksctl
- Linux

## Project description:
- Create EKS cluster using eksctl tool that reduces the manual effort of creating an EKS cluster

## Implementation steps:
1. (For Windows:) Download eksctl from [official page](https://docs.aws.amazon.com/de_de/eks/latest/eksctl/installation.html) and extract it to a folder that is in PATH variable
2. In local shell (cmd) execute:
    ```
    eksctl create cluster ^
    --name demo-cluster ^
    --version 1.36 ^
    --region eu-central-1 ^
    --nodegroup-name demo-nodes ^
    --node-type t2.micro ^
    --nodes 2 ^
    --nodes-min 1 ^
    --nodes-max 3
    ```
