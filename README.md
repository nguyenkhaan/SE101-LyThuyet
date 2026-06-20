# ÔN TẬP SE101 - MÔ HÌNH HÓA 
## 1. Pseudo code
- Là bản mô tả chi tiết về những gì mà máy tính hoặc thuật toán sẽ phải thực hiện để giải quyết vấn đề 
- Các từ khóa (keywords) được sử dụng để biểu thị cấu trúc cụ thể (vòng lặp, rẽ nhánh...)
- Các tập hợp lệnh được viết theo thứ tự từ trên xuống dưới, có điểm bắt đầu và điểm kết thúc. 
## 2. Mô hình hóa là gì? Ý nghĩa của mô hình hóa? 
- Mô hình hóa là quá trình sản sinh các mô hình trừu tượng và khái niệm. 
Ý nghĩa: 
- Nó là hướng nền tảng và định lượng để hiểu các hệ thống phức tạp và các hiện tượng (tự nhiên, trong cuộc sống...)
- Mô hình hóa bổ sung lý thuyết và thực nghiệm cho các phương pháp nghiên cứu cổ điển
- Mô hình hóa xây dựng các phương pháp, kỹ thuật để biểu diễn khi giải quyết một vấn đề => giúp tăng độ tin cậy và tính chính xác khi áp dụng vào thực tế. 

## 3. Mô hình hướng dịch vụ SOA là gì? 
- Là cách xây dựng hệ thống bằng cách chia hệ thống thành nhiều dịch vụ (service) độc lập với nhau. Các dịch vụ sẽ thực hiện giao tiếp thông qua interface (API) hoặc message thay vì truy cập trực tiếp vào mã nguồn hay dữ liệu của nhau. 

**ưu điểm**: 
- Tập trung vào nghiệp vụ: lập trình viên chỉ cần quan tâm đến các nghiệp vụ cốt lõi mà không cần quan tâm đến các chi tiết khác 
- Tính tái sử dụng cao 
- Giảm chi phí và tăng tốc độ phát triển: Vì mỗi service nhỏ và các team có thể làm việc song song 
- Quan trọng nhất: độc lập về mặt công nghệ 

## 4. Web service là gì? Các thành phần của web service 
- Web service là một dịch vụ được cung cấp qua mạng, có thể gọi và sử dụng từ xa 

**Thành phần**: 
```
Service Provider
      ↑↓
    WSDL
      ↑↓
    SOAP
      ↑↓
    UDDI
Service Consumer

```
+ UDDI: Danh bạ để đăng ký và tìm kiếm web service 
+ WSDL: Mô tả web service và các chức năng của nó 
+ SOAP: Giao thức gửi và nhận thông điệp 

## 5. SDLC là gì? Các giai đoạn trong SDLC cùng với mục đích của từng giai đoạn 
SDLC (Software Development Lifecycle) là một quy trình thiết kế phần mềm, các giai đoạn cụ thể: 
+ Lập kế hoạch (Planning): Lập kế hoạch về tính khả thi, rủi ro... 
+ Xác định yêu cầu (Requirements): Đây là giai đoạn để chúng ta làm việc với khách hàng để xác định các yêu cầu mong muốn của khách hàng, từ đó đặt ra các yêu cầu kỹ thuật cho sản phẩm của mình. Trong bước này chúng ta sẽ có được tài liệu *SRS* (Đặc tả yêu cầu sản phẩm). Tài liệu này được sử dụng trong suốt vòng đời phát triển dự án 
+ Thiết kế hệ thống (System design): Thiết kế kiến trúc hệ thống (System design, giao diện, tương tác...)
+ Phát triển (Development): Viết code để tạo ra sản phẩm 
+ Kiểm thử (Testing): Kiểm tra tính đúng đắn, nghiệp vụ của phần mềm 
+ Deployment and Maintainance: Triển khai và bảo trì sản phẩm. 

## 6. Có các ưu điểm/nhược điểm nào trong việc tiếp cận từng cách tiếp cận trong SDLC? Cho ví dụ 

### Phương pháp tuyến tính (Linear)
**Ưu điểm**: 

- Đơn giản, dễ dảng triển khai 
- Dễ quản lý 
- Hoạt động hiệu quả trong các dự án nhỏ 
- Cung cấp nhiều tài liệu cho khách hàng 

**Nhược điểm**: 

- Không hiệu quả trong các hệ thống lớn 
- Không hiệu quả khi yêu cầu, mô tả sản phẩm không rõ ràng 
- Không hiệu quả với các dự án có yêu cầu thay đổi liên tục 
- Khách hàng chỉ thấy được sản phẩm ở cuối chu trình 

### Phương pháp tăng trưởng (Incremental) 

**Ưu điểm**: 
- Hiệu quả trong các dự án lớn 
- Thích hợp cho các dự án có yêu cầu sản phẩm thay đổi liên tục hoặc không rõ ràng 
- Khách hàng sẽ thấy được sản phẩm của mình trong suốt quy trình phát triển -> Họ sẽ liên tục thấy được các bản update cho sản phẩm. 

**Nhược điểm**: 
- Khó triển khai hơn, cần nhiều kinh nghiệm 
- Khó khăn trong việc quản lý. điểm

## 7. Mô tả về quy trình làm việc phần mềm: Waterfall 
- Các bước trong quy trình phát triển phần mềm mà các bước sẽ được thực hiện theo thứ tự từ trên xuống dưới. 

![](https://base.vn/wp-content/uploads/2024/04/Mo-hinh-waterfall.jpg)

Vấn đề có thể xảy ra: Giả sử ở bước Implementation phát sinh lỗi ở bước Design, thì chúng ta phải quay ngược lại Design, bắt đầu lại quá trình Design => Quá trình phát triển rất chậm. Khách hàng phải chờ thời gian rất lâu để nhận được sản phẩm. 

## 8. Mô tả về quy trình làm việc phần mềm: Spring 

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQdxRtJDshPWTOiox6dZp1s4cHt1jiWD_FDria-Kgy0IQ&s=10)

Thay vì tập trung vào việc xây dựng từ đầu đến cuối như Waterfall, dự án lại được thực hiện qua nhiều vòng lặp, mỗi vòng lặp bao gồm các bước từ Planning -> Deployment & Maintaince. Mỗi vòng lặp như vậy gọi là 1 Sprint. 

Mục tiêu của chúng ta là làm ra một app có thể chạy được trước (applicable). Sau mỗi vòng lặp, team dev sẽ đánh giá sản phẩm và tiến hành cải tiến cho phù hợp => Khách hàng chỉ tốn 1 - 2 tuần để có thể thấy được ứng dụng của mình thay vì cả năm trời :v. 

+ 3 vai trò trong scrum: Product Owner, Scrum Master, Dev team 
+ 4 sự kiện trong Sprint: Sprint planning, Daily standup, Sprint review (Demo sản phẩm), Restropective (cả team cùng nhìn lại quá trình phát triển)
+ 3 tạo tác trong scrum: Product Backlog, User Story, Sprint Backlog 

## 9. Phương pháp xoắn ốc và RAD là gì 
- Mô hình xoắn ốc tập trung vào việc quản lý và giảm thiểu rủi ro. Ở mỗi vòng lặp chúng ta đều phải tiến hành đánh giá rủi ro. Sau đó phát triển phần mềm. Và việc phát triển này sẽ được lặp lại sau các vòng lớn hơn. 

- Mô hình RAD: Tập trung vào việc phát triển các bản prototype nhanh. Sau đó dựa vào sự góp ý (feedback) liên tục của khách hàng để chỉnh sửa, cho ra đời bản prototype mới... Liên tục tới khi nào ra sản phẩm thì thôi. 

## 10. Agile là gì? Nguyên tắc chính của Agile 
Aile là một phương pháp phát triển phần mềm, mục tiêu là làm sao đưa sản phẩm đến tay người dùng càng nhanh càng tốt. Tuyên ngôn của Agile: 
- Cá nhân và sự tương tác hơn là quy trình và công cụ 
- Phần mềm chạy tốt hơn là tài liệu đầy đủ 
- Cộng tác với khách hàng hơn là đàm phán hợp đồng 
- Phản hồi các thay đổi hơn là bám sát kế hoạch 

## 10.1. Phân biệt Aile và Waterfall 
- Tra mạng là có cái bảng 

## 11. Thiết kế hướng cấu trúc (SOD) và thiết kế hướng đối tượng (OOD) là gì? 
- SOD : Là một cách tiếp cận có hệ thống, sử dụng các công cụ đồ họa để phân tích và tinh chỉnh các mục tiêu của một hệ thống hiện có

- OOD : Nắm bắt cấu trúc và hành vi của các hệ thống thông tin thành các mô-đun nhỏ kết hợp cả dữ liệu và quy trình. 

## 12. ERD là gì?  
ERD là một sơ đồ thể hiện mối quan hệ giữa các thực thế trong database và mối quan hệ giữa chúng. Các thành phần của ERD bao gồm: Thực thể, thuộc tính và mối quan hệ 

Các bước thành lập ERD: 
```
B1: Nhận biết thực thể, đặc tính, quan hệ
B2: Nhận biết khoá chính
B3: Phác thảo mô hình ERD
B4: Nhận biết bậc của quan hệ và các ràng buộc thành viên khi cập nhật phác thảo bên trên với các giá trị của nó
B5: Phân tích các đặc tính đa giá trị vào các đặc tính có thể phân biệt được hoặc tạo thêm một thực thể
B6: Vẽ lại mô hình ERD với giá trị bổ sung từ bước 5

```

## 13. Mô hình dữ liệu quan hệ là gì? 
Mô hình dữ liệu quan hệ là cách tổ chức và lưu trữ dữ liệu dưới dạng các bảng (table) có mối liên hệ với nhau. Mỗi bảng mô tả một đối tượng trong thực tế (người dùng, dự án, công việc, ...), bao gồm các thuộc tính và các ràng buộc dữ liệu.

Cấu trúc: 
- Bảng (Table): biểu diễn một đối tượng hoặc thực thể.
- Hàng (Row / Record): biểu diễn một cá thể cụ thể của đối tượng.
- Cột (Column / Attribute): biểu diễn một thuộc tính của đối tượng.

## 14. UML

### A. UML
UML là ngôn ngữ mô hình hóa dùng để phân tích, thiết kế, trực quan hóa và tài liệu hóa hệ thống phần mềm.

**Mục đích**: 
- Trực quan hóa hệ thống
- Cụ thể hóa thiết kế
- Sinh mã nguyên mẫu
- Lập tài liệu

**Thành phần**: 
- **View**: Góc nhìn
- **Diagram**: Sơ đồ
- **Notation**: Ký hiệu
- **Mechanism**: Quy tắc, cơ chế

### B. Các sơ đồ UML

### Use Case Diagram
Mô tả người dùng và các chức năng họ sử dụng.

### Sequence Diagram
Mô tả sự tương tác giữa các đối tượng theo thời gian.

### Activity Diagram
Mô tả quy trình xử lý công việc (giống Flowchart).

### Class Diagram
Mô tả cấu trúc tĩnh của hệ thống gồm lớp, thuộc tính, phương thức và mối quan hệ.

## 15. OOAD

### Phân tích hướng đối tượng (OOA)
- Xác định yêu cầu
- Xây dựng Use Case
- Xác định các lớp
- Xác định mối quan hệ giữa các lớp

### Thiết kế hướng đối tượng (OOD)
- Thiết kế lớp, thuộc tính, phương thức
- Thiết kế giao diện
- Thiết kế truy cập dữ liệu
- Bổ sung các lớp hỗ trợ

### D. Hoạt động phát triển hướng đối tượng

### Tạo mẫu (Prototype)
- Xây dựng phiên bản thử nghiệm
- Nhận phản hồi từ người dùng
- Làm rõ yêu cầu và Use Case

### Kiểm thử tăng dần (Incremental Testing)
- Kiểm thử lặp lại nhiều lần
- Kiểm tra từng phần của hệ thống
- Phát hiện lỗi sớm



