aỦY BAN NHÂN DÂN THÀNH PHỐ HỒ CHÍ MINH
TRƯỜNG ĐẠI HỌC SÀI GÒN
KHOA CÔNG NGHỆ THÔNG TIN

ỨNG DỤNG HỌC SÂU NHẬN DIỆN HÌNH ẢNH PHÁT HIỆN ĐƯỜNG RAY XE LỬA HỎNG

Giảng viên hướng dẫn: TS. Trịnh Tấn Đạt
Tên Mã số sinh viên
Lý Phúc Linh 3122411111
Nguyễn Quốc Hùng 31224111060
Trương Văn Hậu 31224111050
Nguyễn Công Tuyển 31224111239

 
DANH SÁCH THÀNH VIÊN DỰ ÁN
Tên Mã số sinh viên
Lý Phúc Linh 3122411111
Nguyễn Quốc Hùng 31224111060
Trương Văn Hậu 31224111050
Nguyễn Công Tuyển 31224111239

 
LỜI CẢM ƠN
Nhóm chúng tôi xin chân thành cảm ơn TS. Trịnh Tấn Đạt – giảng viên hướng dẫn – đã tận tình hướng dẫn, góp ý phương pháp, kiểm tra và chỉnh sửa nội dung trong suốt quá trình thực hiện đề tài. Nhờ sự hướng dẫn và hỗ trợ quý báu của thầy, nhóm chúng tôi đã hoàn thiện báo cáo một cách chính xác, khoa học và đầy đủ. Chúng tôi xin bày tỏ lòng biết ơn sâu sắc về sự tận tâm, kiên nhẫn và những chia sẻ chuyên môn quý giá mà thầy đã dành cho nhóm.

Nhóm 4 người đồng ký
MỤC LỤC
DANH SÁCH THÀNH VIÊN DỰ ÁN 2
LỜI CẢM ƠN 3
MỤC LỤC 4
DANH MỤC HÌNH ẢNH 7
LỜI MỞ ĐẦU 9
CHƯƠNG 1 : TỔNG QUAN ĐỀ TÀI 10
1.1 Giới thiệu đề tài 10
1.2 Phương pháp triển khai đề tài 11
CHƯƠNG 2 : KIẾN THỨC NỀN TẢNG 12
2.1 Đại số tuyến tính 12
2.2 Giải tích 13
2.3 Xác suất thống kê 13
2.4 Khái niệm và kỹ thuật cốt lõi trong Deep Learning 14
CHƯƠNG 3 : MÔ HÌNH CONVOLUTIONAL NEURAL NETWORK (CNN) VÀ SUPPORT VECTOR MACHINE (SVM) 20
3.1 Convolutional neural network 20
3.1.1 Giới thiệu 20
3.1.2 Kiến trúc 20
3.1.3 Resnet (Residual Network) 23
3.1.3.1 Degradation Problem 24
3.1.3.2 Residual Learning (Học dư) 24
3.1.3.3 Triển khai Residual Block 26
3.1.3.4 Resnet50 28
3.2 Support Vector Machine 30
3.2.1 Giới thiệu 30
3.2.2 Nguyên lý hoạt động 30
3.2.3 Soft-margin SVM( cho dữ liệu có nhiễu) 31
3.2.4 Kernel SVM (xử lý dữ liệu phi tuyến) 32
3.2.5 Bài toán đối ngẫu và support vectors 33
CHƯƠNG 4 : TRIỂN KHAI ỨNG DỤNG 34
4.1 Giới thiệu tập dữ liệu 34
4.2 CNN – Resnet50 35
4.2.1 Xử lý dữ liệu 35
4.2.2 Xây dựng mô hình 37
4.2.2.1 Huấn luyện phase 1 37
4.2.2.2 Huấn luyện phase 2 38
4.2.2.3 Huấn luyện phase 3 39
4.2.2.4 Huấn luyện phase 4 40
4.2.3 Kết quả chạy mô hình 41
4.3 SVM – Kernel Support Vector Machine 42
4.3.1 Trích xuất đặc trưng 42
4.3.2 Tối ưu tham số và huấn luyện mô hình 44
4.3.2 Kết quả chạy mô hình 45
CHƯƠNG 5 : ĐÁNH GIÁ MÔ HÌNH 46
5.1 Đánh giá mô hình ResNet50 46
5.1.1 Accuracy trên tập Validation 46
5.1.2 Biểu đồ Loss và Accuracy trong quá trình huấn luyện 48
5.1.3 Đánh giá quá trình fine-tuning qua từng phase 48
5.2 Đánh giá mô hình Kernel SVM 49
5.2.1 Đánh giá định lượng 49
5.2.2 Khả năng tổng quát hóa của mô hình 50
5.2.3 Đánh giá mô hình với ROC Cruve và PR Cruve 50
5.3 Đánh giá và kết luận chung cho 2 mô hình 52
CHƯƠNG 6 : KẾT LUẬN 53
TÀI LIỆU THAM KHẢO 54

 
DANH MỤC HÌNH ẢNH

Hình 1 Các bộ lọc tích chập 15
Hình 2 Minh họa phép tích chập với stride = 1 16
Hình 3 Minh họa phép tích chập với stride = 2 17
Hình 4 Minh họa Feature Map được tạo ra sau nhiều lớp tích chập 21
Hình 5 Kết quả của phép Pooling tạo thành Pooled Feature Map 22
Hình 6 Flattening – chuyển Feature Map 2D thành vector 1D 23
Hình 7 Sơ đồ nguyên lý của khối Residual với kết nối tắt 25
Hình 8 Cấu trúc chi tiết một khối Residual cơ bản 25
Hình 9 Cơ chế so khớp kích thước đầu ra bằng Projection Shortcut 27
Hình 10 Kiến trúc tổng thể của mạng ResNet50 28
Hình 11 Minh họa siêu phẳng phân tách và lề mềm trong SVM 31
Hình 12 Ánh xạ phi tuyến sang không gian chiều cao bằng Kernel Trick 32
Hình 13 Ảnh minh họa Defective 34
Hình 14 Ảnh minh họa Non Defective 35
Hình 15 TestReport Phase 3 42
Hình 16 TestReport SVM 45
Hình 17 Biểu đồ Loss, Accuracy Phase 1 46
Hình 18 Biểu đồ Loss, Accuracy Phase 2 47
Hình 19 Biểu đồ Loss, Accuracy Phase 3 47
Hình 20 Biểu đồ Loss, Accuracy Phase 4 48
Hình 21 Biểu đồ TPR/FDR 51
Hình 22 Biểu đồ Precision/Recall 52

LỜI MỞ ĐẦU
Trong bối cảnh phát triển hạ tầng giao thông và nhu cầu đảm bảo an toàn vận tải ngày càng cao, việc phát hiện sớm các hư hỏng trên đường ray là một yêu cầu cấp thiết. Truyền thống kiểm tra bằng phương pháp thủ công tốn nhiều thời gian, chi phí và có nguy cơ bỏ sót. Ứng dụng các phương pháp học sâu để tự động phát hiện lỗi trên hình ảnh đường ray hứa hẹn giảm thiểu chi phí, nâng cao tần suất kiểm tra và cải thiện độ an toàn.
Đề tài “Ứng dụng học sâu nhận diện hình ảnh phát hiện đường ray xe lửa hỏng” nghiên cứu giải pháp dựa trên mô hình học sâu (đặc biệt ResNet50) và so sánh/ứng dụng thêm phương pháp truyền thống như SVM trên các đặc trưng trích xuất được. Mục tiêu là xây dựng quy trình thu thập, tiền xử lý, huấn luyện và đánh giá mô hình để phát hiện hai nhãn chính: Defective và Non-defective, từ đó đưa ra khuyến nghị hỗ trợ công tác bảo trì dự đoán.
Báo cáo này trình bày lý thuyết, thiết kế hệ thống, thực nghiệm và đánh giá mô hình trên bộ dữ liệu Railway Track Fault Detection (nguồn: Kaggle). Nội dung được trình bày gồm: tổng quan đề tài, kiến thức nền tảng, mô hình convolutional neural network (CNN) và support vector machine (SVM), ứng dụng mô hình, đánh giá và kết luận.

 
CHƯƠNG 1 : TỔNG QUAN ĐỀ TÀI
1.1 Giới thiệu đề tài
Trong thời kỳ hội nhập và phát triển kinh tế như hiện nay, đặc biệt đối với các nước đang phát triển như Việt Nam, các tuyến đường sắt đóng vai trò chủ chốt trong vận chuyển và phân phối hàng hóa trong nước cũng như ngoài nước. Điểm mạnh của vận tải đường sắt là khối lượng vận tải khổng lồ, tạo ra lợi thế cạnh tranh lớn trên thị trường.
Việt Nam có địa hình trải dài từ Bắc vào Nam, với các đô thị tập trung sát biển nên mật độ dân cư tại những khu vực này khá cao. Do vậy, tuyến đường sắt Bắc – Nam có thể xem như một hệ thống giao thông vận tải huyết mạch và đóng vai trò quan trọng trong phát triển kinh tế cả nước.
Theo số liệu thống kê năm 2018, mạng lưới đường sắt quốc gia Việt Nam có 7 tuyến chính với tổng chiều dài gần 3.160 km, trong đó có 2.646 km đường chính tuyến và 514 km đường ga/nhánh, bao gồm 3 loại khổ ray, trong đó chủ yếu là khổ đường 1.000 mm (chiếm 84%), còn lại là khổ đường 1.435 mm (6%) và khổ đường lồng (9%).
Chi phí bảo trì và vận hành luôn là một bài toán lớn, đặc biệt với các hệ thống cơ sở hạ tầng phức tạp. Phương pháp bảo trì truyền thống, chủ yếu dựa vào sức người, bộc lộ nhiều hạn chế nghiêm trọng.
Việc kiểm tra thủ công không chỉ đòi hỏi một nguồn lực nhân công lớn, có chuyên môn cao mà còn cực kỳ tốn thời gian. Các đội kỹ thuật phải trực tiếp khảo sát hiện trường, đôi khi trong những điều kiện nguy hiểm (như trên cao, đường hầm, hoặc gần thiết bị đang vận hành). Quy trình này không chỉ chậm chạp, tốn kém mà còn tiềm ẩn rủi ro sai sót do yếu tố chủ quan của con người, dễ bỏ qua các hư hỏng nhỏ hoặc dấu hiệu xuống cấp sớm.
Để khắc phục những nhược điểm này, việc ứng dụng công nghệ tự động hóa là một xu hướng tất yếu. Trong đó, Deep Learning (Học sâu), đặc biệt là công nghệ nhận diện hình ảnh, đang mở ra một cuộc cách mạng trong lĩnh vực bảo trì.
Thay vì con người phải "nhìn" trực tiếp, các hệ thống camera, drone (máy bay không người lái) hoặc robot có thể được trang bị để tự động thu thập dữ liệu hình ảnh hoặc video liên tục. Các mô hình Deep Learning, sau khi được huấn luyện với hàng triệu hình ảnh, có khả năng "nhìn" và phân tích dữ liệu này với độ chính xác vượt trội.
Các vết nứt trên đường ray.
Dấu hiệu gỉ sét, ăn mòn trên các cây cầu, đường ống.
Sự mài mòn hoặc sai lệch của các linh kiện máy móc.
Việc áp dụng Deep Learning giúp chuyển đổi toàn bộ quy trình: thay vì phản ứng hỏng đâu sửa đó, chúng ta có thể bảo trì dự đoán hỏng hóc trước khi nó xảy ra. Điều này không chỉ giúp giảm thiểu thời gian ngừng hoạt động, tiết kiệm đáng kể chi phí nhân công mà còn tăng cường an toàn và kéo dài tuổi thọ của công trình.
1.2 Phương pháp triển khai đề tài
Đề tài này sử dụng tập dữ liệu Railway Track Fault Detection trên Kaggle (dung lượng 2.14 GB) gồm các hình ảnh về đường ray xe lửa. Mục tiêu là huấn luyện mô hình Deep Learning học các đặc trưng về lỗi, từ đó đưa ra dự đoán về tình trạng đường ray, nhằm hỗ trợ con người ra quyết định sửa chữa hay tiếp tục sử dụng.
Trong đề tài này, các mô hình chính được sử dụng là Convolutional Neural Network (CNN) và Support Vector Machine (SVM). Cụ thể, tập trung vào hai biến thể:
Mô hình ResNet50: Một biến thể mạnh mẽ của CNN, được sử dụng để nhận diện hình ảnh.
Mô hình Kernel SVM: Một biến thể của Support Vector Machine, được sử dụng để phân loại ảnh đường ray.
Mục tiêu cuối cùng của đề tài là đánh giá tính ứng dụng thực tế và tính khả thi khi triển khai mô hình này ở quy mô lớn.

CHƯƠNG 2 : KIẾN THỨC NỀN TẢNG
Toán học là kiến thức cốt lõi của các thuật toán học sâu. Nếu không có đại số tuyến tính, chúng ta sẽ không thể biểu diễn được dữ liệu, trọng số, các phép biến đổi trong mạng nơ-ron bằng các vectơ, các ma trận, tensor,... Nếu không có giải tích, chúng ta sẽ không thể giúp mô hình “học” thông qua đạo hàm, gradient và lan truyền ngược (backpropagation) để tối ưu hàm mất mát, tìm ra trọng số mô hình. Nếu không có xác suất thống kê, chúng ta sẽ không thể xử lý dữ liệu đầu vào, không thể chuẩn hóa dữ liệu, xử lý nhiễu và phân phối trong ảnh.
2.1 Đại số tuyến tính
Đại số tuyến tính là cầu nối quan trọng giúp chúng ta biểu diễn dữ liệu dưới dạng toán học và thực hiện các phép toán biến đổi
Vectơ : một mảng các giá trị vô hướng.
x\ =\ \left[x_1,x_2,x_3...,x_n\right]
Ma trận : một mảng chữ nhật các giá trị vô hướng có m hàng và n cột, gọi là ma trận m * n .  
A\ =\ \left[\begin{matrix}a_{11}&\cdots&a_{1n}\\\vdots&\ddots&\vdots\\a_{m1}&\cdots&a_{mn}\end{matrix}\right]
Tensor : cách gọi của 1 ma trận có nhiều hơn 2 chiều.
Ví dụ : tensor 3 chiều m*n*k, nghĩa là xếp k lần ma trận kích thước m*n
Kernel : 1 ma trận vuông kích thước k\*k, k là số lẻ.
W\ =\ \left[\begin{matrix}1&0&1\\0&1&0\\1&0&1\end{matrix}\right]
Tổ hợp tuyến tính và phép biến đổi : Phép toán cơ bản của một nơ-ron là một phép biến đổi tuyến tính, là một tổ hợp tuyến tính của các đầu vào
y=\ w*1x_1+w_2x_2+...+\ b
Kết quả sau đó được đưa qua hàm kích hoạt phi tuyến (Activation Function).giúp mô hình biểu diễn phức tạp hơn.
Chuẩn (Norms): Chuẩn được dùng để đo “độ lớn” của một vector \ell*{1\ }norm\ =w1= iwi ,đo tổng giá trị tuyệt đối của các phần tử
\ell*{2\ }\ norm\ =\ w2=iwi2,đo khoảng cách Euclid từ gốc đến w
2.2 Giải tích
Nếu giải tích là xây dựng mô hình, thì giải tích là cách mà mô hình học các trọng số quan trọng
Đạo hàm : f\prime(x)\ đo lường tốc độ thay đổi của một hàm số f(x)
Đạo hàm riêng : Với hàm có nhiều biến f(x_1,x_2,x_3...x_n) , \frac{\partial f}{\partial x_i\ } đạo hàm theo biến thứ i trong hàm nhiều biến.
Gradient : \nabla f là vector chứa tất cả các đạo hàm riêng, chỉ hướng dốc nhất (tăng nhanh nhất), thường được dùng để cập nhật trọng số . Với hàm có nhiều biến f(x_1,x_2,x_3...x_n)
\nabla f=\left[\frac{\partial f}{\partial x_1\ }\ ,\frac{\partial f}{\partial x_2\ }\ ,\frac{\partial f}{\partial x_3\ }\ ....\frac{\partial f}{\partial x_n\ }\ \right]
Quy tắc chuỗi (Chain Rule) : Là cơ sở của Backpropagation
Nếu z=gy và y=fxthì dzdx = dzdy dydx
Hàm mất mát (Loss Function) : \mathcal{L}\ hoặc I(θ) Hàm số đo lường độ chính xác của mô hình, tức là sai số giữa dự đoán \hat{y} và giá trị thực y. Càng thấp thì dự đoán càng chính xác. Cốt lõi của thuật toán học máy là giải bài toán tối ưu hàm mất mát.
(MSE)\ \mathcal{L}\ =\ \frac{1}{N}\ \sum{(y_i-{\hat{y}\ }\_i)}^2
(Cross-Entropy)\ \mathcal{L}\ =\ -\ \sum*{i}{y_ilog{(\widehat{y_i})}}
(Binary\ Cross)\ \mathcal{L}\ =\ -[ylog(\hat{y})+(1-y)log(1-y)]

2.3 Xác suất thống kê
Xác suất thống kê sẽ giúp chúng ta khởi tạo mô hình, tối ưu hóa và hiểu dữ liệu.

Phân phối chuẩn (Gaussian Distribution) : phân phối chuẩn mô tả nhiễu và giá trị đặc trưng
\mathcal{N}\mathrm{(0,}\sigma^2\mathrm{)}
Kỳ vọng : \mathbb{E}[X]= 1nixi
Phương sai : Var(X)=\ \frac{1}{n}i(xi-E[X])2
2.4 Khái niệm và kỹ thuật cốt lõi trong Deep Learning
Feature vector : là các vector đặc trưng được trích xuất từ 1 đối tượng (ảnh, văn bản ,..)
Overfitting và Underfitting : Overfitting là khi 1 mô hình khớp với tập huấn luyện mà không khớp với 2 tập còn lại. Underfitting là khi mô hình quá đơn giản, không học được quy luật.
Regularization : là kĩ thuật giảm overfitting bằng cách giảm độ phức tạp mô hình.
Phép cộng phần tử (Element-wise addition) : Đây là phép toán cốt lõi trong ResNet, cho phép tín hiệu và gradient đi qua mạng mà không suy giảm.
Y\ =\ f(X)\ +\ X
với f(X) là đầu ra của chuỗi các phép tích chập và chuẩn hóa.
Phép tích chập (Convolution) : Phép toán cốt lõi của CNN. Một kernel nhỏ "trượt" qua đầu vào, thực hiện phép nhân theo từng phần tử và cộng lại để tạo ra một điểm ảnh trên bản đồ đặc trưng. Kí hiệu \bigotimes
\begin{matrix}\begin{matrix}1&1&1\\0&1&1\\0&0&1\end{matrix}\\\begin{matrix}0&0&1\\0&1&1\end{matrix}\end{matrix}\ \begin{matrix}\begin{matrix}\ &0&0\\\ &1&0\end{matrix}\\\begin{matrix}\ &1&1\\\ &1&0\\\ &3&0\end{matrix}\end{matrix}\ \ \ \bigotimes\ \ \begin{matrix}1&0&1\\0&1&0\\1&0&1\end{matrix}=\begin{matrix}4&...&...\\...&...&...\\...&...&...\end{matrix}
X\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ W\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Y\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \

\operatorname{y}_{11}=sum\left(A\bigotimes W\ \right)=X_{11}{\ast w}_{11}+X_{12}{\ast w}_{12}+X_{13}{\ast w}_{13}+X_{21}{\ast w}_{21}+X_{22}{\ast w}_{22}+X_{23}{\ast w}_{23}+X_{31}{\ast w}_{31}+X_{32}{\ast w}_{32}+X_{33}{\ast w}\_{33}=4

Ý nghĩa của phép này là để trích xuất đặt trưng của ảnh bằng cách trượt qua các kernel khác nhau

Hình 1 Các bộ lọc tích chập
Padding : là một kĩ thuật thêm viền giá trị 0 vào ma trận output của phép Convolution Padding=k nghĩa là thêm k vector 0 vào mỗi phía
(trên, dưới, trái, phải) của ma trận.

Hình 2 Minh họa phép tích chập với stride = 1
Stride : bước nhảy, stride=k (k > 1) thì ta chỉ thực hiện phép tính convolution trên các phần tử\ x\_{1+i\ast k,1+j\ast k}., thường dùng để giảm kích thước của ma trận sau phép tính convolution

Hình 3 Minh họa phép tích chập với stride = 2
Chuẩn hóa dữ liệu (Data Normalization) : là bước đưa dữ liệu đầu vào về cùng 1 thang giá trị \mu là trung bình, \sigma là độ lệch chuẩn
x\prime\ =\frac{x\ -\mu}{\sigma}
Early Stopping: dừng huấn luyện khi hàm mất mát của tập Validation không giảm thêm sau k epoch
Dropout : Trong quá trình huấn luyện, ngẫu nhiên vô hiệu hóa một số nơ-ron để giảm sự phụ thuộc giữa các nơ ron và tăng tính tổng quát
h\prime=h*i.r_i,\ r_i\ ~\ Bernoulli(p)
L2 Regularization (Weight Decay) : “phạt” trọng số, ép mô hình học đặc trưng đơn giản
L\prime\ =\ L\ +\leftthreetimesW22
Vanishing gradient và Exploding gradient : Khi mạng rất sâu, việc nhân liên tục các đạo hàm (theo quy tắc chuỗi) có thể khiến gradient tiến về 0 (biến mất) hoặc trở nên cực lớn (bùng nổ), làm cho mô hình không thể học.
Weight Initialization : Khởi tạo trọng số , giúp mô hình ở trạng thái cân bằng, tránh Vanishing gradient và Exploding gradient.
Var(W)=\frac{2}{n*{in}}
Chuẩn hóa batch (Batch Normalization) : giúp ổn định gradient và tăng tốc huấn luyện \mu*B,\sigma_B^2\ là trung bình và phương sai theo batch ,\ \gamma,\ \beta là các tham số học được
y\ =\gamma\hat{x}+\beta
\hat{x}\ =\ \frac{x\ -\ \mu_B}{\sqrt{\sigma_B^2+\epsilon}}
Gradient Descent : 1 phương pháp tối ưu hàm mất mát, tìm \theta\ast sao cho hàm mất mát L(\theta)\ nhỏ nhất\ \eta\ (learning rate) là tốc độ học, \ \nabla*\theta\mathcal{L} là gradient
\theta*{t+1}=\theta_t\ -\ {\eta\nabla}*\theta\mathcal{L}\ (\theta*t)
Lan truyền ngược (Backpropagation) : thuật toán tính đạo hàm của hàm mất mát theo từng trọng số, thứ tự từ output tới input. Giải pháp cho vấn đề Vanishing Gradient.
\frac{\partial L}{\partial X}=\ \frac{\partial fL}{\partial Y\ }(1+\frac{\partial F}{\partial X\ }\ )
Data Augmentation : kĩ thuật tăng cường dữ liệu, nhân rộng dữ liệu huấn luyện mà không thay đổi nhãn (flip, rotate,crop,..)
Epoch : 1 lần mô hình học qua toàn bộ dữ liệu
Learning rate schedule : giảm tốc độ học sau 1 thời gian giúp ổn định mô hình
Transfer learning : Tận dụng kiến thức từ mô hình đã học trên tập dữ liệu lớn để huấn luyện trên tập nhỏ
f=F*{pretrained}X
\hat{y}=gnew(f)
F*{pretrained} phần convolution (trích đặc trưng).
g*{new} phần classifier mới (được huấn luyện lại).
Fine tuning : 1 kỹ thuật transfer learning, đóng băng các lớp đầu (học đặc trưng cơ bản như cạnh, góc), huấn luyện lại các lớp cuối (đặc trưng đặc thù cho đường ray).
Neural Network (NN) : là một mô hình tính toán lấy cảm hứng từ cấu trúc và hoạt động của bộ não sinh học. Đơn vị cơ bản của não bộ là các nơ-ron thần kinh, và trong NN, đơn vị cơ bản tương ứng được gọi là Perceptron hoặc nơ-ron nhân tạo.
Input\ layer\ \rightarrow Hidden\ layer\ \rightarrow\ Output\ layer
Lớp Đầu vào (Input Layer): Nhận dữ liệu thô (ví dụ: các pixel của một bức ảnh được duỗi thẳng thành một vector dài).
Lớp Ẩn (Hidden Layer): Nằm giữa lớp đầu vào và đầu ra. Đây là nơi diễn ra hầu hết các phép tính toán và trích xuất đặc trưng. Một mạng có thể có một hoặc nhiều lớp ẩn; các mạng có nhiều lớp ẩn được gọi là "học sâu" (Deep Learning).
Lớp Đầu ra (Output Layer): Sản xuất kết quả cuối cùng của mô hình (ví dụ: xác suất ảnh này là "Lỗi" hay "Bình thường").
Precision : Tỉ lệ dự đoán đúng trong số các dự đoán dương tính mà mô hình đã đưa ra. Precision cao nghĩa là mô hình rất ít báo nhầm “có lỗi” khi thực tế không có.
Recall : Tỉ lệ dự đoán đúng trong số các mẫu dương tính thực sự. Recall cao nghĩa là mô hình ít bỏ sót lỗi.
F1-score : Trung bình điều hòa giữa Precision và Recall. Dùng để đánh giá tổng hợp khi cần cân bằng giữa "báo nhầm" và "bỏ sót".
Support : Số lượng mẫu thật sự thuộc về một lớp nào đó trong tập dữ liệu (ví dụ có bao nhiêu ảnh là “Lỗi”, bao nhiêu ảnh “Bình thường”).
Train : Giá trị đo trên tập huấn luyện — nơi mô hình học các đặc trưng.
Val : Giá trị đo trên tập validation — dùng để kiểm tra mô hình có bị overfit không.
LR (Learning Rate) : Tốc độ học, quyết định mức độ điều chỉnh trọng số sau mỗi bước tối ưu. LR quá lớn ➝ dễ làm mô hình dao động; quá nhỏ ➝ học rất chậm.
Công thức 1 nơ ron trong Hidden layer : x*i\ là đầu vào , w_i trọng số tương ứng x_i, b\ là hệ số bias, f(x)\ là hàm kích hoạt phi tuyến , a là đầu ra nơ ron
z\ =\ \sum*{i=1}^{n}{w_ix_i\ +b}\
a\ =\ f(x)\  
CHƯƠNG 3 : MÔ HÌNH CONVOLUTIONAL NEURAL NETWORK (CNN) VÀ SUPPORT VECTOR MACHINE (SVM)
3.1 Convolutional neural network
3.1.1 Giới thiệu
Mạng nơ-ron tích chập (Convolutional Neural Network – CNN) là một loại mô hình học sâu được thiết kế để xử lý dữ liệu có cấu trúc không gian như ảnh, video hoặc chuỗi thời gian. Khác với mạng nơ-ron truyền thống (Fully Connected Neural Network), CNN khai thác mối liên hệ cục bộ giữa các điểm dữ liệu thông qua phép tích chập (convolution), giúp giảm số lượng tham số và tăng khả năng tổng quát hóa.
CNN là nền tảng của hầu hết các ứng dụng trong thị giác máy tính (computer vision) như:
Nhận dạng ảnh (Image Classification)
Phát hiện vật thể (Object Detection)
Phân đoạn ảnh (Image Segmentation)
Phát hiện lỗi bề mặt, hư hại công trình, hoặc đường ray (như trong đề tài này)
3.1.2 Kiến trúc
Kiến trúc mô hình CNN điển hình được cấu thành từ việc xếp chồng nhiều lớp xử lý khác nhau.
Input
│
├── Convolution Layer → ReLU (hàm kích hoạt)
│
├── Pooling Layer
│
├── [Conv → ReLU → Pooling] × N
│
├── Flatten
│
├── Fully Connected Layer → ReLU
│
└── Output
Convolution Layer (Lớp tích chập): Đây là khối xây dựng cơ bản và quan trọng nhất của CNN. Thay vì kết nối mọi nơ-ron đầu vào với mọi nơ-ron đầu ra, lớp tích chập sử dụng các kernel nhỏ để quét qua toàn bộ ảnh. Kernel sẽ trượt trên toàn bộ ảnh đầu vào. Tại mỗi vị trí, nó thực hiện phép nhân theo từng phần tử (element-wise multiplication) với vùng ảnh mà nó bao phủ rồi tính tổng các giá trị đó. Kết quả của phép tính tổng này là một giá trị duy nhất trong ma trận đầu ra.
Feature Map (Bản đồ Đặc trưng): Toàn bộ ma trận đầu ra được tạo ra bởi một bộ lọc duy nhất được gọi là "bản đồ đặc trưng". Nó biểu thị vị trí và cường độ của đặc trưng mà bộ lọc đó tìm thấy trong ảnh. Một lớp tích chập thường có nhiều bộ lọc (ví dụ: 32, 64) để học nhiều loại đặc trưng khác nhau cùng một lúc.

Hình 4 Minh họa Feature Map được tạo ra sau nhiều lớp tích chập
Bản thân phép tích chập là một phép toán tuyến tính . Nếu chỉ xếp chồng các lớp tích chập, toàn bộ mạng vẫn sẽ là một mô hình tuyến tính, không đủ khả năng học các mối quan hệ phức tạp trong thế giới thực. Do đó, sau mỗi lớp tích chập, một hàm kích hoạt phi tuyến được áp dụng cho mọi phần tử trong bản đồ đặc trưng.
ReLU (Rectified Linear Unit): Là hàm kích hoạt phổ biến nhất trong các CNN hiện đại. Công thức của nó cực kỳ đơn giản:\ f(x)\ =\ max(0,\ x)
ReLU giúp giải quyết vấn đề vanishing gradient cho phép mạng học nhanh hơn và huấn luyện được các kiến trúc rất sâu.
Pooling Layer (Lớp gộp) : Sau khi các đặc trưng được phát hiện bởi lớp tích chập và hàm kích hoạt, Lớp Gộp có nhiệm vụ giảm chiều dữ liệu (down-sampling) một cách có hệ thống, làm cho biểu diễn dữ liệu trở nên nhỏ gọn và dễ quản lý hơn.
Giảm tải tính toán: Giảm kích thước không gian (chiều cao, chiều rộng) của bản đồ đặc trưng, từ đó giảm số lượng tham số và phép tính ở các lớp sau.
Tạo tính Bất biến (Invariance): Giúp mô hình có khả năng bất biến với các dịch chuyển nhỏ. Ví dụ, dù đặc trưng (một con mắt) nằm ở pixel (10, 10) hay (11, 11), lớp gộp vẫn sẽ cho ra kết quả tương tự. Điều này giúp mô hình tập trung vào sự hiện diện của đặc trưng chứ không phải vị trí chính xác của nó.
Các loại Gộp phổ biến:
Max Pooling: Phương pháp phổ biến nhất. Nó lấy một cửa sổ (và chỉ giữ lại giá trị lớn nhất trong cửa sổ đó. Điều này có nghĩa là nó giữ lại tín hiệu mạnh nhất, nổi bật nhất của đặc trưng.
Average Pooling: Lấy giá trị trung bình của tất cả các giá trị trong cửa sổ. Phương pháp này làm mượt dữ liệu, nhưng có thể làm loãng các tín hiệu đặc trưng mạnh.

Hình 5 Kết quả của phép Pooling tạo thành Pooled Feature Map
Fully Connected Layer (Lớp Kết nối Đầy đủ) : Sau khi đi qua nhiều chuỗi Convolution Layer và Pooling Layer, mô hình đã học được một tập hợp các bản đồ đặc trưng ở mức độ cao (high-level). Các bản đồ này vẫn ở dạng 3D (chiều cao x chiều rộng x số kênh). Để đưa ra quyết định phân loại cuối cùng, chúng ta cần chuyển đổi dữ liệu 3D này thành một vector 1D:
Flatten Layer (Lớp Làm phẳng): Thực hiện một thao tác đơn giản là "duỗi thẳng" khối đặc trưng 3D thành một vector 1D duy nhất.

Hình 6 Flattening – chuyển Feature Map 2D thành vector 1D
Fully Connected Layer (Lớp Kết nối Đầy đủ): Vector 1D này sau đó được đưa vào một hoặc nhiều Lớp Kết nối Đầy đủ, hoạt động giống hệt như Mạng Nơ-ron Nhân tạo (ANN) . Lớp này có nhiệm vụ tổng hợp tất cả các thông tin đặc trưng đã được trích xuất từ ảnh để đưa ra quyết định.
Output Layer (Lớp Đầu ra): Lớp FC cuối cùng sẽ có số nơ-ron bằng với số lớp (class) mà chúng ta muốn phân loại (ví dụ: 2 nơ-ron cho bài toán "Lỗi" và "Bình thường"). Một hàm kích hoạt như Softmax (cho phân loại nhiều lớp) hoặc Sigmoid (cho phân loại nhị phân) thường được sử dụng ở lớp cuối cùng để chuyển đổi điểm số của nơ-ron thành xác suất.
Tóm lại, một mô hình CNN hoạt động bằng cách sử dụng các Convolution Layer và Pooling Layer để tự động học và trích xuất các đặc trưng phân cấp từ ảnh sau đó sử dụng các Fully Connected Layer để phân loại dựa trên các đặc trưng đó.
3.1.3 Resnet (Residual Network)
Sau thành công của các kiến trúc CNN như AlexNet và VGG, giới nghiên cứu nhận thấy một xu hướng rõ ràng: các mô hình "sâu hơn" (có nhiều lớp hơn) thường cho kết quả tốt hơn. Tuy nhiên, việc đơn giản là xếp chồng thêm nhiều lớp (ví dụ: từ 20 lên 50, 100 lớp) lại dẫn đến một vấn đề nan giải.
3.1.3.1 Degradation Problem
Một cách trực quan, người ta kỳ vọng một mô hình 50 lớp sẽ có hiệu năng ít nhất là bằng một mô hình 20 lớp. Trong trường hợp xấu nhất, 30 lớp thêm vào có thể học một identity mapping (ánh xạ đồng nhất) – tức là chỉ cần trả ra đúng đầu vào của nó mà không làm gì cả, khi đó hiệu năng sẽ tương đương.
Tuy nhiên, thực tế lại không như vậy. Các mô hình rất sâu thường bị degradation (suy giảm): khi số lớp tăng lên, cả training error và testing error đều tăng lên. Điều này cho thấy mô hình không chỉ bị overfitting, mà còn không thể tối ưu được chính nó.
Vanishing Gradient : Càng nhiều lớp, gradient bị giảm khi lan truyền ngược
Khó khăn trong việc học identity mapping: Các hàm kích hoạt phi tuyến và các lớp tích chập khiến việc học một ánh xạ H(x)\ =\ x\ (chỉ trả lại đầu vào) trở nên cực kỳ khó khăn.
Giải pháp cho vấn đề đó, người ta tìm ra Residual Learning (Học dư) và Residual Block (Khối dư)
3.1.3.2 Residual Learning (Học dư)
ResNet, được giới thiệu bởi Kaiming He và cộng sự vào năm 2015, đã giải quyết triệt để vấn đề này bằng một ý tưởng: Skip Connection (Kết nối tắt). Thay vì bắt một khối các lớp học một ánh xạ H\left(x\right) mong muốn, ResNet bắt chúng học một residual mapping (ánh xạ dư), ký hiệu là F\left(x\right).
Kiến trúc của một Residual Block được định nghĩa như sau:
Đầu vào của khối là x
Đầu ra mong muốn của khối là H(x).
Thay vì học H\left(x\right) trực tiếp, ta định nghĩa F\left(x\right)=H\left(x\right)-x. Đây chính là phần residual (dư) – tức là phần chênh lệch mà các lớp này cần học thêm vào x để ra được H\left(x\right).
Từ đó suy ra, ánh xạ cuối cùng của khối là: H(x)\ =\ F(x)\ +\ x

Hình 7 Sơ đồ nguyên lý của khối Residual với kết nối tắt
Cơ chế hoạt động:
Đầu vào x được đưa vào một nhánh tính toán F(x) (thường gồm 2-3 lớp tích chập, Batch Norm và ReLU).
Cùng lúc đóm đầu vào x được đưa qua một skip connection (một đường nối thẳng, không qua phép biến đổi nào, hoặc chỉ biến đổi 1x1 để khớp kích thước) đến cuối khối.
Đầu ra của nhánh F(x) và đầu ra của nhánh tắt x\ được cộng lại với nhau theo từng phần tử (element-wise addition).

Hình 8 Cấu trúc chi tiết một khối Residual cơ bản
Giải quyết vấn đề identity mapping: Nếu trong trường hợp tối ưu, các lớp này không cần làm gì cả (tức H(x)\ =\ x), mô hình chỉ cần học F(x)\ =\ 0.\
Giải quyết vấn đề Vanishing Gradient: Trong quá trình lan truyền ngược, phép cộng H(x)\ =\ F(x)\ +\ x cho phép gradient đi qua hai con đường. Một đường đi qua nhánh F(x) (như bình thường) và một đường đi thẳng qua nhánh x. Con đường này cho phép gradient truyền thẳng về các lớp đầu tiên mà không bị suy giảm, giúp mạng có thể huấn luyện ngay cả khi rất sâu.
Nhờ kiến trúc này, các nhà nghiên cứu đã có thể huấn luyện thành công các mạng có độ sâu 152 lớp, 1000 lớp và hơn thế nữa, đạt được độ chính xác vượt trội trên nhiều bộ dữ liệu.
3.1.3.3 Triển khai Residual Block
Để triển khai khái niệm học dư, ResNet kế thừa triết lý thiết kế sử dụng các Convolution Layer 3x3 đồng nhất. Một Residual Block cơ bản thường được cấu tạo như sau:
Nhánh chính F(x) bao gồm hai Convolution Layer 3x3 được xếp chồng lên nhau, giữ nguyên số kênh đầu ra.
Mỗi lớp tích chập này được theo sau bởi một lớp Batch Normalization và một hàm ReLU.
Sau khi dữ liệu đi qua hai Convolution Layer này, Skip connection sẽ cộng đầu vào x ban đầu vào kết quả F(x).
Tổng H(x)\ =\ F(x)\ +\ x sau đó sẽ được đưa qua hàm ReLU cuối cùng của khối.
Thiết kế này yêu cầu đầu ra của nhánh Convolution F(x)\ phải có cùng hình dạng (chiều cao, chiều rộng, và số kênh) với đầu vào x để phép cộng có thể thực hiện được.Trong trường hợp cần thay đổi (tăng số kênh hoặc giảm kích thước), kết nối tắt x sẽ phải đi qua một Convolution Layer 1x1 bổ sung (projection shortcut). Lớp này có nhiệm vụ chuyển đổi x thành hình dạng mong muốn trước khi thực hiện phép cộng, đảm bảo tính tương thích về kích thước.

Hình 9 Cơ chế so khớp kích thước đầu ra bằng Projection Shortcut

Hình 10 Kiến trúc tổng thể của mạng ResNet50
3.1.3.4 Resnet50
ResNet50 là một trong những kiến trúc mạng nơ-ron tích chập (CNN) phổ biến và có ảnh hưởng nhất, thuộc họ ResNet . Con số "50" thể hiện rằng mô hình này có tổng cộng 50 lớp có thể huấn luyện (bao gồm 49 lớp tích chập và 1 lớp kết nối đầy đủ cuối cùng). Nó được coi là một cột mốc quan trọng vì đã cân bằng thành công giữa deep (độ sâu) của mạng và hiệu quả tính toán, trở thành một lựa chọn mặc định cho rất nhiều bài toán thị giác máy tính.
Khi các mạng ResNet trở nên rất sâu (như 50, 101, hay 152 lớp), Residual block cơ bản bắt đầu trở nên tốn kém về mặt tính toán.
Để giải quyết vấn đề này, ResNet50 (và các mạng sâu hơn) sử dụng một thiết kế Residual block được tối ưu hóa, gọi là Bottleneck Block (Khối "Nút cổ chai"). Khối này hiệu quả hơn về mặt tham số và tính toán.
Thay vì dùng 2 lớp 3x3, Bottleneck Block sử dụng một chuỗi 3 Convolution Layer
Convolution Layer\ \mathbf{1}\mathbit{x}\mathbf{1} (Giảm chiều): Lớp đầu tiên này nhận đầu vào có số kênh lớn (ví dụ: 256 kênh) và áp dụng các bộ lọc 1x1 để giảm số lượng kênh xuống một mức nhỏ hơn (ví dụ: 64 kênh). Đây chính là phần "nút cổ chai", giúp giảm tải tính toán cho lớp 3x3 tiếp theo.
Convolution Layer\ \mathbf{3}\mathbit{x}\mathbf{3} (Xử lý không gian): Convolution Layer 3x3 tiêu chuẩn thực hiện việc học đặc trưng không gian. Nhưng giờ đây, nó chỉ hoạt động trên đầu vào có 64 kênh (đã được giảm) thay vì 256 kênh, khiến phép toán này nhanh hơn đáng kể.
Convolution Layer \mathbf{1}\mathbit{x}\mathbf{1}\ (Phục hồi chiều): Lớp cuối cùng này nhận đầu ra 64 kênh từ lớp 3x3 và sử dụng các bộ lọc 1x1 để mở rộng (phục hồi) số kênh trở lại 256. Việc này đảm bảo rằng đầu ra F(x) có cùng số kênh với đầu vào x ban đầu, để có thể thực hiện phép cộng F(x)\ +\ x của skip connection.
Một Khối Residual Block cơ bản với 256 kênh sẽ có hai lớp 3x3x256. Trong khi đó, Bottleneck Block thay thế điều này bằng các lớp 1x1x64,\ 3x3x64,\ 1x1x256. Thiết kế này cho phép ResNet50 có độ sâu lớn hơn nhiều mà vẫn giữ chi phí tính toán trong tầm kiểm soát.
Kiến trúc ResNet50 đầy đủ được tổ chức thành 5 giai đoạn (phases):
Phase 1 (Conv1): Một lớp tích chập 7x7 lớn ban đầu và một lớp Max Pooling 3x3 để nhanh chóng giảm kích thước không gian và nắm bắt các đặc trưng tổng quát.
Phase 2 (Conv2): Một chuỗi gồm 3 Bottleneck Block.
Phase 3 (Conv3): Một chuỗi gồm 4 Bottleneck Block.
Phase 4 (Conv4): Một chuỗi gồm 6 Bottleneck Block.
Phase 5 (Conv5): Một chuỗi gồm 3 Bottleneck Block
Sau 5 giai đoạn này, một lớp Global Average Pooling (Gộp Trung bình Toàn cục) được sử dụng để lấy trung bình của từng feature map, tạo ra một vector đặc trưng duy nhất. Vector này sau đó được đưa vào một Fully Connection Layer cuối cùng để đưa ra dự đoán.
3.2 Support Vector Machine
3.2.1 Giới thiệu
Support Vector Machine (SVM) là một thuật toán học máy được đề xuất bởi Vapnik và cộng sự, thuộc nhóm mô hình học có giám sát (supervised learning). Khác với mô hình CNN – học trực tiếp từ dữ liệu ảnh thô qua nhiều tầng tích chập, SVM hoạt động bằng cách đi tìm một siêu phẳng (hyperplane) tối ưu để phân tách dữ liệu.
SVM là thuật toán đi tìm một siêu phẳng tối ưu để phân tách các lớp dữ liệu thành 2 phía sao cho các biên (margin) là lớn nhất. Các điểm dữ liệu gần nhất mặt phẳng nhất gọi là Support Vector – chúng là những điểm tiên quyết để quyết định đâu là mặt phẳng tối ưu nhất cho bài toán.
SVM được ứng dụng rộng rãi trong:
Phân loại nhị phân (Binary Classfication)
Phân loại đa lớp (Multi-class Classfication)
Nhận dạng mẫu (Pattern Recognition)
Phát hiện bất thường (Atomoly Detection)
3.2.2 Nguyên lý hoạt động
Khác với CNN vốn làm việc dựa trên việc xử lý các lớp xếp chồng lên nhau, SVM hoạt động dựa trên thuyết tối ưu lồi (convex optimization):
Siêu phẳng phân tách (Separating hyperplane)

Hình 11 Minh họa siêu phẳng phân tách và lề mềm trong SVM
Trong không gian đặc trưng \mathbb{R}^d, ta quy ước một siêu phẳng có dạng sau:
wTx + b = 0
với w\in\ \mathbb{R}^d\ là vector pháp quyến và b là bias. Với nhãn y\in{-1,\ 1}, điều kiện để một siêu phẳng phân tách đúng với mọi điểm là:
y*i(w^Tx_i+b)\geq1,\forall i.
Margin và mục tiêu tối ưu
Margin là khoảng cách giữa hai ranh:
\mathrm{margin}=\frac{2}{\parallel w\parallel}.\bigmVới bài toán SVM thì mục tiêu đặt ra là làm sao để tối đa hoá margin, tương đương tối thiểu hoá \frac{1}{2}\parallel w\parallel^2 dưới các ràng buộc phân lớp. Ta có bài toán tối ưu hoá (hard-margin):
{\min\funcapply}\below{w,b}\mathrm{\ }\frac{1}{2}\parallel w\parallel^2\mathrm{subject\ to\ }y_i(w^Tx_i+b)\geq1.
Đây được gọi là bài toán lồi (convex).
3.2.3 Soft-margin SVM( cho dữ liệu có nhiễu)
Trong thực tế dữ liệu lúc nào cũng bất thưởng: có nhiễu, outliers hoặc hai lớp không hoàn toàn tuyến tính, nằm tách về hai phía. Lúc này ta cần có Soft-margin SVM cho phép một số điểm vi phạm margin bằng cách thêm biến slack \xi_i\geq0:
y_i(w^Tx_i+b)\geq1-\xi_i,\xi_i\geq0.
Kết hợp với bài toán lồi ta có:
{\min\funcapply}\below{w,b,\xi}\frac{1}{2}\parallel w\parallel^2+C\sum*{i=1}^{N}\xi_i,
Trong đó C > 0 là hệ số phạt cho các vi phạm, khi C lớn, môt hình phạt nặng lỗi hạn chế các lỗi của các điểm dữ liệu; khi C nhỏ mô hình hco phép lỗi nhiều để giữ margin rộng hơn việc này sẽ tốt cho tổng quát. Soft-margin có thể được giải qua bài toán đối ngẫu Lagrange hoặc chueyer về dạng không ràng buộc hinge loss để tối ưu bằng gradient-based methods, thuận tiện cho bài toán lớn.
3.2.4 Kernel SVM (xử lý dữ liệu phi tuyến)
Với các nguồn dữ liệu không đẹp, nhiều đữ liệu không thể phân tách bằng một mặt phẳng trong không gian ban đầu. Ta xử dụng ánh xạ dữ liệu sang một không gian mới có chiều cao hơn, nơi dữ liệu trở nên tuyến tính và phân tách.

Hình 12 Ánh xạ phi tuyến sang không gian chiều cao bằng Kernel Trick
Thay vì tình trực tiếp ánh xạ \phi(x) SVM sử dụng Kernel Function K(x,z)=\phi(x)^T\phi(z) để làm mọi phép toán cần thiết trong không gian mới mà không cần ánh xạ rõ ràng. Một trong số các kernel phổ biến:
Linear: K(x,z)=x^Tz
Polynomial: K(x,z)=(\gamma x^Tz+r)^d
RBF (Gaussian): K(x,z)=\exp\funcapply(-\gamma\parallel x-z\parallel^2)— thường được dùng làm mặc định cho bài toán phi tuyến
Sigmoid: K(x,z)=\tanh\funcapply(\gamma x^Tz+r)
Với Kernel thuật toán SVM có thể học các biên phân cách phi tuyến tính phức tạp mà vẫn giữ được lợi thế của SVM là bài toán tối ưu lồi. Tuy, nhiên bài toán cần lưu ma trận kernel (kích thước N x N) vì vậy thuật toán SVM phù hợp với tập dữ liệu vừa và nhỏ.
3.2.5 Bài toán đối ngẫu và support vectors
Sử dụng phươg pháp Lagrange, bài toán trên được chuyển sang bài toán đối ngẫu:
{max}\below\lambda\sum*{i=1}^{N}\lambda_i-\frac{1}{2}\sum*{i,j}\lambda*i\lambda_jy_iy_jK\left(x_i,x_j\right)
Nghiệm \lambda là sparse: chỉ một số \lambda_i>0. Những điểm có \lambda_i>0 chính là support vectors – chỉnh chúng ảnh hưởng đến hàm dự đoán:
\sum*{i=1}^{N}\lambda_iy_i=0,0\le\lambda_i\le C.
Với bài toán đối ngẫu ta sẽ tối ưu hơn cho module bằng các lưu các support vector thay vì phải lưu các ma trận lớn, giảm hiểu không gian lưu trữ cho mô hình, tiết kiệm được phần cứng cung cấp cho dự án.

CHƯƠNG 4 : TRIỂN KHAI ỨNG DỤNG
4.1 Giới thiệu tập dữ liệu
Bộ dữ liệu Railway Track Fault Detection trên kaggle là 1 bộ dữ liệu hình ảnh gồm 3 tệp Train, Validation và Test. Mỗi tệp chứa 2 tệp Defective (Hư hại) và Non-Defective (Bình thường) của các đường ray ở Bangladesh. Bộ dữ liệu gồm 2.14GB, hơn 360 ảnh chụp. Tuy khá ít nhưng vừa đủ để huấn luyện mô hình.
Dữ liệu có độ đa dạng vừa phải, bao gồm nhiều loại lỗi như:
Nứt gãy,
Khuyết thanh ray,
Biến dạng,
Sai lệch bề mặt, cùng với nhiều điều kiện môi trường khác nhau.
Một số hình ảnh minh hoạ của hai lớp được trình bày dưới đây:

Defective

Non defective

4.2 CNN – Resnet50
Trong phần này, mô hình chính được sử dụng là ResNet50 – một mạng CNN sâu 50 lớp, được huấn luyện sẵn (pretrained) trên bộ dữ liệu ImageNet.
ResNet50 áp dụng kiến trúc Residual Learning giúp gradient lan truyền tốt hơn trong mạng sâu, từ đó cải thiện khả năng học và độ chính xác.
Nhằm thích ứng với tập dữ liệu đặc thù của đề tài, mô hình được fine-tune theo 2 giai đoạn (2 phases). Mỗi giai đoạn sẽ mở khoá (unfreeze) thêm các tầng sâu hơn trong mạng và huấn luyện lại với learning rate phù hợp.
4.2.1 Xử lý dữ liệu
Dữ liệu hình ảnh ban đầu có kích thước và tỉ lệ khác nhau. Tính toán tệp dữ liệu bằng python:

sizes = []

for cls in classes:
folder = os.path.join(train_dir, cls)
for filename in os.listdir(folder):
if filename.lower().endswith(('.jpg', '.jpeg', '.png')):
path = os.path.join(folder, filename)
with Image.open(path) as img:
sizes.append(img.size) # (width, height)

# Đếm tần suất từng kích thước

size_counts = Counter(sizes)

Do đó cần được chuẩn hoá trước khi đưa vào mô hình. Các bước xử lý chính bao gồm:
Resize ảnh về 224 × 224 pixels
Chuyển ảnh sang dạng Tensor.
Chuẩn hoá theo bộ giá trị trung bình và độ lệch chuẩn của ImageNet.
Tăng cường dữ liệu (Data Augmentation)
Để khắc phục việc thiếu dữ liệu và giúp mô hình tổng quát hóa tốt hơn, nhiều kỹ thuật tăng cường được áp dụng:
Horizontal Flip
Random Rotation
Normalization
Các thao tác này làm tăng sự đa dạng của dữ liệu huấn luyện mà không làm thay đổi nhãn ảnh.
#Image Normalize và Augmentation
train_tfms = transforms.Compose([
transforms.Resize((256, 256)), # Cố định kích thước trước
transforms.RandomCrop(224), # Crop nhẹ để tạo biến thể
transforms.RandomHorizontalFlip(), # Lật ngang (an toàn)
transforms.RandomVerticalFlip(), # Lật dọc (an toàn với đường ray)
transforms.RandomRotation(10), # Xoay nhẹ
transforms.ToTensor(),
transforms.Normalize(mean, std)
])

4.2.2 Huấn luyện phase 1
Mục tiêu: Khởi tạo classifier head phù hợp với dataset. Quá trình huấn luyện được triển khai theo mini-batch, sử dụng backpropagation và cập nhật trọng số bằng Adam optimizer.
Chiến lược:
Freeze: Toàn bộ backbone (layer1-4)
Train: Chỉ FC layer (classification head)
Optimizer: Adam với learning rate 1e-4
Loss: CrossEntropyLoss
Lý do: Giữ nguyên features từ ImageNet, chỉ học phân loại 2 classes mới.

# --- PHASE 1: WARM UP HEAD (5 Epochs) ---

for param in model.parameters():
param.requires_grad = False
for param in model.fc.parameters():
param.requires_grad = True

# Loss, optimizer

optimizer = optim.Adam(model.fc.parameters(), lr=1e-4)
criterion = nn.CrossEntropyLoss(label_smoothing=0.01)

4.2.3 Huấn luyện phase 2
Mục tiêu: Điều chỉnh các high-level features để phù hợp với railway track.
Chiến lược:
Freeze: Không
Train: Toàn bộ ResNet50
Optimizer: Adam với learning rate 1e-4
Epochs: tối đa 20, dừng sớm khi không cải thiện được thêm.
Lý do: điều chỉnh các đặc trưng cấp cao và trung gian cho phù hợp với domain railway track, đồng thời sử dụng early stopping để tránh overfitting.

# Mở khóa layer4 + fc để fine-tune (các layer khác giữ nguyên đóng băng)

for param in model.parameters():
param.requires_grad = True

# Optimizer LR nhỏ để không phá hỏng backbone

optimizer = optim.Adam(model.parameters(), lr=1e-4, weight_decay=1e-4)
scheduler = optim.lr_scheduler.ReduceLROnPlateau(optimizer, mode='max', factor=0.1, patience=
best_acc = 0.0
EPOCHS = 20
early_stop = EarlyStopping(patience=5, min_delta=1e-4)

4.2.4 Kết quả chạy mô hình
Kết quả chạy ra ở phase 1

Kết quả chạy ra ở phase 2

Kết quả finaly
=== 📊 Classification Report (Test set – Final Result) ===
Precision Recall F1-Score Support
Defective 1.000 0.909 0.952 11
Non Defective 0.917 1.000 0.957 11
Accuracy 0.955 22
Macro avg 0.958 0.955 0.954 22
Weighted avg 0.958 0.955 0.954 22

Hình 15: Kết quả tốt nhất của tập Test sau fine-tuning
4.3 SVM – Kernel Support Vector Machine
Khác với phương pháp học sâu thuần túy ở phần trước, phần này áp dụng phương pháp hỗn hợp. Chúng tôi sử dụng ResNet50 làm bộ trích xuất đặc trưng để chuyển đổi hình ảnh thành các vector đặc trưng, sau đó sử dụng thuật toán SVM để phân loại.
4.3.1 Trích xuất đặc trưng
Mục tiêu: Chuyển đổi dữ liệu hình ảnh thô thành các vector số học mang ý nghĩa ngữ nghĩa cao, đồng thời giải quyết vấn đề mất cân bằng dữ liệu thông qua tăng cường ngoại tuyến.
Chiến lược:
Backbone: Sử dụng ResNet50 (weights='imagenet') bỏ lớp Fully Connected (include_top=False) và dùng lớp Global Average Pooling để thu về vector đặc trưng kích thước (2048).
Augmentation: Dữ liệu Train được tăng cường trước khi đưa vào trích xuất đặc trưng. Mỗi ảnh gốc được sinh ra thêm 7 biến thể (n_aug=7) bao gồm xoay, dịch chuyển và chỉnh độ sáng.
Lý do: Việc trích xuất đặc trưng giúp SVM làm việc hiệu quả trên không gian dữ liệu chiều cao, giảm tải tính toán so với việc fine-tune toàn bộ mạng CNN, đồng thời tận dụng được khả năng nhận diện đặc trưng mạnh mẽ của ResNet50.

resnet_model = ResNet50(
weights='imagenet',
include_top=False,
pooling='avg'
)

def extract_features(paths, batch_size=16):
features = []
for i in range(0, len(paths), batch_size):
batch_paths = paths[i:i+batch_size]
imgs = [img_to_array(load_img(p, target_size=(224, 224))) for p in batch_paths]
arr = preprocess_input(np.array(imgs))
feats = resnet.predict(arr, verbose=0)
features.append(feats)
return np.vstack(features)

# Augmentation

datagen = ImageDataGenerator(
rotation_range=15,
width_shift_range=0.1,
height_shift_range=0.1,
horizontal_flip=True,
brightness_range=[0.8, 1.2],
fill_mode='nearest'
)

def extract*augmented_train(paths, labels, n_aug=7):
features, labs = [], []
for p, l in zip(paths, labels):
img = img_to_array(load_img(p, target_size=(224, 224))) # Ảnh gốc
feats_orig = resnet.predict(preprocess_input(np.array([img])), verbose=0)
features.append(feats_orig)
labs.append(l) # Ảnh augmentation
for * in range(n_aug):
aug = next(datagen.flow(img.reshape(1, \*img.shape), batch_size=1))[0]
feats_aug = resnet.predict(preprocess_input(np.array([aug])), verbose=0)
features.append(feats_aug)
labs.append(l)
return np.vstack(features), np.array(labs)

# Trích xuất đặc trưng

X_train_feat, y_train_aug = extract_augmented_train(X_train_paths, y_train, n_aug=7)
X_val_feat = extract_features(X_val_paths) # Validation RAW
X_test_feat = extract_features(X_test_paths) # Test RAW

4.3.2 Tối ưu tham số và huấn luyện mô hình
Mục tiêu: Tìm ra siêu phẳng (hyperplane) tối ưu để phân tách hai lớp "Defective" và "Non defective" với sai số thấp nhất.
Chiến lược:
Pipeline: Chuẩn hóa dữ liệu đầu vào (StandardScaler) trước khi đưa vào mô hình SVC để đảm bảo sự hội tụ tốt hơn.
Kỹ thuật K-Fold Cross-Validation: Để đảm bảo tính khách quan và tránh hiện tượng overfitting cục bộ, chúng tôi áp dụng kỹ thuật kiểm định chéo với K=3 (3-Fold Cross-Validation).
Tập dữ liệu huấn luyện được chia thành 3 phần (folds) bằng nhau.
Quá trình huấn luyện được lặp lại 3 lần: mỗi lần sử dụng 2 phần để train và 1 phần để validate.
Kết quả cuối cùng là trung bình cộng của 3 lần chạy, giúp đánh giá chính xác độ ổn định của bộ tham số.
Hyperparameter Tuning: Sử dụng GridSearchCV với kiểm định chéo (Cross-Validation, cv=3) để tìm bộ tham số tốt nhất.
Không gian tham số (Param Grid):
C: [0.1, 0.5, 1] (Kiểm soát mức độ phạt lỗi - Regularization).
kernel: ['linear', 'rbf'] (So sánh giữa phân tách tuyến tính và phi tuyến).
gamma: [0.001, 0.005, 'scale'] (Hệ số nhân cho kernel RBF).
Lý do: GridSearch giúp tự động hóa việc thử nghiệm các tổ hợp tham số, đảm bảo mô hình chọn được cấu hình tối ưu nhất cho tập dữ liệu đường ray.
param_grid = {
'svc**C': [0.1, 0.5, 1],
'svc**kernel': ['linear', 'rbf'],
'svc\_\_gamma': [0.001, 0.005, 'scale'],

pipeline = make_pipeline(StandardScaler(), SVC(probability=True, random_state=42))
grid = GridSearchCV(pipeline, param_grid, cv=3, scoring='f1', n_jobs=-1, verbose=2)
grid.fit(X_train_feat, y_train_aug)

4.3.3 Kết quả chạy mô hình
Classification Report - Test:
, , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , ,
Class Precision Recall F1-score Accuracy
0 Non defective 0.909091 0.909091 0.909091 0.909091
1 Defective 0.909091 0.909091 0.909091 0.909091
2 Macro avg 0.909091 0.909091 0.909091 0.909091
3 Weighted avg 0.909091 0.909091 0.909091 0.909091

Hình 16 TestReport SVM
GridSearchCV đã thử 18 tổ hợp siêu tham số và thực hiện tổng cộng 54 lần huấn luyện (3-fold CV cho mỗi tổ hợp). Bộ tham số tối ưu tìm được là C=1, kernel=rbf và gamma='scale'. Đây là cấu hình giúp mô hình đạt F1-score cao nhất (0.909091) trên 3 lần chia dữ liệu, chứng tỏ mô hình có khả năng tổng quát hóa tốt.
CHƯƠNG 5 : ĐÁNH GIÁ MÔ HÌNH
5.1 Đánh giá mô hình ResNet50
Class Precision Recall F1-score Support
Defective 0.933 0.903 0.918 31
Non defective 0.906 0.935 0.921 31
Accuracy 0.919 62
Macro avg 0.920 0.919 0.919 62
Weighted avg 0.920 0.919 0.919 62
5.1.1 Accuracy trên tập Validation
Sau quá trình huấn luyện gồm bốn phase fine-tuning, mô hình ResNet50 đạt độ chính xác trên tập validation tốt nhất là 0.919.
So với các phase trước đó, Phase 1 kết thúc với val accuracy khoảng 0.871.

Hình 17 Biểu đồ Loss, Accuracy Phase 1
Phase 2 đạt 0.887

Hình 18 Biểu đồ Loss, Accuracy Phase 2
Phase 3 đạt 0.919

Hình 19 Biểu đồ Loss, Accuracy Phase 3
Phase 4 chỉ cải thiện nhẹ nhưng không vượt qua mức 0.919.

Hình 20 Biểu đồ Loss, Accuracy Phase 4
Điều này chứng minh rằng việc fine-tuning theo từng giai đoạn đã giúp mô hình hội tụ ổn định và tăng dần độ chính xác theo thời gian.
5.1.2 Biểu đồ Loss và Accuracy trong quá trình huấn luyện
Dựa trên log huấn luyện bốn phase, Loss giảm đều và ổn định theo từng epoch. Accuracy cũng tăng dần qua mỗi phase, đặc biệt từ Phase 2 đến Phase 3.
Không xuất hiện hiện tượng dao động mạnh hay mất ổn định gradient. Early stopping xảy ra ở Phase 3, đảm bảo mô hình không bị overfitting.
Việc huấn luyện theo từng giai đoạn, bằng cách unfreeze dần từng phần backbone, đã giúp tránh hiện tượng catastrophic forgetting. Đồng thời, phương pháp này tận dụng tốt trọng số pretrained và tối ưu hiệu quả mà không làm mô hình mất ổn định.
5.1.3 Đánh giá quá trình fine-tuning qua từng phase
Trong Phase 1, khi chỉ huấn luyện Fully Connected Layer, độ chính xác trên tập huấn luyện tăng từ 0.640 lên 0.797, trong khi độ chính xác trên tập validation tăng từ 0.532 lên 0.871. Điều này cho thấy mô hình đã học được các đặc trưng cơ bản của bài toán.
Sang Phase 2, khi mở một phần backbone, độ chính xác tăng nhẹ nhưng ổn định; cụ thể, val accuracy tăng từ 0.855 lên 0.887. Kết quả này cho thấy mô hình bắt đầu học sâu hơn vào các đặc trưng hình ảnh đường ray.
Trong Phase 3, khi mở sâu hơn các tầng và giảm learning rate, val accuracy đạt đỉnh 0.919. Đây là giai đoạn quan trọng nhất, mô hình tối ưu tốt nhất và cho hiệu quả cao nhất trên tập validation.
Phase 4 thực hiện fine-tuning toàn bộ mô hình. Val accuracy dao động trong khoảng 0.855 đến 0.903, không vượt qua mức 0.919 đã đạt ở Phase 3. Phase này giúp mô hình hội tụ mượt hơn, ổn định hơn nhưng không cải thiện vượt trội về hiệu năng.
Kết luận chung là Phase 3 là giai đoạn tối ưu nhất cho mô hình ResNet50.
5.2 Đánh giá mô hình Kernel SVM
Mô hình SVM được huấn luyện dựa trên đặc trưng 2048 chiều được trích xuất từ ResNet50 (với include_top = False, pooling = 'avg') và áp dụng tăng cường dữ liệu (augmentation) với hệ số nhân 7×. Sau khi tối ưu siêu tham số bằng GridSearchCV, mô hình SVM đạt hiệu năng cao trên cả ba tập Train – Validation – Test. Phần này trình bày chi tiết các chỉ số đánh giá, khả năng tổng quát hóa và hiệu năng phân biệt của mô hình.
Bộ dữ liệu Accuracy F1-score Precision Recall Specificity
Train 0.998746 0.99874 1.0000 0.997483 1.0000
Validation 0.935484 0.935484 0.935484 0.935484 0.935484
Test 0.909091 0.909091 0.909091 0.909091 0.909091
5.2.1 Đánh giá định lượng
Dựa vào các thông số của mô hình ta thấy:
Train Accuracy gần như tuyệt đối (0.9987):
Augmentation tạo ra nhiều mẫu rất đa dạng,
Đặc trưng ResNet50 có khả năng phân tách mạnh,
SVM kernel RBF là mô hình phi tuyến hiệu quả.
Validation đạt 93.55% và Test đạt 90.91%:
Không có dấu hiệu overfitting nghiêm trọng.
Mức giảm giữa Train → Val → Test là hợp lý.
Precision = Recall = F1 ở cả 3 tập:
Điều này chứng tỏ mô hình cân bằng giữa False Positive và False Negative, phù hợp với yêu cầu phát hiện lỗi đường ray.
Specificity > 0.90:
Mô hình ít báo động giả.
5.2.2 Khả năng tổng quát hóa của mô hình
Sự chênh lệch giữa Train – Validation – Test được xem là thấp: (Train: 0.9987, Validation: 0.935, Test: 0.9090). Điều này cho thấy:
Mô hình học tốt và ổn định với dữ liệu chưa từng thấy.
Bộ đặc trưng ResNet50 có tính tổng quát cao, đặc biệt hiệu quả khi dataset nhỏ.
SVM sử dụng kernel RBF đã tạo được biên phân chia tối ưu trong không gian 2048 chiều.
GridSearchCV(3-Fold) giúp tìm ra tham số tối ưu nhất đối với mô hình:
C = 1
gamma = 'scale'
kernel = 'rbf'
Best CV F1-score = 0.8356
5.2.3 Đánh giá mô hình với ROC Cruve và PR Cruve
Để đánh giá khả năng phân biệt giữa hai lớp “Defective” và “Non-defective”, mô hình SVM được kiểm tra bằng hai đường cong quan trọng: ROC Curve (Receiver Operating Characteristic) và Precision–Recall Curve. Hai loại biểu đồ này phản ánh chất lượng dự đoán vượt ra ngoài các metrics truyền thống như Accuracy hay F1-score, đặc biệt hữu ích trong các bài toán có tính rủi ro cao như phát hiện lỗi đường ray.
Đánh giá với ROC Cruve
ROC Curve biểu diễn mối quan hệ giữa:
TPR (True Positive Rate / Recall)
FPR (False Positive Rate)
Khi thay đổi ngưỡng phân loại. Một mô hình tốt sẽ có đường ROC nằm càng xa đường chéo ngẫu nhiên (0.5) càng tốt. Giá trị này biểu thị diện tích dưới đường cong ROC, cho thấy mô hình có khả năng phân biệt hai lớp rất tốt. AUC gần 1.0 nghĩa là xác suất mô hình xếp một ảnh “Defective” cao hơn một ảnh “Non-defective” gần như tuyệt đối.

Hình 21 Biểu đồ TPR/FDR
Dựa trên kết quả thực nghiệm, mô hình đạt:
ROC – AUG = 0.959
Giá trị này biểu thị diện tích dưới đường cong ROC, cho thấy mô hình có khả năng phân biệt hai lớp rất tốt. ROC gần 1.0 nghĩa là xác suất mô hình xếp một ảnh “Defective” cao hơn một ảnh “Non-defective” gần như tuyệt đối.
Đánh giá với mô hình PR Curve
Precision–Recall Curve được sử dụng đặc biệt hiệu quả cho bài toán mất cân bằng lớp, nơi số lượng mẫu lỗi thường ít hơn mẫu bình thường – đúng với đặc trưng của dữ liệu đường ray.
Biểu đồ PR mô tả mối quan hệ giữa:
Precision – độ chính xác khi mô hình dự đoán ảnh có lỗi
Recall – khả năng mô hình phát hiện lỗi mà không bỏ sót

Hình 22 Biểu đồ Precision/Recall
Kết quả thực nghiệm cho thấy:
PR-AUC = 0.966
Đây là một giá trị rất cao, chứng minh mô hình vừa phát hiện lỗi tốt (Recall cao), vừa ít báo nhầm lỗi (Precision cao) trên tập Test.
5.3 Đánh giá và kết luận chung cho 2 mô hình
Mặc dù cả hai mô hình đều đạt kết quả trên 90%, ResNet50 cho thấy hiệu năng vượt trội hơn (+1.0%) so với SVM. Việc cho phép mô hình tinh chỉnh các trọng số sâu giúp nó học được những đặc trưng tinh tế nhất của vết nứt đường ray mà phương pháp trích xuất đặc trưng cố định của SVM có thể đã bỏ qua. Do đó, ResNet50 được đề xuất là mô hình cuối cùng cho ứng dụng thực tế.

 
CHƯƠNG 6 : KẾT LUẬN
Trong bối cảnh hạ tầng đường sắt Việt Nam còn nhiều hạn chế và việc kiểm tra thủ công tốn nhiều nhân lực, thời gian và không đảm bảo độ chính xác, việc ứng dụng các mô hình học sâu vào phát hiện lỗi đường ray là một hướng đi thực tiễn. Thông qua đề tài này, nhóm đã triển khai thành công mô hình Convolutional Neural Network (CNN), cụ thể là kiến trúc ResNet50, nhằm nhận diện các trường hợp đường ray hư hại dựa trên dữ liệu hình ảnh.
Trong quá trình thực hiện, nhóm đã tiến hành xử lý dữ liệu, xây dựng pipeline huấn luyện theo phương pháp fine-tuning nhiều giai đoạn, cùng với các kỹ thuật tối ưu như Data Augmentation, Weight Decay và Mixup. Các kỹ thuật này giúp mô hình học sâu hơn, ổn định hơn và tránh hiện tượng overfitting khi tập dữ liệu không quá lớn.
Kết quả đánh giá cho thấy mô hình ResNet50 đạt hiệu suất cao trên cả tập Validation. Chỉ số Accuracy ở mức đáng tin cậy, khẳng định khả năng phân loại tốt giữa hai nhóm ảnh “Defective” và “Non-defective”. Đồng thời, việc phân tích các trường hợp dự đoán sai đã cung cấp những góc nhìn thực tế về hạn chế của mô hình, như: nứt gãy, khuyết thanh ray, biến dạng, sai lệch bề mặt, cùng với nhiều điều kiện môi trường khác nhau.
Mặc dù mô hình đã đạt kết quả tốt, đề tài vẫn còn một số hạn chế. Tập dữ liệu hiện tại còn nhỏ và chưa đa dạng về môi trường, điều kiện ánh sáng và góc chụp. Ngoài ra, mô hình chưa được thử nghiệm trên môi trường thực tế hoặc trên video liên tục.
Tổng kết lại, mô hình ResNet50 là một giải pháp khả thi và hiệu quả cho bài toán phát hiện lỗi đường ray dựa trên hình ảnh. Đề tài đã chứng minh được tiềm năng ứng dụng của Deep Learning trong công tác giám sát và bảo trì hạ tầng giao thông, góp phần hướng đến một hệ thống đường sắt hiện đại, an toàn và vận hành hiệu quả hơn trong tương lai.

TÀI LIỆU THAM KHẢO
Nguyễn, Tuấn Thanh. Deep Learning cơ bản. Nguyễn Thanh Tuấn, 2020. Blog | Deep Learning cơ bản, https://nttuan8.com/sach-deep-learning-co-ban/.
Vũ, Tiệp Hữu. Machine Learning cơ bản. Vũ Hữu Tiệp, 2018. Machine Learning cơ bản, https://machinelearningcoban.com/ebook/.
Zhang, Aston, et al. Dive into Deep Learning. Cambridge University Press, 2023. Dive into Deep Learning, https://D2L.ai.
