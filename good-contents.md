# Good contents

## Giới thiệu về [hệ thống MCI của Windows](https://msdn.microsoft.com/en-us/library/windows/desktop/dd757151%28v=vs.85%29.aspx) - **Meigyoku Thmn**

> Về cơ bản thì đây là 1 hệ thống để play video trong Windows<br>
> ý tưởng thì đơn giản: dùng 1 hwnd, bind một video vào nó, rồi play nó, nó sẽ play async với app của mình<br>
> hwnd đó của mình sẽ hiện đúng cái video đó luôn<br>
> còn muốn làm thêm thanh slide các kiểu thì dựa 100% vào hệ thống message event<br>
> play nhạc cũng được và thậm chí mở ảnh gif<br>
> cái này mà code được thành module cho javascript thì hơi bị hay, vì nó là async<br>
> 2 project trên codeproject điển hình nhất là:
> - [Fun-with-Video](https://www.codeproject.com/Articles/785008/Fun-with-Video)
> - [MFC-Wrapper-Class-for-MCIWnd](https://www.codeproject.com/Articles/3500/MFC-Wrapper-Class-for-MCIWnd)
> 
> Tương ứng với 2 loại API để tiếp cận MCI<br>
> rất nhiều game ngày xưa xài cái này để chạy cutscene<br>
> nếu video được bật với device type là mpegvideo<br>
> thì nếu máy có directvobsub và file phụ đề (ass, srt) bên cạnh<br>
> thì nó load cùng luôn, mà máy còn phải có lav decoder hoặc ffdshow decoder nữa<br>

## Giải thích dễ hiểu nhất về Big Data - **Library**

> tớ sẽ giải thích từ việc đưa ra 1 vấn đề, và cách giải quyết vấn đề đó<br>
> cơ mà, tớ ko phải chuyên gia về big data, nên có thể điều tớ nói ko đúng. Nếu sai thì cậu cứ góp ý nhé 😄<br>
> giờ tưởng tượng, cậu là 1 genius kid, được học sinh giỏi liên tục 9 năm, được giải thành phố môn tin học<br>
> hiệu trưởng rất ấn tượng về cậu, nên nhờ cậu giải quyết 1 bài toán mà bác ấy rất đau đầu<br>
> đấy là làm thế nào để thống kê ra những học sinh có thành tích học tập xuất sắc như cậu, để từ đó bồi dưỡng, cho đi học Harvard hay làm hacker gì đó<br>
> bác ấy cũng ko biết nhiều về lập trình, và cũng lười<br>
> nên nhờ cậu giúp<br>
> để giải quyết công việc đó, cậu cần phải thu thập được thông tin, đấy là dữ liệu điểm thi của các học sinh toàn trường<br>
> may mắn là cậu đã có các cô giáo giúp, nên cậu có 1 tập các file text chứa điểm đó<br>
> cái việc từ dữ liệu thô, ra dữ liệu báo cáo những genius kid, đc gọi là xử lý dữ liệu<br>
> với dữ liệu toàn trường tầm vài trăm người, cậu nghĩ "cái này ko khó lắm, chỉ cần 1 script để trích xuất ra điểm, rồi lọc ra những người có điểm cao, và tóm gọn nó thành 1 bản báo cáo là đủ"<br>
> nếu cậu chưa biết, script là 1 chương trình nhỏ, nhằm thực hiện 1 công việc nhanh nào đó. Nó thường ngắn gọn và dễ viết<br>
> thế là cậu viết 1 script python khoảng 50 dòng, chạy 1 phát ra 1 report những wonderkid<br>
> rồi, để ý mấy chữ in đậm nhé cậu<br>
> cậu phải trích xuất (map), lọc (filter) và tóm gọn (reduce) cho công việc này<br>
> đó thực ra là 3 thao tác cơ bản khi cậu làm việc với dữ liệu 😄<br>
> giờ, thầy hiệu trưởng của cậu rất hài lòng, thầy ấy đi khoe khắp nơi rằng thầy ấy đã giải quyết đc vấn đề đau đầu đó<br>
> tiếng lành đồn xa, sở giáo dục nghe đc điều đó<br>
> họ mời cậu tới và nhờ cậu làm việc đó với toàn bộ học sinh trong thành phố, ở cả 3 cấp<br>
> cậu đồng ý nhanh chóng, rất tự hào vì điều đó<br>
> nhưng khi cậu bắt đầu làm, cậu nhận ta số lượng dữ liệu của cậu ko còn là vài trăm, mà là vài trăm nghìn<br>
> cậu gặp khó khăn, vì lúc này script của cậu sẽ tốn thời gian hơn, tiêu tốn cpu với ram hơn để làm<br>
> vì thế cậu quyết định: đưa tất cả bản ghi vào trong csdl. Cậu chỉ cần index hợp lý là cậu sẽ có thể đưa ra report rất nhanh, mà hiệu quả nữa<br>
> cậu viết 1 script để insert vào csdl<br>
> rồi viết 1 trang web nhờ vào việc cậu đang học lập trình mảng ứng dụng web<br>
> nó là cơ hội tốt để cậu tập tành skill đó<br>
> sau 2 tháng, 1 trang web đc hoàn thành<br>
> sở giáo dục rất hài lòng, và trong báo cáo cuối năm, họ đưa cậu vào trong báo cáo đó<br>
> khiến bộ giáo dục rất bất ngờ<br>
> họ lập tức mời cậu tới, nhờ cậu làm điều tương tự với hs cả nước<br>
> và hi vọng cậu sẽ giải quyết vấn đề của họ, tìm ra những wonderkid để bồi dưỡng tài năng<br>
> cậu hơi do dự, nhưng rồi cũng đồng ý, sau khi bộ trưởng hứa sẽ giúp cậu đi du học Harvard<br>
> và nhanh chóng, cậu nhận ra dữ liệu của cậu là hàng triệu<br>
> và csdl của cậu trả về report sau hàng giờ<br>
> cậu tốn vài tuần để thử optimize tất cả các câu query, tuning csdl và website của cậu<br>
> nhưng vô vọng<br>
> rồi cậu đọc đc đâu đó, có 1 thứ là elasticsearch, cái này đc dùng chuyên để search<br>
> cậu nghĩ: nó có thể có ích<br>
> sau khi làm thử 1 số prototype, cậu nhận ra nó rất nhanh<br>
> nên cậu viết 1 script để migrate csdl của cậu sang elasticsearch<br>
> và kaboom, report đc xuất ra sau vài s<br>
> cậu đc đi du học Harvard<br>
> bộ trưởng bộ giáo dục rất vui, cậu đc gọi tới khen thưởng<br>
> rồi bác chủ tịch nước sau 1 hôm đi công du Mỹ, đã nói với Trump<br>
> Trump rất ấn tượng, và đưa vấn đề này lên LHQ<br>
> họ gọi cậu tới và mong cậu làm điều tương tự cho toàn thế giới<br>
> tới đây, cậu nhận ra<br>
> "oh my big data"<br>
> tớ nghĩ là qua ví dụ giải quyết vấn đề trên, cậu đã hiểu:<br>
> 1. Xử lý dữ liệu là gì
> 2. Tại sao phải xử lý nó - để đưa ra các dữ liệu có ý nghĩa, nhằm mục đích phân tích
> 3. Vấn đề khi xử lý dữ liệu, cùng 1 số cách giải quyết khi lượng dữ liệu ở vài trăm, vài trăm nghìn, vài trăm triệu
> 4. Làm sao để xử lý vài tỷ dữ liệu
>
> mục 4 tớ chưa đề cập tới đâu 😄<br>
> giờ thử xem họ làm thế nào với vài tỷ record dữ liệu nha<br>
> cậu biết cậu phải xử lý khối dữ liệu lớn. "đây là big data trong truyền thuyết" - cậu nghĩ<br>
> thế nên cậu về, thuê server, setup apache hadoop<br>
> lúc này, cậu phân phối dữ liệu lên các server khác nhau<br>
> lúc này, việc cậu làm là để feed data vào hadoop<br>
> để nó phân phối dữ liệu lên các server khác nhau<br>
> rồi khi cậu query, cậu sẽ định nghĩa các script hướng dẫn map dữ liệu như thế nào<br>
> reduce ra sao<br>
> hadoop sẽ lo phần còn lại cho cậu<br>
> đó là cách mà họ xử lý big data: phân phối nó ra nhiều server, và tìm kiếm song song trên đó<br>
> 1 cách đơn giản nhất là vậy<br>
> tới đây, tớ nghĩ là cậu đã hiểu rõ, phải ko? 😄

## Cách đọc code - **Library**

> Nếu cậu đọc code không hiểu, khả năng là cậu thiếu căn bản.
> 
> Tớ recommend cậu làm thế này nha:
> * Đọc code structure để biết các yếu tố cơ bản của project.<br>
> Tớ recommend đọc từ mô tả thư viện, các file config, rồi đọc code xem kiến trúc mà họ theo là gì.<br>
> Sẽ có nhiều thư viện cậu không hiểu, hay các config khó hiểu, nhưng cậu chỉ cần biết nó được dùng để làm gì. Những cái nào chưa biết, cậu nên note lại để hỏi senior member.<br>
> Điều này sẽ giúp cậu nhớ được nơi cần tìm thông tin cần thiết.
> * Đọc yêu cầu mà task của cậu giao cho thật kỹ, và *chỉ* tìm code liên quan tới phần này.<br>
> Tớ biết rất nhiều novice sẽ đi đọc rất xa ở những chỗ mà không liên quan, nhưng cậu cần hoàn thành công việc trước khi làm việc đó.<br>
> Nếu có những cài đặt khó hiểu, cậu có thể check test case để biết cách sử dụng của nó, hoặc debug (kiến thức từ recommend đầu tiên sẽ giúp cậu) để kiểm tra flow.
> * Note lại những điều cậu chưa hiểu, và hỏi càng sớm càng tốt.<br>
> Nếu cậu không hỏi, *kể cả những câu hỏi đơn giản và ngu ngốc*, cậu sẽ không biết. Hỏi một câu hỏi ngu ngốc sớm so với hỏi câu hỏi ngu ngốc sau 6 tháng sẽ hoàn toàn khác nhau 😄
> * Nếu đọc được requirement là điều tốt nhất. Hẳn nhiên cậu sẽ khá tốn thời gian ở giai đoạn đầu, nhưng về sau sẽ ổn hơn.<br>
> Cậu nhớ đừng đọc lan man quá. Tớ chứng kiến nhiều novice member đọc cả code project khác khi làm việc rồi.
> 
> Khi cậu đọc task & yêu cầu cần làm, cậu phải chắc chắn hiểu rõ tất cả mọi thứ về yêu cầu đó, trước khi thực sự code.<br>
> Nếu cậu có requirement, đọc hết requirement liên quan tới phần đó, đồng thời cũng đọc tất cả các reference từ ticket + requirement. Việc này sẽ hơi tốn thời gian, nhưng so với  thời gian cậu cứ nhận bug, sửa lỗi nhiều lần chỉ vì cậu không hiểu rõ yêu cầu, thì thời gian này ít hơn nhiều.<br>
> Nếu có bất cứ thắc mắc, một lần nữa cậu nên hỏi ngay lập tức.
> 
> Thời điểm này cậu không có shortcut nào đâu. Khi cậu hình thành được framework của riêng mình, lúc đó cậu mới biết shortcut.<br>
> Cho tới lúc đó, cậu buộc phải bỏ công ra thôi 😄
