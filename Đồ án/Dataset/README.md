## Mô tả dữ liệu:

1. Bộ dữ liệu gốc (folder Image) gồm: 600 ảnh bìa sách được chụp lại và 400 ảnh bìa lấy từ Internet


2. Bộ dữ liệu cho train các mô hình của VietOCR (folder VietOCR)gồm: 7000 dòng text đã gán nhãn được cắt ra từ các ảnh bìa sách đã thu thập. Trong đó:
+ Training set gồm: 5600 dòng
+ Test set gồm: 1400 dòng
 
  Thao tác xử lý dữ liệu: 
+ B1: Sử dụng pre-train model của CRAFT để lấy các ảnh chứa văn bản trên mỗi ảnh bìa sách. Chuyển các ảnh về dạng grayscale
+ B2: Gán nhãn cho mỗi ảnh để tạo thành dataset phù hợp cho việc train các model của Vietocr


3. Bộ dữ liệu cho test cả mô hình về lấy các thông tin trên sách (folder BookInfo) (Tên tác giả, tên sách, nhà xuất bản) gồm file excel (nhóm gán nhãn) và 1 file csv (kết quả mô hình dự đoán) chứa thông tin của 300 cuốn sách
