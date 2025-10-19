# 📝 Bài tập 1: Làm quen với Git cơ bản

**🎯 Mục tiêu:** Học cách fork, clone và tạo branch đầu tiên

**⏰ Thời gian:** 30-45 phút

**📚 Kiến thức cần:** Không cần kiến thức trước

---

## 🎯 Nhiệm vụ

### Phần A: Setup ban đầu (15 phút)

1. **Fork repo này về GitHub cá nhân**
   - Click nút "Fork" ở góc trên phải
   - Chọn account của bạn làm destination

2. **Clone repo về máy**
   ```bash
   git clone https://github.com/<your-username>/github-practice-beginner.git
   cd github-practice-beginner
   ```

3. **Kiểm tra thông tin Git**
   ```bash
   git config --global user.name "Tên của bạn"
   git config --global user.email "email@example.com"
   ```

### Phần B: Tạo branch và thực hiện thay đổi (20 phút)

4. **Tạo branch mới**
   ```bash
   # Thay "ten-ban" bằng tên thật của bạn (không dấu, không space)
   git checkout -b ten-ban/bai-tap-1
   ```

5. **Thêm tên vào file members.txt**
   - Mở file `members/members.txt`
   - Thêm thông tin của bạn theo format:
   ```
   - [Tên đầy đủ] - [Trường/Khoa] - [Email] - [GitHub username]
   ```
   
   Ví dụ:
   ```
   - Nguyễn Văn A - HUST/CNTT - vana@gmail.com - @vana123
   ```

6. **Commit thay đổi**
   ```bash
   git add members/members.txt
   git commit -m "Bài tập 1: Thêm thông tin cá nhân vào danh sách thành viên"
   ```
### Phần C: Push và tạo Pull Request (10 phút)

7. **Push branch lên GitHub**
   ```bash
   git push origin ten-ban/bai-tap-1
   ```

8. **Tạo Pull Request**
   - Vào GitHub repo của bạn
   - Click "Compare & pull request"
   - base: ten-ban/main compare ten-ban/bai-tap-1 (pull request từ nhánh bai-tap-1 về nhánh main)
   - Title: `[Tên bạn] - Hoàn thành bài tập 1`
   - Mô tả: "Đã thêm thông tin cá nhân vào danh sách thành viên"
   - Click "Create pull request"
---

## ✅ Checklist hoàn thành

- [ ] Đã fork repo thành công
- [ ] Đã clone về máy local
- [ ] Đã cấu hình Git user name và email
- [ ] Đã tạo branch mới với đúng format
- [ ] Đã thêm thông tin vào members.txt
- [ ] Đã commit với message rõ ràng
- [ ] Đã push lên GitHub
- [ ] Đã tạo Pull Request

---

## 🆘 Gặp lỗi?

### Lỗi thường gặp:

**1. Git không nhận diện username/email:**
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

**2. Permission denied (publickey):**
- Cần setup SSH key hoặc sử dụng HTTPS
- Xem hướng dẫn tại [common-issues.md](../resources/common-issues.md)

**3. Branch đã tồn tại:**
```bash
git checkout main
git branch -D ten-ban/bai-tap-1
git checkout -b ten-ban/bai-tap-1
```

---

## 🎉 Sau khi hoàn thành

Chúc mừng! Bạn đã hoàn thành bài tập đầu tiên. Bạn đã học được:
- ✅ Cách fork repository
- ✅ Cách clone về máy local  
- ✅ Cách tạo và chuyển branch
- ✅ Cách commit thay đổi
- ✅ Cách push lên GitHub
- ✅ Cách tạo Pull Request

**➡️ Tiếp theo:** [Bài tập 2 - Sửa lỗi Markdown](./bai-tap-2.md)
