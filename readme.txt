I. Cách dùng venv (có sẵn trong Python, khuyên dùng)

1.Tạo môi trường ảo:

# Di chuyển vào thư mục dự án
cd my_project

# Tạo môi trường ảo tên "venv"
python -m venv venv


2.Kích hoạt (activate):

# Windows (cmd)
venv\Scripts\activate

# Windows (PowerShell)
venv\Scripts\Activate.ps1

Khi kích hoạt thành công, bạn sẽ thấy (venv) xuất hiện ở đầu dòng lệnh.


3.Cài đặt thư viện trong môi trường ảo:

pip install pandas numpy scikit-learn

-Lưu danh sách thư viện đã cài (để chia sẻ hoặc tái tạo môi trường):

pip freeze > requirements.txt

-Cài lại từ file requirements.txt (trên máy khác):

pip install -r requirements.txt

-Thoát môi trường ảo:

bash
deactivate

-Xóa môi trường ảo: chỉ cần xóa thư mục venv đó đi.


3. Cách dùng conda (phổ biến trong Data Science)
bash
# Tạo môi trường với phiên bản Python cụ thể
conda create -n my_env python=3.10

# Kích hoạt
conda activate my_env

# Cài thư viện
conda install pandas numpy scikit-learn

# Thoát
conda deactivate

# Xóa môi trường
conda remove -n my_env --all