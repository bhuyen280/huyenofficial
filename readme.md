kiểm tra kiến thức cũ nhá
git là gì ? 
git laf 1 dichj vụ lưu trữ, để lưu trữ code
git không phải là 1 dịch vụ lưu trữ
git là 1 hệ thống kiểm soát kiểm soát phiên bản (version control system - VCS)
github mới là để lưu trữ nhá.
git là cái bạn bạn đang cài trên máy đây, nó ko lưu trữ, mà code của bạn lưu tữ trên máy của bạn.
ko có git thì vẫn lưu trữ code được đó thôi, nó lưu trên ổ cứng máy ấy
nhưng git là 1 hệ thống kiểm soát kiểm soát phiên bản VCS
code của bạn push lên github, nó mới là công cụ lưu trữ.
nói thêm về file .md nha
thì thông thường để cho chuyên nghiệp
trong 1 folder code ABC hay có 1 file tên là readme.md hoặc document.md
nó sẽ nằm ở thư mục ngoài cùng,  chứ ko phải ở trong 1 thư mục con của ABC
nó dùng để viết nhữung cái mô tả thêm về dự án của bạn, ví dụ tác giả, ngày code, sử dụng những công nghệ gì vv..
nói chung là tất những gì mình muốn người ta biêt khi mở folder dự án lên
người ta nhìn thấy file .md tự hiểu là file để mô tả về dự án
mô tả gì ? thì tùy bạn thôi.
thông thườn những project chuyên nghiệp chắc chắn phải co 1 file .md 
file .md cũng giống như file .docx hay .txt 
dùng để lưu văn bản thôi, ko phải để viết code
nhưng ko dùng file .docx hay .txt trong project
ví dụ, tải bùa 1 dự án về xem nó file .md khôn gnhá
không bắt buộc có file.md nhưng mà nó thể hiện sự chuyên nghiệp
bạn nói lại về quy tắt đặt tên trong khóa học đã nói đi. ngắn gọn thôi
1 có ý nghĩa
2 ưu tiên tieenga anh
3 bắt đầu băng chữ cái hoặc dấu gạch dưới
4 nếu 1tuwf thì nên viết thường
nếu 2 từ thì từ liền sau viết hoa hặc cách bằng dấu gạch ngang, gạch dưới
ok vậy là ổn rồi, quan trọng là không cách bằng dấu cách là được,
cách tạo thêm 1 repo (respository = KHO) trên github
new/ viết tên (cũng ưu tiên tiếng anh, không cách, dùng dấu gạch thay cho dấu cách, nếu chỉ 1 từ thì ko cần cách)/ chọn public hoặc privateví dụ nhá à thôi , cái này ví dụ sau, nếu ko gì đặc biệt thì mặc định là public (công khai, tức mọi ng có thể xem được code của bạn trong repo này
giống kiểu chỉnh sửa quyền riêng tư của 1 bài viết trên fb, private kiểu là "chỉ mình tôi", public là "mọi người")
Add a README file  là tùy chọn, nó sự thêm file READ ME.md vào repo của bạn, hoặc bạn cũng có thể không tick
vì bạn có thể tự tạo ra file này 
đó, giờ thì nó tự tạo ra trong repo 1 file readme.md ko thích có thể xóa
bây giờ là có 2 repo
code trong mỗi repo là độc lập với nhau
vì nó ở trên github chứ chưa ở trong máy , nên gọi là remote repo
NHÁNH TRONG REPO // quan trọng 
bây h bỏ qua repo kia, tập trung nói về repio official này
branch nghĩa là nhánh
một local repo (tức là trong máy tính) hay remote repo ( tức lưu trên github) có thể có nhiều nhánh
khi bạn khởi tạo git init thì mặc định có 1 nhánh master







kiểm tra xem đang có  những nhánh nào trong local repo bằng lệnh git branch, nhưng trước tiên phải cd vào local repo đã

git branch // xem những nhánh trên local repp
nó hiện ra mỗi master tức bạn chỉ 1 nhánh tên là master, nhánh master tự được tạo ra khi bạn git init
muốn tao them nhanh moi , dung leny
git branch ten_nhanh_moi ten_nhanh_source
hoac
git branch checkout -b ten_nhanh_moi
lưu ý là những nhánh này đều cùng 1 repo
bây giờ kiểm tra nhánh bằngg git branch như trên
bạn đã có 2 nhánh, nhánh màu xanh và có dấu * là nhánh bạn đang ở
nhánh có tác dụng gì
là để tạo những luồng làm việc độc lập với nhau, ko liên quan gì với nhau, khi code trên nhánh này thì nhánhh kia ko bị ảnh hưởng
khi tạo ra nhánh mới thì nó sẽ có toàn bộ commmit và code như nhánh source của nó
xin lỗi nãy thiếu nhánh source , nếu  bạn ko điền thì nó sẽ lấy nhánh hiện tại(check nhánh hiện bằng lệnh git branch như trên đã nói) làm source,
và branh dược tạo sẽ có toàn bộ code và commmit giống  y hệt như source branch, thông thườn là bỏ qua ten_nhanh_source
để chuyển nhánh dùng
git checkout ten_nhanh_can_chuye (LƯU Ý LÀ NHÁNH PHẢI ĐƯỢC TẠO( TẠO BẰNG 2 CÁCH ĐÃ NÓI BÊN TRÊN ) RA RỒI, KO THỂ CHUYỂN ĐẾN 1 NHÁNH KO TỒN TẠI)
nó có chữ switch to.... gì đó
tức là đã chuyển và ko có lỗi
bây giờ check xem mình đã ở nhánh nào
nhánh màu xanh và có dấu * là nhánh bạn đang ở
lưu ý là khi mới tạo nhánh thì mình đang chưa ở nhánh đó, mà phải checkout tên nhánh thì mới ỏ nhánh đó và sau đó hãy git branch kiểm tra mình đang
ở nhánh nào
bây giờ tạo ra 1 file mới (file này là tạo ra trên nhán hiện tại ( là nhánh tes_code), nhánh khác ko liên quan)
đã tạo ra file  mới thì theo quy trình; phải git add rồi git commit
bây giờ trên  nhánh test_codeôó những file như trên
thử checkout sang nhánh master xem , hơi lỗi chút nãy chưa commmit xong, bây giờ checkout nha
ơ sao không add , commmit được file râđ me ta.







cd là change diretory (thay đổi thư mục)
diretory  =folder nghĩa là thư mục
cd bằng git bash
bạn tự cd đi
làm mẫu nhá
mặc định thì nó đang ở lenovo s145 nên mình phải về ổ C: ( có dấu hai chấm) trước, rồi mới dẫn vào repo
bạn tự cd tiếp đi 
hình dung bạn ở ổ C, bạn phải cd vào thư mục là con cỦA C, html css là cháu mấy đời  rồi ,ko cd thẳng vào được
mà phải cd dần dần
làm mẫu , nếu mà nhớ cấu trúc thưu mục thì cứ thế cd, ko thì vào this PC, từ tra vừa cd
bây giờ đã cd vào xampp rồi, thì cd tiếp con của xampp
ko biết con của xampp có folder nào thì vào this pc xem, cd đến khi nòa đến repo thì thôi
LÀMLẠI ĐI
OK ĐÚNG RỒI ĐÓ, CÓ 1 CÁCH KHÁC NHANH HƠN
đó là vào thẳng folder đó và "git  bash here"
thư mục hiện tại nó hiện trên đầu của git bash đấy nhá
cách này nhanh hơn cách cd , làm lại đi
ok đúng r
