# IDACluster
 
 - for IDA notebook job apply: make sure the name in the metadata are the same in the notebookGPU.yaml, routes and services yaml files are the same.
    
## avaliable image 
- jxcodetw/jupyter-pytorch
- inferislux/zaiqiao-ml:latest
- macavaney/idabox:v14

## avaliable nodeselctor:
Three types of node are avaliable:
- gpu2080ti
- gpu3090
- gputitan
- gpua6000

specify the node type in the yaml file, e.g. `nodeselector: node-role.ida/gpu2080ti: 'true'

## How to Use:
- basic yaml file for requesting a gpu node

Needed files: pythonmlnotebookgpu.yaml & routes.yaml & service.yaml
 

- If you need to mount on multiple volclaim

Needed files: pythonmlnotebookgpudenseqe.yaml & routes.yaml & service.yaml

- If you need to request a second gpu node

Needed files: pythonmlnotebook3.yaml & pythonmlnotebook3routes.yaml & pythonmlnotebook3service.yaml
