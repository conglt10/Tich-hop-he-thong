# Các bước triển khai tích hợp

### Bước 1: Clone source code tại đường dẫn [Github](https://github.com/conglt10/Tich-hop-he-thong)

### Bước 2: Tạo một repo mới với tài khoản github cá nhân

### Bước 3: Copy source code clone ở bước một và push lên repo ở bước 2

### Bước 4: Đăng nhập [CircleCI](https://circleci.com/) với tài khoản github cá nhân

### Bước 5: Liên kết CircleCI với repo github cá nhân vừa tạo

### Bước 6: Đăng ký tài khoản mới tại [Chatwork](chatwork.com) và [Slack](https://slack.com/) hoặc dùng tài khoản sẵn có

### Bước 7: Lấy API key của tài khoản chatwork

![](https://i.ibb.co/sKh6CsC/Screenshot-from-2019-12-31-14-09-33.png)

![](https://i.ibb.co/Gxv0HF9/Screenshot-from-2019-12-31-14-13-09.png)

### Bước 8: Tạo Bot Slack tại [đây](https://api.slack.com/messaging/webhooks)

### Bước 9: Thêm biến môi trường cho project trên circleCI

- CHATWORK_TOKENL: Là API Key của tài khoản chatwork
- CHATWORK_ROOM: Là room_id của box chat (dãy số đằng sau chữ rid trên url của box chat).

![](https://i.imgur.com/g1sEfcp.png)

![](https://i.ibb.co/FDRY4m7/Screenshot-from-2019-12-31-14-15-47.png)

### Bước 10: Thêm webhook url trong config chat notification ở circleCI

![](https://i.imgur.com/zymm1bP.png)

## Thử nghiệm

Khi đã hoàn thành các bước setup, khi chúng ta push code mới (hay merge code) trên github thì sẽ có thông báo gửi đến box chatwork và slack thông báo.

![](https://i.imgur.com/mGz1Qen.png)

![](https://i.imgur.com/IPB7KuY.png)
