Nguồn mình lấy của bạn hàn lập, thấy viết khá hay và chi tiết dành cho người mới

fb:   https://www.facebook.com/groups/490627898299119/user/61555389550737/

blog: https://lephivu.substack.com/p/lam-the-nao-e-bat-au-voi-bug-bounty

# Bug-Bounty
Làm thế nào để bắt đầu với Bug Bounty

Làm thế nào để bắt đầu với bug bounty
Một số kinh nghiệm chia sẻ cho các bạn mới bắt đầu với bug bounty

Mar 22, 2025

Chào các bạn,

Disclaimer: Bài viết chỉ là quan điểm cá nhân của 1 hunter 1 năm kinh nghiệm, để cho người mới có thể tham khảo thôi nhé.

Mình là 1 bug bounty hunter kinh nghiệm hơn 1 năm. Mình chỉ tập trung mảng web application, một ít mobile app, và sau này sẽ học thêm phần này. Tóm lại mình chỉ chốt tập trung vào web app và app mobile.

Mình có note lại một số kinh nghiệm sau hơn 1 năm chơi bug bounty, khó khăn gặp phải, kinh nghiệm học, thực hành. Hi vọng có ích cho các bạn nào có ý định bắt đầu với bug bounty.

Trước khi bắt đầu, mình nói qua một số cái bắt buộc: 1 là tiếng Anh, 2 là kĩ năng tìm kiếm. Kĩ năng tìm kiếm rất quan trọng, trong bài ở một số phần mình sẽ để từ khóa cho các bạn tự tìm kiếm và tìm hiểu.

Web Pentest khác gì bug bounty hunter?
Quy trình thế này: Công ty thuê các pentester kiểm tra website, nên web pentest là người đầu tiên tiếp xúc với web app. Sau đó công ty đưa web app lên bug bounty program cho các hunters húp lại xem còn bug gì sót không

Như thế để thấy là Bug Bounty khó hơn rất nhiều so với Web Pentest > Nên cần phải cố gắng rất rất nhiều.

## 1. Bug bounty là gì?
Rất đơn giản, tìm lỗi cho các công ty và nhận tiền thưởng cho lỗi đó. Hãy chủ động tìm kiếm với Google:

bug bounty là gì?

what is bug bounty?

…

## 2. Làm thế nào để bắt đầu?
Lại vẫn là Google thôi. Sau này bạn sẽ biết có thể tìm bug thông qua Google dork.

Thực tế thì chỉ cần 1 cái trình duyệt, 1 công cụ bắt request là Burp Suite là có thể bắt đầu được

Môi trường của mình là: Hệ điều hành Linux, Burp Suite Pro, Firefox

Biết lập trình là 1 lợi thế lớn, thực tế có rất nhiều Developer chuyển qua làm Security và thành công

Nếu chưa biết lập trình, thì hãy học cơ bản HTML, Javascript

Javascript rất quan trọng, bạn có thể hiểu sâu nó càng tốt, để sau này hunt các lỗi client side, chủ ýếu là đọc từ code Javascript

Nếu là Linux thì nên biết bash cơ bản, sau này đến một thời điểm bạn sẽ dùng nó thường xuyên

Còn hiện tại hãy tạm thời bỏ qua nó

Tìm hiểu kĩ HTTP request > Tìm hiểu kĩ và hiểu nó nhé

Request data

Response data

## 3. Học tập trung 1 số loại bug hay học hết các loại bugs?
Chỗ này sẽ có 2 trường phái:

1 là tập trung vào 1 hoặc 2 bugs và chỉ hunt nó.

Chỉ học và hunt đúng các bug mình chọn, ví dụ XSS thì khi duyệt web/app bạn chỉ chăm chăm chọc cái này ngoáy cái kia để có thể ra bug XSS thôi

2 là hunt các loại bugs mà bạn biết

Test hết các loại bug mình biết

Thực tế thì kiểu nào cũng có người rất giỏi và thành công ở mỗi trường phái trên.

Theo mình thì 1-2 năm đầu nên tập trung vào 1 số bugs cơ bản dễ học, để đỡ bị ngợp: IDOR, XSS, Information Disclosure. Lại nói kĩ năng tìm kiếm: IDOR là lỗi gì?, XSS là gì? Information Disclosure là lỗi gì?…

## 4. Cân bằng giữa học và thực hành
Sau này bạn sẽ biết, mỗi một người sẽ có 1 phương pháp tiếp cận (hack) 1 website: cái đó gọi là methodology và nó là duy nhất của mỗi người

Và để có được methodology của bạn thì bạn phải thực hành rất nhiều và bạn sẽ tự rút ra được nên làm gì trước hay là có cái tips hay tricks gì khi hunt 1 website không, cái đó bạn phải trải nghiệm, và bạn sẽ nhớ. Còn nếu chỉ đọc của người khác thì 1 ngày, 1 tuần bạn có thể nhớ, nhưng sau 1 tháng mình nghĩ bạn sẽ quên ngay.

Có một cái những người mới hay mắc phải là vòng lặp learning vô tận, đang học cái A, lại tòi ra cái B, lại đọc B, tòi ra cái C… cứ thế nó sẽ thành 1 cái vòng lặp… rất mất thời gian và không có hiệu quả. Nên là hãy phân chia thời gian hợp lý. Theo mình thì 25-30% thời gian để học, còn lại là thực hành, và nên nhớ là áp dụng cái mình học vào thực hành nhé, chứ học cái A mà thực hành cái B thì hỏng.

## 5. Học ở đâu, thực hành ở đâu và học thế nào?
### 5.1 Học ở đâu và học thế nào?
Lại nói phần 4, học ở đâu cho hiệu quả.

Portswigger academy: Miễn phí thì có rất nhiều. Tốt nhất theo mình vẫn là portswigger academy (đây là keyword nhé)

Vào portswigger academy rồi pick 1, 2 loại bugs mà bạn muốn đào sâu, đọc lý thuyết rồi thực hành lab. Theo cái mục 3, bạn có thể theo gợi ý của mình: XSS, IDOR, Information Disclosure

Đọc writeup: write up là các bài viết cách tìm ra bug này bug nọ của các hunter khác. Hãy đọc và take notes sao cho đơn giản mà vẫn hiểu được khi đọc lại nhé

Twitter (X): Quên facebook đi, X mới là chân ái, hãy follow các pro security trên X, sẽ có rất nhiều tips/tricks được share

Keyword cho bạn là vào x.com tìm hashtag #bugbountytips

1 số pro: zeason, naham sec, jhaddix: hãy tìm và follow rồi đọc tweet, write up của các pro này

Hackerone Hacktivity: các report được disclose trên Hackerone

Tips là google dork site:hackerone.com tên bug

Ví dụ site: hackerone.com xss

Tips nữa là search top hackerone reports github

Google

Mình có cái kinh nghiệm riêng chỗ này là. Ví dụ mình tập trung vào XSS, thì mình sẽ lên mạng tìm tất tần tật các bài viết liên quan đến lỗi XSS, cách tìm nó, sau đó đọc và note lại nó, sau đó áp dụng vào lab (nếu đang học) hoặc program (nếu có kinh nghiệm rồi)

Mình nhắc lại là đừng có sa vào vòng lặp học và học như đã nói ở phần trên.
Theo kinh nghiệm 1 ngày, cái này chủ quan theo kinh nghiệm cá nhân của mình, bạn có thể thử rồi chỉnh sửa cho phù hợp

ít nhất 1h, tối đa 2h cho: Writeup, X, Google, Hackerone Hacktivity

1-2h cho làm lab, nhớ là làm lab cái lỗi nào bạn học ở trên nhé

Còn lại áp dụng cái đã học vào program

### 5.2 Thực hành thế nào
Quên mất cái này mình nói luôn vào chỗ 5.1 rồi nhé

Kinh nghiệm của mình chỗ này thì

Nếu có mentor dẫn dắt thì lên trình rất nhanh: Nhưng cái này khó, ko phải ai cũng sẵn sàng hướng dẫn bạn vô điều kiện

2 là tìm 1, 2 bạn đồng hành học cùng, có thể sau này làm 1 team

Nhiều cái đầu sẽ hơn 1 cái đầu

Cùng học tập chia sẻ với nhau để phát triển

Đỡ nhàm chán

## 6. Nói qua về Platform, Company, Program, Hunter
Company: là các công ty

Program: là chương trình bug bounty của 1 company. 1 Company có thể có 1 hoặc nhiều Program

Có 2 loại Program

VDP: là report và deck được tiền, chỉ được point hoặc Hall of shame

BBP: là report và nhận được tiền

Lưu ý là khi hunt 1 program nhớ đọc kỹ policy của họ, nhất là phần out of scope

Platform: thằng này cho phép Company tạo Program để cho các Hunter tìm bug và report

Có nhiều platform, nối tiếng là

Hackerone: Nổi tiếng nhất, lớn nhất

Bugcrowd: khá hard core, lúc nào có kinh nghiệm hãy vào

Synack: toàn các pro

Intigriti: Có vẻ phù hợp cho người mới

Mình khuyên nên pick Intigriti. Hoặc tùy bạn quan trọng là ở mình thôi.

Hunter: chính là bạn hướng đến, tìm lỗi và report kiếm tiền

## 7. First bug? Khó khăn gặp phải là gì?
Chà chà phần này hay nha.

Theo kinh nghiệm 1 năm của mình, 95% sẽ bỏ cuộc sau 6 tháng mà ko có bug nào.

Nói thế để biết tìm được first bug không phải dễ dàng. Nhưng cũng đừng nản chí vội, nó cũng không phải là quá khó khăn.

Mình liệt kê một số cái khó khăn gặp phải

Vòng lặp học, học và học: Như đã nói ở trên

Phân chia thời gian cho hợp lý, thời gian học <= 1/3 thời gian thực hành

Oải: sao lại oải?

1 tuần ko tìm được cái gì > ooh mình mới học thế là bình thường

1 tháng ko tìm được gì > ooh mới có 1 tháng và mình cũng mới bắt đầu, deck sao cả, cố gắng

3 tháng ko tìm được gì > ahh dm 3 thang rồi del có bug gì, lấy cái dell gì để thành toán bill đây > hơi nản

6 tháng ko tìm được gì > dmmm sao dell được cái gì cả. Nản vl. dell làm nữa.

Và bạn phải vượt qua nó, vẫn phải tiến lên. Nếu không tiến lên thì bạn sẽ góp phần vào 95% trên đó.

Nói phét thế, tiến lên thế nào nhỉ?

Mình cũng trải qua rồi, nói chung là rất oải, lạc lối, vì sau mình còn có gia đình nhỏ, bao nhiêu chi phí.

Có thời điểm 4,5 tháng mình không tìm được gì, bao nhiêu chi phí dồn lên đầu

Nhưng mình không bỏ cuộc vẫn phải tiếp tục thôi

Lại nói 6 tháng trên nếu bạn chăm chỉ theo cách phân chia thời gian trên, có thể bạn ko tìm được bugs hoặc có bugs Informative, Not capatable, hay Duplicate > Nhưng bạn sẽ có kinh nghiệm thực tế và nếu tiếp tục cái kinh nghiệm nó sẽ ++++ lên > Việc tìm được bug chỉ là sớm muộn thôi nhé.

Có một kinh nghiệm chỗ này nhé

Một là Nếu bạn tham gia X/Twitter: bạn sẽ gặp rất nhiều cái tweet kiểu như sau

Dm chúng mày ơi, tao vừa kiếm được 5k$ (5 nghìn đô nhé) ở Hackerone

Yay, I have awarded 30000$ at Hackerone…

Nếu có thấy các tweet đó, thường mình sẽ rất nôn nóng. Chỗ này mà nôn nóng là hỏng > Phải tìm cách vượt qua được, kệ mẹ nó nhé

Tức là không so sánh gì cả

Để được cái Tweet đó, thường các pro đó phải có >=2 năm hì hục ngày đêm

1 tweet đơn giản thế thôi, chứ để tìm ra nó có khi ông pro này hì hục bao ngày đêm với cái web app đó, chứ không phải tự nhiên có nhé

Và mình cũng tin là ông pro có cái tweets trên cũng trải qua các bước khó khăn mà mình liệt kê trên.

Hai là đừng để tiền nó chi phối bạn: Chỗ này hơi trừu tượng, tại vì nó sẽ làm cho tâm lý của bạn khó học, khó làm hơn.

Kiểu hãy học, hack vì đam mê, tiền nó sẽ tự đến… Đại khái là sau làm bạn sẽ hiểu, mình cũng dell biết giải thích sao

## 8. Bug bounty program
Ok đến được phần này. Ở đây lại có 2 trường phái

Một là wide scope program: là các chương trình mà scope rất rộng

keyword scope của program là gì > lại tìm kiếm nhé

ví dụ *.domain.com, các trang web của program đều nằm trong scope

Ví dụ công ty A: các tên miền mà công ty A quản lý thì bạn có thể tìm bug trên đó và report là hợp lệ

Cách này đòi hỏi bạn có khả năng fuzzing, tìm kiếm, sáng tạo

Vẫn phải hiểu được công ty này làm gì, sản phẩm là gì

Công ty có giá trị nào cần bảo vệ

Ví dụ thông tin khách hàng

Ví dụ thông tin backup

Ví dụ thông tin clients, orders payments

Những cái họ cần bảo vệ thì mình tìm cách chọc ngoái, tìm ra nó > bugs

Recon, keyword cho trường phái này là recon

Recon để tìm ra assets mới để hack vào

Hai là chỉ có 1 web site: Ví dụ app.domain.com

Nếu bạn hunt ở web site khác ngoài cái trên thì không hợp lệ - Out of scope

Cách này đòi hỏi bạn hiểu sâu về web app đó

Hãy dùng web app thường xuyên như 1 người dùng bình thường,

dùng đến mức mà bạn hiểu web site đó, có chức năng gì, có đối tượng gì…

Dùng đến mức thành thạo hơn cả ông Dev viết ra cái web site đó

Nếu bạn làm đến bước này > sớm hay muộn bạn sẽ tìm ra được bug

## 9. Kinh nghiệm của mình
Chọn 1 program public cũng được không sao cả, sao cho

Web app cực kì phức tạp

Web app có nhiều tính năng

Có phân quyền người dùng càng tốt

Tìm hiểu web app đó hoạt động thế nào, hiểu rõ luồng lạch của web app đó

Sử dụng app như người dùng bình thường, dùng đến khi bạn có thể hiểu được tất tần tật các chức năng của web app đó

Với trường phái này mình khuyên bạn theo pro này https://www.bugbountyhunter.com/methodology/zseanos-methodology.pdf

Pro này là zseano: top 1 chương trình Amazon bug bounty. Ông này chỉ hunt mỗi Amazon và hình như đâu đó 7 năm rồi, đến mức ông hiểu hết các chức năng, các website của Amazon hơn cả Dev

Hãy in ra giấy và rảnh cứ lôi ra đọc.

Cố gắng lên, Việt Nam mình rất nhiều anh tài ẩn mình. Phải bơi ra biển lớn tranh tài với các quốc gia khác chứ không phải ở Việt Nam mình.

Chúc các bạn may mắn và vượt qua được cái cột mốc first bug.

Yoo!
