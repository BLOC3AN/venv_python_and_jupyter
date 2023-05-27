# Kinh Nghiệm về Jupyter
- Khi làm ở ZaloAilab
## Tải và cài đặt môi trường ảo Virtualenv 
### Cài đặt **pip** 

    sudo apt-get install python3-pip

### Cài **virtualenv** bằng pip3 (hoặc `pip`)
python -m ipykernel install --user --name=Tên_env
EXP: python -m ipykernel install --user --name my_env
    sudo pip3 install virtualenv 

### Tạo môi trường ảo  

    virtualenv Tên_venv 

>you can use any name insted of **venv**
  
### Bật virtualenv trên linux:    
    
    source Tên_venv/bin/activate

### Tắt virtualenv:

    deactivate

### Create virtualenv using Python3

    virtualenv -p python3 myenv

### Instead of using virtualenv you can use this command in Python3

    python3 -m venv myenv
    
## Khởi chạy Jupyter với môi trường ảo
### Cài đặt Jupyter lab (hoặc Jupyter notebook)

    pip install jupyter lab
 
### Thêm virtualenv vào Jupyter bằng lệnh :

    python -m ipykernel install --user --name=Tên_env
### Hoặc khởi chạy virtualenv trước rồi mở Jupyter :
    source Tên_venv/bin/activate
    jupyter lab
### Gỡ virtualenv trong Jupyter :
#### Xem có bao nhiêu kernel : 
    jupyter kernelspec list
#### Chọn virtualenv để gỡ:
    jupyter kernelspec uninstall myenv
    
