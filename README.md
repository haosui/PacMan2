# PacMan2
Câu 1:
Hàm đánh giá:
gồm 3 trường hợp: 
biến ret
+ Nếu ma ở gần. return ret (= -1000) nếu kc nhỏ hơn 2,  giảm hàm ret đi tùy theo khoảng cách với ma, tối đa 5 ô
+ Nếu thức ăn ở vị trí đang xét và không xảy ra trường hợp <2 ô. thì return ret += 1000
+ Nếu không thì trả về khoảng các mahatan đến thức ăn gần nhất +ret

Câu 2:
Minimax
Chúng ta có hàm đệ quy:
+ Điều kiện dừng:
-depth =4
- win/lose
+ vào mỗi lần gọi value nếu index = 0 thì gọi hàm max, nếu không thì gọi hàm min
+Hàm max:
-lấy ra tất cả các state có thể của pacman, gọi hàm value với mỗi hướng và lấy max của nó tăng index lên 1.
khi tăng index lên 1 tức là nó khác 0. vòng value vừa gọi sẽ gọi hàm min
+Hàm min
- lấy ra tất cả state hướng có thể đi của ma, gọi hàm value với mỗi hướng và lấy min của nó, tăng index lên 1 để gọi con ma tiếp theo 

Câu 3 tương tự câu 2
với mỗi lần gọi ta lưu 2 biến alpha beta,
khi đang xét hàm max nếu giá trị đang xét mà lớn hơn beta, thì return luôn giá trị đó k xét nhánh đó nữa vì chắc chắn beta sẽ không lấy nhánh ddang xét vì có beta tốt hơn rồi.
Nếu giá trị đang xét thì lớn hơn alpha thì cập nhật alpha hiện tại , vì alpha la tốt nhất của giá trị max
Khi xét hàm min 
hàm min là hàm lấy giá trị nhỏ nhất trong các state 
Nếu có một stat nhỏ hơn alpha thì chắc chán alpha sẽ không lấy giá trị nào ở nhánh này vì khiểu gì hàm min sẽ cũng sẽ lấy giá tị nhở hơn bằng giá trị đang xét vad alpha sẽ không lấy nó.
nếu có beta nhỏ hơn thì cập nhật beta.

Câu 4.
chúng ta đang xét hàm min không phải là tối ưu, vì vậy ta lấy giá trị trung bình của tất cả các trường hợp của hàm min, 




https://www.coursera.org/learn/introduction-to-cloud/home/welcome
https://www.bmc.com/blogs/saas-vs-paas-vs-iaas-whats-the-difference-and-how-to-choose/
https://www.coursera.org/learn/aws-iot-developing-and-deploying-an-internet-of-things

