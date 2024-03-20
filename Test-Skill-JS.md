## Bài kiểm tra kỹ năng sơ bộ

### Bài 1:

Chuyển số nguyên dương thành mảng nghịch đảo của các chữ số của số nguyên đó.

Cho một số ngẫu nhiên không âm, bạn phải trả về các chữ số của số này trong một mảng theo thứ tự ngược lại.

Ví dụ (Input => Output):

```
35231 => [1,3,2,5,3]
0 => [0]
```

### Bài 2:

Để có thể chuyển đổi đơn vị tiêu hao nhiên liệu từ
Dặm/gallon Anh (mpg) -> km/lít (kpl).

Hãy tạo một hàm trả về số thập phân là số km/lít (output) dựa trên số dặm/gallon(input).

Hãy đảm bảo làm tròn kết quả đến hai chữ số thập phân.

Một số liên kết hữu ích có liên quan đến bài toán này:

1 Gallon Anh = 4.54609188 lít
1 Dặm = 1.609344 kilomet

### Bài 3:

Tạo một ứng dụng trả về kết quả tính toán của quy luật sau:

- Input: Một số nguyên bất kỳ (nguyên âm hay dương đều được)
- Output: Là một số nguyên thỏa mãn luật số sau:

```
3 --> 15 ( 3 * 5¹)
10 --> 250 ( 10 * 5²)
200 --> 25000 (200 * 5³)
0 --> 0 ( 0 * 5¹)
-3 --> -15 ( -3 * 5¹)
```

Hãy tự tìm ra quy luật và giải bài toán.

### Bài 4:

Sau vòng bảng của một giải đấu bóng đá, ban tổ chức cần tính điểm của các đội

Kết quả trận đấu của mỗi đội được ghi lại trong một tập hợp các chuỗi. Mỗi trận đấu được biểu diễn bằng một chuỗi theo định dạng "x:y".

Trong đó x là số điểm của đội nhà và y là số điểm của đội khách.

Ví dụ đội ABC sẽ gửi cho ban tổ chức chuỗi sau: ["3:1", "2:2", "0:1", ...]

Điểm được ghi nhận cho mỗi trận đấu như sau:

- `x > y`: `3` điểm (`W - Win`)
- `x < y`: `0` điểm (`L - Lose`)
- `x = y`: `1` điểm (`D - Draw`)

Hãy tạo một function nhận vào mảng input theo mẫu trên và trả về số điểm của đội bóng tương ứng có được.

Ghi chú: Mỗi đội bóng luôn thi đấu 10 trận trong giải đấu.

- 0 <= x <= 4
- 0 <= y <= 4

### Bài 5:

Trên các cao tốc người ta thường đặt các cột đá ven đường để đánh đấu mốc km

Khoảng cách giữa các cột là như nhau và chiều rộng của các cột cũng như nhau.

Hãy tạo một hàm có 3 đối số:

- Số lượng cột (≥ 1);
- Khoảng cách giữa các cột (10 - 30 mét);
- Chiều rộng của cột (10 - 50 centimet).

Output cần tìm là khoảng cách giữa cột đầu tiên và cột cuối cùng tính bằng centimet (không tính chiều rộng của cột đầu tiên và cột cuối cùng).

### Bài 6:

Tính tổng của tất cả các số trong một mảng được cung cấp (list), trừ phần tử lớn nhất và nhỏ nhất (theo value, không phải theo index).

Phần tử lớn nhất hoặc nhỏ nhất chỉ được tính 1 lần, kể cả khi có 2 giá trị trùng nhau.

Chú ý về xác thực đầu vào.

Ví dụ

- `{ 6, 2, 1, 8, 10 } => 16`
- `{ 1, 1, 11, 2, 3 } => 6`

Nếu một giá trị rỗng (`null`, `None`, `Nothing` v.v.) được cung cấp thay vì một mảng, hoặc mảng được cung cấp là một danh sách rỗng hoặc một danh sách chỉ với 1 phần tử, trả về 0.

### Bài 7:

Bài toán sau là một biến thể của việc xác định các năm nhuận, giả sử chỉ sử dụng số nguyên và năm có thể là số âm và dương.

Viết một hàm sẽ trả về số ngày trong năm. Với năm được nhập vào dưới dạng một chuỗi.

Ví dụ: `yearDays(2000)` trả về `"2000 has 366 days"`

Chúng ta sẽ chấp nhận một số giả định: năm 0, ngay cả khi không có năm 0.

Ngoài ra, quy tắc cơ bản để xác minh một năm nhuận như sau:

Hầu hết các năm có thể chia hết cho 4 là năm nhuận.

Ngoại lệ: Năm thế kỷ KHÔNG phải là năm nhuận TRỪ KHI chia hết cho 400.

Vì vậy, các năm 0, -64 và 2016 sẽ trả về 366 ngày. Trong khi đó, 1974, -10 và 666 sẽ trả về 365 ngày.

### Bài 8:

Tạo một hàm có tên là `combineNames` chấp nhận hai tham số (tên và họ). Hàm này sẽ trả về họ và tên đầy đủ.

Ví dụ: `combineNames('James', 'Stevens')`

Output: `'James Stevens'`

### Bài 9:

Để tìm thể tích (centimet khối) của một hình hộp chữ nhật, sử dụng công thức:

`volume = Length * Width * Height`

Giả sử chúng ta chỉ có thể biết được volume, và length của một cạnh duy nhất!

Dựa vào 2 chỉ số trên, hãy xác nhận một hình hộp chữ nhật có phải khối lập phương hay không.

Hàm trả true nếu hình hộp chữ nhật là khối lập phương, trả về false nếu không.

Trả về false cho các số không hợp lệ (ví dụ: thể tích hoặc cạnh nhỏ hơn hoặc bằng 0).

Lưu ý: cạnh sẽ là một số nguyên

### Bài 10:

Tạo một hàm trả về tổng của hai số dương nhỏ nhất được cho trong một mảng chứa ít nhất 4 số nguyên dương. (Không có số thập phân hoặc số âm trong input)

Ví dụ:

- Input : `[19, 5, 42, 2, 77]`
- Output: `7`

Hoặc:

- Input : `[10, 343445353, 3453445, 3453545353453]`
- Output: `3453455`

### Bài 11:

Bob là một người phân biệt giới tính của gà. Công việc của anh ấy là phân loại gà con thành hai đống Đực (M) và Cái (F). Khi Bob không thể đoán được, anh ấy có thể giơ tay lên và tuyên bố với dấu '?'.

Cấp trên của Bob chưa tin tưởng vào khả năng của Bob, vì vậy họ đã giao cho anh ấy làm việc cùng với một người phân biệt giới tính chuyên nghiệp. Tất cả các quyết định của Bob sẽ được kiểm tra so với lựa chọn của chuyên gia để tạo ra một điểm số chính xác.

Quy tắc Điểm số
Khi họ đồng ý, anh ấy được 1 điểm.
Khi họ không đồng ý nhưng một người đã nói dấu '?' , anh ấy được 0.5 điểm.
Khi họ không đồng ý hoàn toàn, anh ấy được 0 điểm.

### Bài 12:

Chú T đã ứng tuyển việc làm là một nhân viên phân biệt giới tính gà trong nông trại.

Công việc của chú là phân loại gà con mới nở thành hai đống Đực (M) và Cái (F). Khi Chú T không thể phân biệt được, chú sẽ đánh kết quả là '?'.

Tuyển trạch viên chưa tin tưởng vào khả năng của chú T. Vì vậy chú cần tham gia một bài test cùng với một người phân biệt giới tính chuyên nghiệp.

Tất cả các quyết định của chú T sẽ được kiểm tra so với lựa chọn của chuyên gia để tạo ra một điểm số chính xác.

Quy tắc tính điểm như sau:

- Khi chuyên gia đồng ý với chú T, chú được 1 điểm.
- Khi chú T đánh '?' và chuyên gia cũng không phân biệt được, chú được 0.5 điểm.
- Khi chuyên gia báo sai, chú không có điểm.

Viết một function nhận vào mảng phán đoán của chú T và mảng kết quả của chuyên gia, mỗi mảng gồm 10 phần tử. Nếu điểm dưới 5 thì chú T trượt. Nếu đạt thì funciton trả về true, ngược lại trả về false.

### Bài 13:

Cho đầu vào là số nguyên. Hãy trả lại một hình vuông có chiều dài và chiều rộng bằng số nguyên đó. Số nguyên sẽ là một số nguyên dương từ 1 đến 50.

Ví dụ: `n = 3`, output sẽ là chuỗi sau:

```
+++
+++
+++
```

### Bài 14:

Cho 2 string array là a1 và a2, output là một array đã sắp xếp theo thứ tự `a-z`
Thảo 2 điều kiện:

- Là con của mảng a1
- Là chuỗi con của ít nhất 1 phần tử trong a2.

Ví dụ 1:

```
a1 = ["arp", "live", "strong"]
a2 = ["lively", "alive", "harp", "sharp", "armstrong"]
Output: ["arp", "live", "strong"]
```

Ví dụ 2:

```
a1 = ["tarp", "mice", "bull"]
a2 = ["lively", "alive", "harp", "sharp", "armstrong"]
Output: []
```

### Bài 15:

Bạn sẽ nhận được một mảng các số nguyên. Nhiệm vụ của bạn là lấy mảng đó và tìm index N sao cho tổng các số nguyên ở bên trái của N bằng tổng các số nguyên ở bên phải của N.

Ví dụ 1:

- Input: `{1,2,3,4,3,2,1}`
- Ouput: `3`, vì ở vị trí thứ 3 của mảng, tổng của phía bên trái chỉ mục đó ({1,2,3}) và tổng của phía bên phải của chỉ mục đó ({3,2,1}) đều bằng 6.

Ví dụ 2:

- Input: `{1,100,50,-51,1,1}`
- Ouput: `1`, vì ở vị trí thứ 1 của mảng, tổng của phía bên trái của chỉ mục đó ({1}) và tổng của phía bên phải của chỉ mục đó ({50,-51,1,1}) đều bằng 1.

Ví dụ 3:

- Input: `{20,10,-80,10,10,15,35}`
- Ouput: `0`, tại chỉ mục 0, phía bên trái là {}, phía bên phải là {10,-80,10,10,15,35}, chúng đều bằng 0 khi được cộng.

Lưu ý:

- Input: Một mảng số nguyên có độ dài 0 < arr < 1000. Các số trong mảng có thể là số nguyên dương hoặc số nguyên âm.
- Nếu bạn được cho một mảng với nhiều câu trả lời, hãy trả về index nhỏ nhất.
- Nếu không có index nào thỏa mãn, trả về -1.
