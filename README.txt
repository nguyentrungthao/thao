// CÁC LỆNH THAO TÁC TRÊN FILE THƯ MỤC 
    mkdir (tên thư mục) // tạo thư mục mới 
    rmdir (tên thư mục) // xóa thư mục 

    type nul > (tên file).(đuôi) // tạo file mới
    del (tên file) // xóa file XÓA LÀ XÓA MẤT LUÔN CHỨ KO CÓ TRONG THÙNG RÁC 

CÁC LỆNH GIT 
    git -v or git --version // kiểm tra version của git 
    
    git config --global user.name "(tên tài khoản @.......)"
    git confgi --global user.email "(gmail đăng kí tài khoản)"
    git config --list

    git init // khởi tạo git ở local(1 thư mục bên trong máy tính)

THAO TÁC TRÊN Branch
    git branch (tên nhánh mới)  // chỉ tạo ra nhánh mới 
    git checkout -b (tên nhánh mới) // tạo mới và chuyển sang nhánh đó 

    git branch -d  (tên nhánh) // xóa nhánh ở local

    git push -d (tên nhánh) // xóa nhánh ở WEB

    # git push -u <remote> (tên nhánh mới) // đưa nhánh vừa tạo lên WEB 

    git checkout (tên nhánh) // di chuyển giữa các nhánh ( cần commit trước khi chuyển)

    git merge (nhánh cần merge vào) // LƯU Ý merge nhánh trong lệnh với nhánh hiện tại lưu trong nhánh hiện tại
                                        xử lý xung đột trong vscode sau đó add, commit lại
THAO TÁC GẮN tag
    git tag (tên tag) // đặt tên cho commit mà HEAD đang trỏ 
    git tag -a (tên tag) // Để thêm annotated tag, hãy chỉ định lựa chọn -a trong lệnh tag rồi thực hiện. Khi thực hiện thì trình soạn thảo sẽ khởi động nên hãy nhập bình luận sẽ thiết lập trong tag.
    git tag -am  "(comment)" (tên tag) // vừa đặt tag vừa đặt comment
    
    git tag -n // để xem tag và các cmt 

    git tag -d (tên tag) // xóa tag 
THAO TÁC log 
    git log // hiển thị thông tin các commit
        --oneline // chỉ hiển thị vị trí commit
        --decorate // hiển thị lịch sử thông tin tag 
