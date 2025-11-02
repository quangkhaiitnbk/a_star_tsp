# 🚀 Mô phỏng sử dụng thuật toán A* (A-Star) để giải quyết Bài toán Người Du Lịch (TSP)

Đây là một dự án Web App sử dụng **Radzen Blazor** (.NET 8) để mô phỏng trực quan cách thuật toán A* tìm ra lời giải tối ưu cho Bài toán Người Du Lịch (TSP).

Điểm mấu chốt của mô phỏng này là trực quan hóa "suy nghĩ" của A* bằng cách hiển thị không chỉ đường đi hiện tại (g(n)), mà còn cả hàm heuristic (h(n)) được tính toán dựa trên **Cây khung tối thiểu (Minimum Spanning Tree - MST)** của các thành phố còn lại.

---

## ✨ Tính năng

* **Trực quan hóa A*:** Hiển thị từng bước của thuật toán khi nó khám phá không gian trạng thái O(N x 2^N).
* **Hiển thị Heuristic:** Vẽ Cây khung tối thiểu (MST) của các nút chưa được thăm (màu xanh lam) để biểu diễn chi phí ước lượng h(n).
* **Hiển thị đường đi:** Vẽ đường đi hiện tại đang được xét g(n) (màu đỏ) và đường đi tối ưu cuối cùng (màu xanh lá).
* **Bảng điều khiển:** Cho phép người dùng:
    * Tạo ngẫu nhiên số lượng thành phố (N).
    * Bắt đầu / Reset mô phỏng.

---

## 🖥️ Công nghệ sử dụng

* **.NET 8.0**
* **Blazor Server** (hoặc WASM, tùy bạn chọn `@rendermode`)
* **Radzen.Blazor:** Bộ thư viện UI component chính.
* **C#:** Ngôn ngữ lập trình.

---

## 🔧 Hướng dẫn Cài đặt và Chạy

### Yêu cầu

* [.NET 8.0 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
* Một trình soạn thảo code (như [Visual Studio 2022](https://visualstudio.microsoft.com/) hoặc [VS Code](https://code.visualstudio.com/)).

### Các bước cài đặt

1.  **Clone (Tải) Repository:**
    ```bash
    git clone [https://github.com/your-username/your-repo.git](https://github.com/your-username/your-repo.git)
    ```
    (Hoặc tải file ZIP và giải nén)

2.  **Điều hướng đến thư mục dự án:**
    ```bash
    cd your-repo-folder
    ```

3.  **Khôi phục các gói (Restore Packages):**
    Chạy lệnh này để tải về Radzen và các thư viện .NET cần thiết.
    ```bash
    dotnet restore
    ```

4.  **Chạy dự án:**
    ```bash
    dotnet run
    ```

5.  **Mở ứng dụng:**
    Mở trình duyệt và truy cập vào địa chỉ `http://localhost:xxxx` (địa chỉ này sẽ được hiển thị trong terminal của bạn, thường là `http://localhost:5123` hoặc `https://localhost:7123`).

---

## ⚙️ Cách sử dụng

1.  Chạy ứng dụng và truy cập vào trang mô phỏng.
2.  Sử dụng textbox để chọn số lượng thành phố.
    * **Cảnh báo:** Thuật toán này có độ phức tạp hàm mũ. Hãy giữ N < 10.
3.  Nhấn nút **"Tạo ngẫu nhiên"**.
4.  Nhấn nút **"Chạy A TSP"** để xem mô phỏng.

---

Đề tài tiểu luận của Trần Văn Quang Khải.
