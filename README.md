# Github
các câu lệnh thường sử dụng
**1.Khởi tạo và cài đặt kho lưu trữ
git init: Tạo một kho lưu trữ Git mới trong thư mục hiện tại.
git clone <URL>: Sao chép một kho lưu trữ từ xa về máy cục bộ.
**2. Làm việc với các thay đổi trong kho lưu trữ
**git add <file>: Thêm file cụ thể vào "staging area" để chuẩn bị cho commit.
git add .: Thêm tất cả các thay đổi trong thư mục hiện tại vào "staging area".
git status: Kiểm tra trạng thái của các file (đã thay đổi, đang ở "staging area", chưa được theo dõi).
git diff: Hiển thị các thay đổi chưa được thêm vào "staging area".
git diff --staged: Hiển thị các thay đổi đã thêm vào "staging area" nhưng chưa commit.
**3. Commit các thay đổi
**git commit -m "message": Commit các thay đổi trong "staging area" với một thông điệp.
git commit -a -m "message": Commit tất cả các thay đổi của file đang theo dõi, bỏ qua "staging area".
git commit --amend: Sửa đổi commit cuối cùng (sửa thông điệp hoặc thêm file).
**4. Làm việc với các nhánh (branches)
**git branch: Hiển thị danh sách các nhánh hiện có.
git branch <branch-name>: Tạo một nhánh mới.
git checkout <branch-name>: Chuyển sang nhánh khác.
git checkout -b <branch-name>: Tạo và chuyển ngay sang nhánh mới.
git merge <branch-name>: Gộp nhánh đã chọn vào nhánh hiện tại.
git branch -d <branch-name>: Xóa nhánh đã chọn (sau khi đã merge).
**5. Làm việc với kho lưu trữ từ xa (remote repository)
**git remote add <name> <URL>: Thêm một kho lưu trữ từ xa.
git remote -v: Hiển thị danh sách các kho lưu trữ từ xa.
git push <remote> <branch>: Đẩy nhánh hiện tại lên kho lưu trữ từ xa.
git push -u <remote> <branch>: Đẩy nhánh lên kho lưu trữ từ xa và theo dõi nhánh đó.
git fetch <remote>: Lấy dữ liệu từ xa về nhưng không gộp vào nhánh hiện tại.
git pull <remote> <branch>: Lấy dữ liệu từ xa và gộp vào nhánh hiện tại (kết hợp fetch và merge).
**6. Xem lịch sử và thông tin commit
**git log: Hiển thị lịch sử commit của dự án.
git log --oneline: Hiển thị lịch sử commit dưới dạng ngắn gọn.
git log --graph --oneline: Hiển thị lịch sử commit dưới dạng đồ thị ngắn gọn.
git show <commit>: Hiển thị chi tiết về một commit cụ thể.
**7. Hoàn tác thay đổi
**git checkout -- <file>: Hủy các thay đổi trong file và đưa nó về trạng thái của commit cuối.
git reset <file>: Gỡ file khỏi "staging area" nhưng vẫn giữ nguyên các thay đổi.
git reset --soft <commit>: Hoàn tác các commit về một commit cụ thể và giữ lại các thay đổi trong "staging area".
git reset --hard <commit>: Hoàn tác các commit về một commit cụ thể và xóa các thay đổi hoàn toàn.
git revert <commit>: Tạo một commit mới đảo ngược thay đổi của commit chỉ định mà không làm thay đổi lịch sử commit.
**8. Làm việc với các thẻ (tags)
**git tag <tag-name>: Tạo một thẻ (tag) mới cho commit hiện tại.
git tag -a <tag-name> -m "message": Tạo một thẻ có chú thích.
git push <remote> <tag-name>: Đẩy một thẻ cụ thể lên kho lưu trữ từ xa.
git push --tags: Đẩy tất cả các thẻ lên kho lưu trữ từ xa.
**9. Làm việc với stash (lưu tạm thời thay đổi)
**git stash: Lưu các thay đổi hiện tại vào stash và làm sạch "working directory".
git stash list: Hiển thị danh sách các stash.
git stash apply: Áp dụng các thay đổi trong stash nhưng không xóa chúng khỏi stash.
git stash pop: Áp dụng các thay đổi từ stash và xóa stash đó.
git stash drop: Xóa stash hiện tại.
**10. Cấu hình Git
**git config --global user.name "Your Name": Thiết lập tên người dùng.
git config --global user.email "your.email@example.com": Thiết lập email người dùng.
git config --list: Hiển thị danh sách các cấu hình hiện tại của Git.
