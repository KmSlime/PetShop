# PetShop
DoAn ASP.NET


Tất cả các admin đều có pass là A123456
client tự đăng ký

# Chức năng: 

-> Client

	1. Trang chủ: 	-> Ấn vào logo có thể về trang chủ
					-> Sử dụng boostrap để tạo banner động (Carousel) 
					-> Các menu bar tùy chức năng: ở đây có nút icon trang chủ, thẻ giới thiệu, droplist shop và blog, giỏ hàng
					-> Dropdown list để thu gọn menu account
					-> Nút liên kết với các trang khác của chủ shop (ở đây lấy ví dụ là Liêm)
					-> 3 menu danh mục: sử dụng sẽ trỏ tới các sản phẩm thuộc danh mục đó 
					-> các sản phẩm có các nút thêm vào giỏ hàng: click sẽ hiển thị messagebox thêm thành công
					-> sản phẩm khuyến mãi sử dụng hover và focus để hiển thị và ẩn các nút xem chi tiết: click sẽ vào trang chi tiết sản phẩm
																										và các sản phẩm liên quan
					-> Sản phẩm bán chạy tương tự
					-> foother có các colum hiển thị các thông tin về shop
	
	2. Dropdown list Shop có thể hiển chọn mục cho thú cưng: ví dụ như chó và mèo
					-> trong đó có sẵn các danh mục được sắp xếp và thêm sẵn với id của thú cưng
	
	3. Tìm kiếm 	-> Tìm kiếm constain + lower case! 
	
	4. Giỏ hàng 	->  - bấm vào sẽ di chuyển tới menu giỏ hàng
						- Xóa sản phẩm. xóa tất cả sản phẩm 
							+ Show message box nếu giảm số lượng xuống dưới 1
						- Tổng tiền (+- theo sản phẩm) + tăng giảm sản phẩm
						- Tạo order sẽ hiển thị tên, địa chỉ, sdt, đơn hàng, tổng tiền và chỉnh sửa vị trí giao hàng
						- Cho phép đồng thời gửi dữ liệu về database
						- Thanh toán sẽ gửi hóa đơn về mail -> hiển thị màn hình confirm và cảm ơn
						- Partial view
	5. Trang sản phẩm 				-> hiển thị thông tin sản phẩm	
	
	6. Trang chi tiết sản phẩm 		-> có thông tin chi tiết sản phẩm, nút thêm giỏ hàng, tăng giảm số lượng, các sản phẩm liên quan
	
	5. Login 		 ->	- thực hiện những cái trên
						- dropdown list có hiển thị thông tin khách hàng
						- đổi mật khẩu: + nếu nhập lại mk ko giống với mk mới -> thông báo ko trùng
										+ nếu đổi được -> thông báo đổi thành công
						- Đăng xuất: logout khỏi tài khoản
                        
-> Admin
	1. Trang chủ: coi được danh mục, sản phẩm, đơn hàng, khách hàng
				-> Khách hàng: có thể chỉnh sửa thông tin hoặc xóa khách hàng, sắp xếp theo tên thứ tự alphabex hoặc ngày tạo tk 
				-> Sản phẩm: - hiển thị thông tin sản phẩm, thêm mới, hiển thị theo sắp xếp: tên, ngày nhập, giá, sl tồn
							 - chỉnh sửa, xóa
							 - thêm mới
							 - tìm kiếm theo contains lower case 
				-> Đơn hàng: - thông tin đơn hàng
							 - thông tin chi tiết đơn hàng 
							 - sửa, xóa đơn hàng: trong mục sửa có xác nhận trạng thái
							 - tìm kiếm đơn hàng
				-> Danh mục sp: 
							 - sắp xếp: tên
							 - Thêm mới
							 - sửa, xóa
							 - tìm kiếm đơn hàng
