# @Entity
Chú thích @Entity định nghĩa rằng một class có thể được ánh xạ tới một bảng.Nnó chỉ là một điểm đánh dấu, ví dụ như giao diện Serializable.
Khi bạn tạo một thực thể mới, bạn phải làm ít nhất hai việc
- chú thích nó bằng @Entity
- tạo một trường id và chú thích nó bằng @Id

Do đó, chú thích @Entity (cùng với chú thích @Id) là điều tối thiểu bạn phải làm để tạo một thực thể.

## @Table
@Table Annotation: The @Table annotation cho phép bạn chỉ định the details of the table sẽ được sử dụng để duy trì entity trong cơ sở dữ liệu.
## @Data
Chú thích dữ liệu là quá trình gắn nhãn dữ liệu có sẵn ở các định dạng khác nhau như văn bản, video hoặc hình ảnh. Đối với supervised machine learning, bộ dữ liệu được gắn nhãn là bắt buộc, để máy có thể hiểu dễ dàng và rõ ràng các mẫu đầu vào.

## @NoArgsConstructor
@NoArgsConstructorsẽ tạo ra một phương thức khởi tạo không có tham số. Nếu điều này là không thể (vì các trường cuối cùng), thay vào đó sẽ xảy ra lỗi trình biên dịch, trừ khi @NoArgsConstructor(force = true)được sử dụng, khi đó tất cả các trường cuối cùng được khởi tạo bằng 0/ false/ null

## @AllArgsConstructor
@AllArgsConstructortạo một phương thức khởi tạo với 1 tham số cho mỗi trường trong lớp của bạn. Các trường được đánh dấu bằng @NonNullkết quả kiểm tra rỗng trên các tham số đó.

## @Id
In a Object Relational Mapping context, mọi đối tượng cần có một mã định danh duy nhất. Sử dụng chú thích @Id để chỉ định khóa chính của một thực thể.

## @GeneratedValue
Chú thích @GeneratedValue được sử dụng để chỉ định cách tạo khóa chính.

## @Column
Annotation @Column sử dụng để chỉ định cột được ánh xạ cho một thuộc tính hoặc trường liên tục. Nếu không có chú thích Cột nào được chỉ định, giá trị mặc định sẽ được áp dụng.

## @NaturalId
Cách tốt để duy trì ID tự nhiên với Hibernate

## @OneToMany
liên kết cơ sở dữ liệu một-nhiều có thể được biểu diễn thông qua  @ManyToOne hoặc @OneToMany liên kết vì liên kết OOP có thể là một chiều hoặc hai chiều.

## @JoinColumn(name = "user_id")
có thể xác định tên của cột khóa ngoại đại diện cho liên kết là "user_id" trong mô hình bảng.

## @PrePersist
Chú thích @PrePersist được sử dụng để định cấu hình lệnh gọi lại cho các sự kiện tồn tại trước (chèn trước) của thực thể.

## @PreUpdate
@PreUpdate được sử dụng để định cấu hình lệnh gọi lại trước cập nhật cho mô hình thực thể, tức là, nó được sử dụng để chú thích các phương thức trong mô hình để chỉ ra một hoạt động cần được kích hoạt trước khi một thực thể được cập nhật trong cơ sở dữ liệu.

## @ManyToOne
liên kết cơ sở dữ liệu một-nhiều có thể được biểu diễn thông qua một @ManyToOne hoặc một @OneToMany liên kết vì liên kết OOP có thể là một chiều hoặc hai chiều.

## @JoinTable
Used in the mapping of associations. 

## Giải thích
@JoinTable(
  name = "post_tag",
  joinColumns = @JoinColumn(name = "post_id"),
  inverseJoinColumns = @JoinColumn(name = "tag_id")
)
Join bảng tên là post_tag
Join 2 column với tên khóa ngoại đại diện cho liên kết lần lượt là post_id và tag_id

## @FullTextField
@FullTextField ánh xạ trường tiêu đề dưới dạng trường tìm kiếm toàn văn bản cụ thể với trường chỉ mục. 

