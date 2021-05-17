Thêm bản ghi TXT trên quản lý DNS

“v=spf1 ip4:118.102.6.0/24 a mx ~all” đây chính là bản ghi TXT khai báo cấu hình SPF
spf1: version c ủa SPF
ip4:118.102.6.0/24: Domain @topdev.vn sẽ sử dụng dải IP này để gửi email
a: sử dụng IP domain topdev.vn, nếu ghi là a:server1.topdev.vn thì nghĩa là sử dụng IP bản ghi A server1.topdev.vn
mx: giống như bản ghi A nhưng đây là bản ghi MX
~all: Nói với bên nhận email “Các IP ngoài các IP trên thì đều không phải gửi từ @zing.vn nhưng bạn hãy cứ nhận email và đánh dấu nó”