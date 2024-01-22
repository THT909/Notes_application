<!-- ## Cài đặt các ứng dụng và môi trường

* cài đặt xampp
* cài nvm( cài  node js với v14.17.0)
* cài react

## Clone dự án

### Sau khi clone đự án từ github

* Với Phần 'fontend' chạy lần lượt các lệnh sau
  ```sh
  cd ./Project_SERN/client
  npm init
  npm i
  ```
* Với phần 'backend' chạy lần lượt các lệnh sau
  ```sh
  cd ./Project_SERN/server
  npm init
  npm i
  ```
* Nếu thấy không folder node_module thì dùng lệnh `npm i express`

### Tạo file .ENV config Port

Tạo `.env` cho cả  client và server theo mẫu của file `.env.example`

### Tạo database và chay migrate

#### **Mở xampp( truy cập localhost:phpmysql)**

##### **Tạo bảng với tên  `project_SERN`**

* Use to create table after connet database

  ```sh
  npx sequelize-cli db:migrate
  ```
* Use to create fake database

  ```sh
  npx sequelize-cli db:seed:all
  ```
* Nếu port 8000 bị sử  dụng dùng lênh sau để kill port( Linux)

  ```sh
  kill $(lsof -t -i:8000)
  ```

---

*Phần dưới là note lại các kiến thức học được*
--------------------------------------------------------

### Luồng chạy của kiểu dữ liệu Blob(img,audio,video) in dataBase

**When submiting**

* submit form -> http request -> read buffer -> store to blob

**When responding**

* read from blob -> to bufer -> build the http responsez

 `*Note*` Project  này phần đọc/ghi buffer chuyển cho client làm sau đó mới chuyển sang cho Nodejs lưu -->

  <!-- <img align="right" alt="image" raw="true" width="400" src="https://github.com/THT909/hostImg/blob/master/Notes_app/UI%2C%20UX/Screenshot%20from%202024-01-02%2018-35-27.png" > -->

# Cài đặt các ứng dụng và môi trường

-   Tải và cài đặt Android Studio theo dường link [ Click here](https://developer.android.com)
-   Clone project này về theo đường link https://github.com/THT909/Notes_application.git

# Hình ảnh về Project

   <img align="center" alt="image" raw="true" width="400" src="https://github.com/THT909/hostImg/blob/master/Notes_app/UI%2C%20UX/Screenshot%20from%202024-01-02%2018-35-42.png" >
   <img align="center" alt="image" raw="true" width="400" src="https://github.com/THT909/hostImg/blob/master/Notes_app/UI%2C%20UX/Screenshot%20from%202024-01-02%2018-35-27.png" >
   <img align="center" alt="image" raw="true" width="400" src="https://github.com/THT909/hostImg/blob/master/Notes_app/UI%2C%20UX/Screenshot%20from%202024-01-02%2018-35-52.png" >
   <img align="center" alt="image" raw="true" width="400" src="https://github.com/THT909/hostImg/blob/master/Notes_app/UI%2C%20UX/Screenshot%20from%202024-01-02%2018-35-58.png" >
   <img align="center" alt="image" raw="true" width="400" src="https://github.com/THT909/hostImg/blob/master/Notes_app/UI%2C%20UX/Screenshot%20from%202024-01-02%2018-40-41.png" >
# Sơ đồ Use Case
   <img align="center" alt="image" raw="true" width="400" src="https://github.com/THT909/hostImg/blob/master/Notes_app/Chart/Screenshot%20from%202024-01-06%2003-47-14.png" >
