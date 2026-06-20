# Chương 0: Lời giới thiệu (Introduction)

Chào mừng bạn đến với series Khoa học Máy tính (Computer Science)!

Series này gồm 13 chương, gói gọn những phần quan trọng nhất trong chương trình đại học Khoa học Máy tính — từ các nền tảng lý thuyết cho đến lập trình hệ thống và cả những công nghệ AI thời thượng nhất. Đọc xong series này, bạn sẽ có một bức tranh toàn cảnh cực kỳ vững chãi về thế giới khoa học máy tính.

---

## Câu chuyện của mình

Khi bắt đầu công việc lập trình viên đầu tiên, mình nhận ra bản thân có quá nhiều chỗ trống kiến thức. Có những khái niệm mình từng nghe loáng thoáng nhưng chưa bao giờ có thời gian tìm hiểu kỹ. Lúc đó thì cũng tạm ổn — ít ra mình còn biết sự tồn tại của chúng. Nhưng khi dừng lại để suy nghĩ sâu hơn, mình chợt nhận ra chiếc máy tính mình đang gõ hằng ngày giống như một chiếc hộp đen thần bí. Ai mà biết bên trong nó có cái gì? Code của mình thực sự chạy tới bộ vi xử lý (processor) bằng cách nào, và làm sao con chip đó biết phải làm gì với đống code đó? Rồi làm thế nào một máy chủ biết khi nào có request gửi tới và chúng đi đường nào? Mình có thể hiểu rất rõ một tầng ứng dụng ở trên, nhưng lại hoàn toàn mù tịt về tầng ngay bên dưới nó. Cảm giác lúc đó giống như mình đang xây dựng sự nghiệp trên bãi c\*t (cát) vậy.

Rõ ràng, giải pháp duy nhất là phải quay lại học những kiến thức nền tảng mà mình đang thiếu. Ở một góc độ nào đó, tự học khá là dễ vì tài nguyên trên Internet bây giờ nhiều vô kể và hoàn toàn miễn phí. Nhưng chính sự dư thừa đó lại dễ làm chúng ta bị "ngợp" và bất động nếu không biết bắt đầu từ đâu. Cuốn giáo trình nào mới thực sự hữu ích? Mình có thực sự cần biết mọi thứ họ dạy không, hay có những phần giờ đã lỗi thời rồi? Nên học các chủ đề theo thứ tự nào? AI tất nhiên có thể giúp ích rất nhiều, nhưng chúng ta cũng không thể tin tưởng hoàn toàn vào câu trả lời của nó.

---

## Series này giúp gì cho bạn?

Series này ra đời để làm người dẫn đường cho bạn. 13 chương được sắp xếp theo một lộ trình cực kỳ hợp lý, chương sau nối tiếp và xây dựng dựa trên các khái niệm đã giới thiệu ở chương trước. Mỗi chương sẽ tập trung vào những kiến thức thực tế giúp bạn nâng trình lập trình của mình lên. Mình luôn ưu tiên tính thực tiễn hơn là lý thuyết hàn lâm suông. Dù vậy, ở một số chỗ, các lý thuyết trừu tượng là không thể né tránh — nhưng tin mình đi, chúng cực kỳ thú vị! Cuối mỗi chương đều có một phần **Tài liệu đọc thêm** để gợi ý cho bạn tự nghiên cứu sâu hơn những chủ đề nâng cao mà khuôn khổ của series chưa nói hết được.

Khi đi qua từng chương, bạn sẽ thấy một số "chủ đề xuyên suốt" lặp đi lặp lại:

1. **Xây dựng các tầng trừu tượng (layers of abstraction) để quản lý sự phức tạp.** Chúng ta sẽ thấy mô hình này xuất hiện từ những cổng logic bé xíu trong chip xử lý cho đến tận những hệ thống phân tán khổng lồ.
2. **Những giới hạn vật lý và logic không thể vượt qua.** Có những bài toán đã được chứng minh là không thể giải được, hoặc những sự đánh đổi (trade-offs) mà bạn buộc phải chấp nhận. Những giới hạn này không phải là rào cản, mà là những biển chỉ dẫn giúp chúng ta biết điều gì là khả thi.
3. **Mọi thứ trong thế giới máy tính đều dựa trên các quy ước và cam kết (conventions & contracts) giữa các hệ thống để cùng nhau vận hành.**

Mình sẽ chỉ ra những chủ đề này khi chúng xuất hiện, nhưng bạn hãy cứ tinh mắt chú ý nhé, bạn sẽ thấy chúng ở những nơi không ngờ tới nhất đấy. Đây chính là những viên gạch nền móng để bạn xây dựng nên mô hình tư duy (mental model) của mình về máy tính.

---

## Một series thực tế và tinh gọn

Cuốn sách kinh điển _Modern Operating Systems_ (Các hệ điều hành hiện đại) dày tới 1136 trang. Cuốn _Database Systems: The Complete Book_ dày 1140 trang. Bộ _TCP Illustrated_ chỉ riêng tập đầu đã là 1060 trang! Một series tinh gọn như thế này không bao giờ có thể so bì về độ dày hay tính chi tiết với những cuốn "kinh thánh" đó được.

Để gói gọn cả một chương trình Computer Science vào một series duy nhất, mình đã phải chọn lọc cực kỳ kỹ lưỡng. Mình chỉ tập trung vào các chủ đề và khái niệm mà mình đã trực tiếp va chạm trong sự nghiệp lập trình của mình, bởi vì mình biết chắc chắn chúng quan trọng. Mục tiêu của mình không phải là dạy bạn mọi thứ trên đời, mà là vẽ bản đồ cho những vùng đất bạn chưa biết, giúp bạn có đủ kiến thức và sự tự tin để tự mình khám phá sâu hơn sau này.

Mình hy vọng bạn sẽ thích series này và thấy nó có ích. Nếu bạn có bất kỳ phản hồi hay góp ý nào, mình rất muốn được lắng nghe từ bạn!

Chúc bạn có một chuyến hành trình học tập thật vui vẻ!

---

[Tiếp theo: Chương 1: Lý thuyết tính toán (Theory of computation) &rarr;](./01_theory_of_computation.md)
