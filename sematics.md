# Tìm hiểu về các semantic tags trong HTML5
## 1. Thẻ < section >
- Thẻ section dùng để phân chia các phần riêng biệt của trang HTML, ví dụ trong trang có các phần như About, Contact,... thì các phần này sẽ được bọc trong các thẻ section

## 2. Thẻ < article >
- Thẻ article dùng để chứa các nội dung độc lập trong trang. Những nội dung này có thể được cắt ra mang đi nơi khác mà người dùng ở nơi khác đọc vẫn có thể hiểu được, không phụ thuộc vào nội dung chứa trong trang.

## 3. Thẻ < nav >
- Thẻ nav thường dùng để list các thẻ a, dùng trong thẻ header hoặc thẻ footer để list danh sách các link 

## 4. Thẻ < aside >
- Thẻ aside chứa 1 số thông tin bên lề nội dung chính của trang. Những nội dung chứa trong aside có thể bị xóa đi mà không làm ảnh hưởng đến nội dung chính của trang. Lưu ý, nếu aside nằm trong thẻ article thì nội dung nằm trong thẻ aside đó chỉ chứa thông tin bên lề nội dung chính của article chứ không phải của toàn trang.

## 5. Thẻ < main >
Thẻ main dùng để chứa nội dung chính của trang, nó sẽ không chứa các thông tin như header, footer, aside,... hoặc những gì thuộc phần intro,...

Trong 1 trang chỉ có 1 thẻ main duy nhất

## 6. Thẻ < div >
- Thẻ div là thẻ không hề có Semantic meaning. Nó chỉ dùng để bọc những nội dung có liên quan đến nhau lại. Khi không tìm được thẻ thích hợp để bọc phần nội dung đó thì ta sẽ sử dụng thẻ div.

- Ví dụ như phần intro của trang web, nó không thể nằm trên header cũng không thể nằm trong main, khi ấy ta sử dụng thẻ div để bọc các thông tin đó lại.

- Ngoài ra, người ta còn sử dụng thẻ div để bọc những nội dung cần format giống nhau bằng CSS, cũng như tách trang thành từng phần nhỏ, để trình duyệt có thể render từng phần 1, tăng tốc độ hiển thị đến người dùng thay vì phải load toàn bộ trang mới render.
- Thẻ div là dạng block

## 7. Thẻ < header > và < footer >
- Thẻ header bọc những thông tin giới thiệu về toàn trang web hoặc navigation bar
- Thẻ footer bọc những thông tin về trang web, thẻ footer của toàn trang thường chứa contact information, copyright information,...

## Áp dụng 
```html
<!DOCTYPE html>
<html>
 <head>
   <title faricon="">Review sách Trại Hoa Vàng</title>
   <link rel="icon" type="image/x-icon" href="data:image/jpeg;base64,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"
  </head>
  
 <body>
   <div>
     <header>
       <h1>Cảm nhận từ người đọc Trại Hoa Vàng</h1>
       <p>Một blog nhỏ chia sẻ về cuốn sách Trại Hoa Vàng</p>
       
       <nav>
         <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/#about">About</a></li>
          <li><a href="/#articles">Articles</a></li>
          <li><a href="/#contact">Contact</a></li>
         </ul>
        </nav>
      </header>
      
     <article id="review-THV">
       <header>
         <h2>Review Trại Hoa Vàng</h2>
         <p>By: Mon - NTB98</p>
         <p>Publish: 10/01/2022</p>
         <h2>Thông tin cuốn sách</h2>
         <p>Tên sách: Trại Hoa Vàng</p>
         <p>Tác giả: Nguyễn Ngọc Ánh</p>
       </header>
       
       <img src="https://vcdn.tikicdn.com/media/catalog/product/t/r/trai-hoa-vang.jpg" alt="thông tin quyển sách">
       
       <p>"Trước nay, ba tôi vẫn thường hay để ý đặc biệt đến cách ăn mặc của tôi. Không hiểu nghe lỏm được ở đâu, ông cứ đinh ninh chuyện quần áo liên quan mật thiết đến tính khí con người. Hễ ăn mặc giản dị, thanh bần mới là người chăm học. Còn ai quần áo đẹp đẽ đều được ông liệt vào dạng ăn chơi, đàn đúm. "Mốt miếc" ông càng ghét tợn. Năm ngoái, thanh niên toàn thị trấn đều mặc quần ống chật, cỡ 16-18 li, ông bắt tôi may quần 28 li, đi quét đất hệt nhu bà nội tôi. Ngày đi may đồ mới, cả thế giới ai cũng hồi hộp vui mừng, chỉ riêng tôi là khóc nức nở"</p>
       <p>Đó là phần trích đoạn trong phần giới thiệu ở cuối cuốn sách Trại Hoa Vàng. Các bạn thấy đó, một câu chuyện của một cậu bé từ một thời đại khác với những gì chúng ta, những gen Z trải qua. Vậy đâu là lý do một người lười đọc sách như tôi thích thú đọc hết cuốn sách này. Tôi tìm đến Trại Hoa Vàng, không vì phần nội dung giới thiệu của sách làm mình thấy thích thú và muốn tìm hiểu, ban đầu, tôi đọc vì thích nhà văn. Đúng vậy, lối hành văn trong các tác phẩm của nhà văn Nguyễn Nhật Ánh đều có một nét đặc trưng chung, tôi gọi đó là dấu hiệu nhận biết về sách của ông. Những cuốn sách như những món quà dành cho những tâm hồn cần được trẻ lại, bình yên hơn và được chữa lành. Trại Hoa Vàng cũng vậy, nó giản dị, đời thường và mang lại nhiều thích thú cho người đọc. Một câu chuyện tình yêu ngọt ngào thời học sinh, có rung động, có lo lắng, sợ hãi, lén lút, cũng có vui vẻ và cả nuối tiếc . Tất nhiên tôi chưa từng trải qua những câu chuyện đó nên Trại Hoa Vàng không phải thu hút tôi bởi đem lại những ký ức tuổi thơ, nhưng mỗi trang, mỗi dòng luôn cuốn tôi theo câu chuyện của Chuẩn. Tôi muốn biết rồi "thằng đầu bò, không được thông minh cho lắm" như Chuẩn tự nhận về mình có cố gắng học tập và thi đậu để có được "Huy chương vàng" hay không. Vui vẻ với tình bạn của Chuẩn, Cường và Phú ghẻ. Muốn xem bé Thảo có tình ý gì với ông anh Chuẩn trồng một vườn hoa đẹp ơi là đẹp? Và câu chuyện tình cảm của Chuẩn và Cẩm Phô làm tôi nhớ về những rung động thời còn cắp sách đến trường. Mọi thứ nhẹ nhàng, bình dị. Lôi cuốn người đọc thư thả tâm hồn mà chiêm ngưỡng câu chuyện của những đứa trẻ ấy, để nhẹ nhàng hơn, vui vẻ hơn.</p>
       <p>Tất nhiên, sách sẽ phù hợp với những bạn đang đi tìm chút bình yên, giản dị trong cuộc sống xô bồ, vội vã này. Nó không dành cho những bạn đang muốn đọc để thu nạp thêm nhiều kiến thức mới, kỹ năng mền hay đại loại thế...</p>
     </article>
     
     <aside>
      <h3>Có thể bạn quan tâm</h3>
       <ol>
        <li>
            <img 
                src="https://bnabooks.vn/wp-content/uploads/2021/09/SXCpimR3large.jpeg"
                alt="Tôi thấy hoa vàng trên cỏ xanh"
                width="59"
                height="59">
            <a href="#">Review sách Tôi Thấy Hoa Vàng Trên Cỏ Xanh</a>
        </li>
        <li>
            <img 
                src="https://nhungcuonsachhay.com/wp-content/uploads/2021/04/Mat-biec-Nguyen-Nhat-Anh.jpg"
                alt="Mắt Biếc"
                width="59"
                height="59">
            <a href="#">Review sách Mắt Biếc</a>
        </li>
        <li>
            <img 
                src="https://bnabooks.vn/wp-content/uploads/2021/09/SXCpimR3large.jpeg"
                alt="Mắt Biếc"
                width="59"
                height="59">
            <a href="#">Review sách Bồ câu không đưa thư</a>
        </li>
        <li>
            <img 
                src="https://bnabooks.vn/wp-content/uploads/2021/09/SXCpimR3large.jpeg"
                alt="Mắt Biếc"
                width="59"
                height="59">
            <a href="#">Review sách Làm bạn với bầu trời</a>
        </li>
       </ol>
     </aside>
    <footer>
     <p>©2022 MON, The Blog</p> 
    </footer>
  </div>
  </body>
</html>
```