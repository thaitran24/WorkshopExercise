# Exercises
## Question 1
Như bạn đã biết, mỗi commit đều có một mã riêng (ID) của nó. Giả sử bạn có một commit với cột mốc quan trọng (dự án đã chạy tốt ở commit này), sau đó bạn có vài chỉnh sửa và thêm một số commit nữa. Muốn quay lại một commit cột mốc đó, chúng ta có thể sử dụng mã của commit đó với lệnh `git checkout`. Hãy tìm cách để có thể quay lại commit cột mốc đó mà không sử dụng mã của commit đó. Ví dụ với hình bên dưới, làm sao để quay về commit c3 mà không sử dụng mã "c3".

<p align="center">
  <img src="https://raw.githubusercontent.com/thaitran24/WorkshopExercise/master/ex1.PNG">
</p>

## Question 2
Như bạn đã biết, các stash lưu lại công việc chưa được commit tại một branch. Xét một trường hợp cụ thể sau đây:
- Dự án của bạn có một file `exercise.txt` với nội dung như sau:
```
Hello 2022!
Workshop Git
TickLab
```
- Dự án đang có hai branch `master` và `test` đều được commit file `exercise.txt`.
- Tại branch `master`, hãy thêm ở dòng 4 nội dung "Master". Sau đó chuyển qua branch `test`.
- Tại branch `test`,  hãy thêm ở dòng 4 nội dung "Test". Sau đó `stash` công việc và quay trở lại branch `master`.
- Tại branch `master`, sử dụng lệnh `git stash pop`.

Bạn hãy theo dõi hành vi của Git và giải thích.

## Question 3
Xét trường hợp sau đây:
- Dự án của bạn có một file `exercise.txt` với nội dung như sau:
```
Hello 2022!
Workshop Git
TickLab
```
- add và commit file `exercise.txt` tại nhánh `master`.
- Tạo một nhánh mới tên `test`.
- Tại branch `master`, bạn thêm nội dung "Test" tại dòng 4 của file `exercise.txt` và commit file đó.
- Tuy nhiên, bạn phát hiện ra commit đấy đáng lẽ phải ở branch `test`.

Làm sao để bạn có thể chuyển những thay đổi trong commit ở branch `master` sang branch `test`?
