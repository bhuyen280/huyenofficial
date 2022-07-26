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
ơ sao không add , commmit được file râđ me ta. à được ròi, chắc nó dở chứng tí ,hhhhhhh
bây giờ sau khi commmit trên  trên nhánh têst_code , thử check out sang master
à hiểu rồi, tức là tôi vùa commmit xong, lại viết lên đây, nên nó yêu cầu phải commit xong xuôi mới mới chuyển nhánh được
nhưng commit xong thì tôi lại viết tiếp ra đây , nên nó lại đòi commit tiếp, mới cho checkout s
bạn hiểu chỗ này ko có nha
bây h tôi sẽ commuit, xong viêt tiếp ra note pad







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
đã chuyển sang nhánh test_code
như bạn thấy code nó về đúng trạng thái của commit cuối (trên nhánh test_code)
mấy đoạn viết vùa rồi là viết trên master, nên nó ko hiện khi checkout sang test_code
bạn hiểu sự độc lập của các nhánh ko, có
 như bạn  thấy commmit mới nhất trên test_code là 4cbfb0c 
 nó khác với commit mới nhất trên master
 nhưng các commit kể từ trước  4cbfb0c   thì nó lại giống hệt (vì như đã nói, khi tạo ra nhánh mới, nhánh mới sẽ có toàn bộ commit của nhánh source
 và kể từ sau đó,  chúng nó mới bắt đầu khác nhau, khác về  mã code, nội dung commit, số lượng commit, vv......)
 bạn hiểu đoạn nayfy chuws, rồi nha
 lưu ý: nếu có thay đổi phải commit trước khi chuyển nhánh, như vừa nãy bị lỗi đó
 tất nhiên 2 nhánh vừa rồi đều thuộc 1 local repo
 nhưng nó  mới có trên local thôi, chưa có trên remote repo, tôi sẽ tạp trung làm việc với reop official thôi, còn repo text chưa bàn tới
 mới có 1 nhánh master trên remote
 nhưng trên local là có 2 branches








 để up load nó lên remote thì mình dùng lệnh
    $ git push --set-upstream ten_remote(chính là tên bí danh ấy) ten_nhanh_muon_up lên (chính là cái nhánh mà trên remote chưa có mà trên local đã có)
    (đoạn này sẽ phải đợi nó mọt vài giây, vì là upload mà, tùy vao tốc độ mạng)
    quay lạ remote check
    như vậy là đã có nhánh mới trên remote
    nó sẽ có toàn bộ code của nhánh đó trong lần commit cuối và có những lịch sự commit y hệt
    bạn hiểu chỗ này k có
    lệnh upstream này chỉ dùng 1 lần đầu khi nhánh mới tạo tạo local chưa có trên remote
    khi nó đã tạo ra trên remote rồi, từ lấn bạn dùng git push
    bạn giờ tạo ra thay đổi và push lên đi thạy đổi kiểu gì
    tạo ra file mới, hoặc xóa file đã có ,hoặc chèn , sửa, ........
    hỏi thật hay đùa đấy, kiểu vẫn chưa  hình dung ra là thêm xóa file, hay là thêm xóa text nào đó trong file (tùy mà, chủ yếu để check lệnh mới học, nên cứ thay đổi tùy ý)
    làm đi
    làm đi
    làm đi
    làm đi









  (xin lỗi hơi quên phải tra gg)
  mà còn nhớ bí danh là gì ko ta
  là tên thay thế hay đại diện cho url của remote repo https://github.com/bhuyen280/huyenofficial.git (đây là link của remote repo, có thể copy trên github)
  đó khi viết ra bí danh thì nó sẽ biết mình muốn up lên remote repo nào , thay vì phải viết url của remote repo dài như trên
  bí danh này do mình tự đặt, nên(nên thôi nha) đặt trùng tên repo tức là huyenofficial
  kiểm tra bàng lệnh git remote -v (ghi rồi đó, check lại đi)
  nó hiện ra 4 dòng như thực chất là có 2 remote repo nha, 1 repo thì có 2 link nó giống y nhau thôi  (push và fetch)
  để add remote repo thì tôi đã nói lần trước rồi, do mình đã add nên nó mới hiện ra như vậy
  lênh add như nào nhỉ , nhớ k
  git remote add bí danh + url nữa (đúng ko) đr, thiếu url, thì cái bí danh đó sẽ đại diện cho url đó, chỉ ra cho git biết muốn push lên url nào bằng cách gọi bí danh của
  có thể loại bỏ remote repo (chắc cái này chưa nói ha)chưa
  git remote rm tên_bí_danh
  hoặc
  git remote remove tên_bí_danh
  dùng cái nào cũng được , đã remove thì sẽ ko gọi nó ra được nữa, hoặc phải add lại , trức khi gọi
  tôi tạm remote cái binh đi
sau đó check ok r
  
     $ git branch --set-upstream  

 
