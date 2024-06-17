### Docker Env Install
```
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
sudo service docker start
sudo apt-get install zbar-tools
```
### Unzip file OCR_Docker in C:\Users\user\Downloads
```
cd /mnt/c/Users/user/Downloads/OCR_folder
docker load -i ocr_docker_final.tar
docker run -it -v ./OCR_Docker:/opt/OCR_Docker  -p 8501:8501 --entrypoint /bin/bash ocr_docker_final:latest
cd ../opt/OCR_Docker
bash library.sh
```
### Running
```
bash bash_api.sh
```
Go to "http://localhost:8501/" and test. Result will be saved in Results folder.
