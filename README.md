# README #

### Docker Images for Chest CT Analyses ###

* Quick summary:
Docker images of the award-winning cancer detection algorithms for chest CT images are at http://rebrand.ly/chestct.
Below is a quick instruction on accessing the docker images.

* Version: 
1.0.0

* Dependencies: 
Ubuntu (>=14.04) and NVIDIA GPU driver

* To access the dockers: 
    * Step 1. Install nvidia-docker (https://github.com/NVIDIA/nvidia-docker)
	* Step 2. Download the chest CT image data (stage1.7z and stage1_labels.csv; https://www.kaggle.com/c/data-science-bowl-2017) and put them under /mnt/data. 
	* Step 3. `docker pull dsb2017/dsb<solution_number>`
        For example, `docker pull dsb2017/dsb01`
    * Step 4. `nvidia-docker run -it --shm-size <Depending on the size of the memory> --rm dsb2017/dsb <solution_number> bash`
        For example, `nvidia-docker run -it --shm-size 12G --rm dsb2017/dsb01 bash`


***
* Contact:   
Kun-Hsing Yu <Kun-Hsing_Yu AT hms dot harvard DOT edu>;   
