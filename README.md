


<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
    <title>Chào mừng đến với LUXURY GIRL 🎀</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>

#accessCodeDisplay {
    padding: 5px 7px;
    position: fixed;
    top: 20px;
    right: 30px;
    background: #DAA520; /* Màu vàng với độ trong suốt */
    padding: 10px;
    border-radius: 5px;
    display: none; /* Ẩn mặc định */
    z-index: 1000; /* Đảm bảo nổi bật */
    color: #000; /* Màu chữ */
    font-weight: bold; /* Đậm chữ */
        body { font-family: 'Poppins', sans-serif; background: linear-gradient(135deg, #ff7e5f, #feb47b); padding: 0; margin: 0; }
        .modal { position: fixed; top: 0; left: 0; width: 100%; height: 100%; display: flex; align-items: center; justify-content: center; z-index: 1001; }
        .modal-overlay { position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0, 0, 0, 0.5); z-index: 1000; }
        .modal-content { background-color: #fff; padding: 20px; border-radius: 10px; z-index: 1001; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); text-align: center; }
        .info-message { color: #ffffff; }
        .contact-button { color: #ff0000; font-weight: bold; }
        input[type="text"] {
        font-size: 16px; /* Thiết lập kích thước chữ mặc định lớn hơn để tránh phóng to trên iOS */
      }
    }
      #warning {
            font-size: 15px;
            color: #007413; /* Chữ trắng */
            text-align: center;
            background-color: #ff3d00; /* Màu nền cam */
            padding: 10px;
            border-radius: 5px;
            position: fixed;
            top: 25px; /* Căn cách lề trên */
            left: 20px; /* Căn cách lề trái */
            z-index: 9999; 
            display: none; /* Ẩn mặc định */
        }
        /* CSS cho spinner và thông báo */
.spinner-container {
    text-align: center;
    margin-top: 20px;
}

.spinner {
    border: 4px solid rgb(255, 255, 255);
    border-top: 4px solid rgb(255, 0, 0);
    border-radius: 50%;
    width: 50px;
    height: 50px;
    animation: spin 1s linear infinite;
}

@keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
}

.info-message {
    font-size: 14px;
    margin-top: 10px;
}
.contact-button {
    color: #ff6600;
    text-decoration: none;
    font-weight: 700; /* Đậm chữ */
}

.contact-button:hover {
    text-decoration: underline;
}
  .character {
            margin-bottom: 20px;
        }
        .status-btn {
            padding: 5px 10px;
            margin-left: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>
</script>
</body>
</html>







<div id="accessCodeModal" class="modal" style="display: flex;">
    <div class="modal-overlay"></div>
    <div class="modal-content">
<!-- Logo lớn -->
<div class="logo-container">
        <img src="https://i.ibb.co/q0cnWqD/photo-2024-10-15-22-09-13.jpg" alt="Logo" style="width: 90px; height: auto; margin-bottom: -30px;">
        <img src="https://i.ibb.co/7WW4LrB/photo-2024-08-19-18-39-28-2.jpg" alt="Logo" style="width: 90px; height: auto; margin-bottom: -30px;">
    </div>

        <h4>Nhập mã vùng khu vực do LUXURY GIRL BOOKING  cấp vì lí do bảo mật và lợi ích của khách hàng </h4>
        <div style="position: relative; width: 100%;">
            <input type="password" id="accessCodeInput" placeholder="Nhập mã tại đây" style="width: calc(100% - 40px); padding: 10px; margin-bottom: 10px;  border-radius: 10px; /* Viền vàng kim */">
           <span id="togglePassword" onclick="togglePasswordVisibility()" style="position: absolute; right: 10px; top: 50%; transform: translateY(-50%); cursor: pointer;">
                👁️
              
            </span>
        </div>
        <button onclick="checkAccessCode()" style=" box-shadow: 0 4px 10px rgba(0, 0, 0, 0.6); /* Hiệu ứng đổ bóng */ transition: background-color 0.3s, transform 0.3s, box-shadow 0.3s; background-color: #000000; /* Nền đen */ Viền vàng */ padding: 10px 20px;  border-radius: 5px;    
         cursor: pointer;">
            Xác nhận
        </button>

        <!-- Spinner khi đang kiểm tra mã -->
        <div class="spinner-container" id="spinnerContainer" style="display: none;">
            <div class="spinner"></div>
            <p class="spinner-text">Vui lòng đợi, hệ thống đang kiểm tra và tìm kiếm các bé gần nhất cho bạn...</p>
            <div class="progress-bar">
                <div class="progress"></div>
            </div>
        </div>

        <!-- Dấu tích xanh hiển thị khi mã được xác nhận -->
        <div class="success-message" id="successMessage" style="display: none; margin-top: 10px;">
            <span style="color: green; font-size: 24px;">&#10004;</span> Mã đã được xác nhận thành công!
        </div>

        <div class="info-message">
            <img src="https://i.ibb.co/R38vw3M/pngegg.png" alt="Custom Logo" style="height: 20px; width: 20px; vertical-align: middle; margin-right: 5px;">
  Bật vị trí để hệ thống có thể giúp bạn tìm kiếm và cung cấp chính xác vị trí các bé gần nhất nhé

        </div>
    </div>
</div>

<div id="accessCodeDisplay"></div>






<style>
    .modal { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.5); display: flex; align-items: center; justify-content: center; }
    .modal-content { background: #FFD700; border: 1px solid #DAA520; /* Viền vàng */ padding: 20px; border-radius: 8px; text-align: center; width: 300px; }
    .spinner-container { display: flex; flex-direction: column; align-items: center; justify-content: center; position: relative; width: 100%; }
    .spinner { border: 4px solid #00ff62; border-top: 4px solid #ff0000; border-radius: 50%; width: 40px; height: 40px; animation: spin 1s linear infinite; margin-bottom: 10px; }
    .spinner-text { color: #1100ff; /* Màu xanh lá đậm */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); font-size: 14px; font-weight: bold; }
    .progress-bar { width: 100%; border: 1px solid #DAA520; /* Viền vàng */
 background-color: #f3f3f3; height: 5px; margin-top: 10px; }
    .progress { width: 0%; height: 100%; background-color: #ff0000; animation: progressBar 2s ease-in-out infinite; }
    @keyframes spin { 100% { transform: rotate(360deg); } }
    @keyframes progressBar {
        0% { width: 0%; }
        50% { width: 50%; }
        100% { width: 100%; }
    }
    .success-message { font-weight: 600; color: green; border: 1px solid #DAA520; /* Viền vàng */}
    input[type="password"] { font-size: 16px; }
    button:disabled { background-color: gray; }
</style>

<script>
const correctAccessCode = "695422"; // Đặt mã truy cập hợp lệ

// Hàm kiểm tra mã truy cập
function checkAccessCode() {
    const inputCode = document.getElementById("accessCodeInput").value.toUpperCase();  // Chuyển tất cả chữ thành chữ hoa
    document.getElementById("spinnerContainer").style.display = "block";
    document.getElementById("accessCodeInput").disabled = true;
    document.querySelector("button").disabled = true;

    setTimeout(() => {
        if (inputCode === correctAccessCode) {
            localStorage.setItem('accessCodeEntered', 'true');
            localStorage.setItem('accessCode', inputCode);
            displayAccessCode(inputCode);

            // Hiển thị dấu tích xanh
            document.getElementById("successMessage").style.display = 'block';

            closeModal('accessCodeModal');
            requestLocation();

            alert("Đã kiểm tra thành công. Các bé gần nhất cho bạn đã được đề xuất. Mỗi mã vùng sẽ chỉ cập nhật chính xác cho lần đầu tiên ! ");
        } else {
            alert("Mã truy cập không chính xác. Vui lòng thử lại hoặc liên hệ hỗ trợ.");
        }

        document.getElementById("spinnerContainer").style.display = "none";
        document.getElementById("accessCodeInput").disabled = false;
        document.querySelector("button").disabled = false;
    }, 6000); // Giả lập thời gian kiểm tra mã (2 giây)
}

// Hàm hiển thị mã khu vực
function displayAccessCode(code) {
    const accessDisplay = document.getElementById('accessCodeDisplay');
    accessDisplay.innerText = `Mã vùng: ${code}`;
    accessDisplay.style.display = 'block';
}

// Hàm đóng modal
function closeModal(modalId) {
    document.getElementById(modalId).style.display = "none";
}

// Hàm khởi tạo trang
function initializePage() {
    const accessCodeEntered = localStorage.getItem('accessCodeEntered');
    if (accessCodeEntered !== 'true') {
        document.getElementById('accessCodeModal').style.display = 'flex';
    } else {
        const savedCode = localStorage.getItem('accessCode');
        displayAccessCode(savedCode);
    }
}

// Hàm yêu cầu bật vị trí
function requestLocation() {
    if (navigator.geolocation) {
        navigator.geolocation.getCurrentPosition(
            () => {
                alert("Vị trí đã được cấp thành công!");
            },
            (error) => {
                if (error.code === error.PERMISSION_DENIED) {
                    alert("Bạn đã từ chối quyền vị trí. Một số chức năng có thể không hoạt động.");
                }
            }
        );
    } else {
        alert("Trình duyệt của bạn không hỗ trợ Geolocation.");
    }
}

// Hàm bật/tắt hiển thị mật khẩu
function togglePasswordVisibility() {
    const passwordInput = document.getElementById("accessCodeInput");
    const toggleIcon = document.getElementById("togglePassword");

    if (passwordInput.type === "password") {
        passwordInput.type = "text";
        toggleIcon.innerText = "🙈"; // Thay đổi biểu tượng
    } else {
        passwordInput.type = "password";
        toggleIcon.innerText = "👁️";
    }
}

// Chạy khi trang được tải
window.onload = function() {
    initializePage();
};
</script>





    <style>
        #accessCodeDisplay {
            position: fixed;
top: 20px;
right: 20px;
background: rgba(0, 255, 0, 0.5); /* Màu xanh lá cây với độ trong suốt */
padding: 4px 8px;
border-radius: 5px;
display: none; /* Ẩn mặc định */
z-index: 1000; /* Đảm bảo nổi bật */
color: #000; /* Màu chữ */
border: 1px solid #000000; /* Viền màu đen */
box-shadow: 0 4px 10px rgba(0, 0, 0, 0.6); /* Hiệu ứng đổ bóng */
animation: blink 1s infinite; /* Hiệu ứng nhấp nháy */

}
body {
    background: linear-gradient(45deg, #ff7eb9, #ff65a3); /* Nền hồng gradient */
    color: #ffffff; /* Màu chữ tối để dễ đọc trên nền sáng */
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
}
        h2 {
        
            padding: 10px 15px;
          font-size: 20px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.6); /* Hiệu ứng đổ bóng */
    
    background: #ffffff; 
    color: #000000; 
    border-radius: 10px;

}

        .info-message {
            color: #000000; /* Màu chữ đen */

    }
    .contact-button {
        color: #ffe600; /* Màu chữ cho liên kết */
        font-weight: 700; /* Đậm chữ */
    }
    .info-message p {
    color: #FFD700; /* Chữ vàng */ /* Màu chữ cho thẻ <p> */
    }
        .modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 1001;
            display: none; /* Mặc định là không hiển thị */
        }
        .modal-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            z-index: 1000;
        }
        .modal-content {
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            z-index: 1001;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            text-align: center;
        }
        #locationError {
            display: none;
            text-align: center;
        }  

        .container {
            width: 80%;
            margin: 0 auto;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            color: #221414; /* Màu chữ tối */
        }
        .header {
            text-align: center;
            padding: 20px;
            position: relative;
            margin: 20px 0;
        }
        .header img {
            width: 90px;
            height: 130px;
            vertical-align: middle;
            margin-left: 10px;
            
        
          }

            .title {
    display: inline-block; /* Để logo và tiêu đề trên cùng dòng */
    font-size: 25px; /* Kích thước tiêu đề */
    font-weight: bold;
    color: #000000; /* Màu hồng đậm cho tiêu đề */
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5); /* Đổ bóng cho tiêu đề */
    vertical-align: middle; /* Căn chỉnh logo và tiêu đề theo chiều dọc */
}
        
h1 {
    display: inline-block;
    font-family: 'Poppins', sans-serif; /* Chọn font chữ */
    font-size: 15px; /* Kích thước chữ */
    font-weight: bold; /* Chữ đậm */
    text-align: center; /* Căn giữa tiêu đề */
    color: #000000; /* Chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
    background: linear-gradient(45deg, #FF6FB1, #FF7F7F); /* Nền hồng gradient */
    border-radius: 10px; /* Bo góc nền */
    padding: 10px; /* Khoảng cách giữa chữ và viền */
  
    text-transform: uppercase;
    letter-spacing: 3px;
    margin-bottom: 10px;

/* Keyframes cho hiệu ứng nhấp nháy */
@keyframes blink {
    0%, 100% {
        opacity: 1;
    }
    50% {
        opacity: 0.5;
    }
}
}
 @keyframes fadeIn {
            0% {
                opacity: 0;
                transform: translateY(-50px);
            }
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }
        .breadcrumb a {
            margin-top: -20px; /* Điều chỉnh giá trị này theo nhu cầu */

            color: #000000;
            text-decoration: none;
            font-family: 'Poppins', sans-serif;
        }
        .breadcrumb a {
            margin-top: -20px; /* Điều chỉnh giá trị này theo nhu cầu */

            color: #000000; /* Màu chữ breadcrumb */
            text-decoration: none;
        }
        .breadcrumb a:hover {
            text-decoration: underline;
        }
        .menu {
            padding: 20px; /* Khoảng cách giữa container và các nút */

            display: flex;
            justify-content: space-around;
            background: #000000;
            padding: 5px;
            border-radius: 5px;
            color: #000000; /* Chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
    transition: transform 0.3s ease, background-color 0.3s ease; /* Hiệu ứng chuyển động mượt mà */
          
        }
         .menu-item {
            padding: 10px; /* Khoảng cách giữa container và các nút */

            color: #ffffff;
            cursor: pointer;
            font-size: 13px;
            font-weight: 700;
            font-family: 'Poppins', sans-serif;
            border-radius: 5px;
        }

       
    
        .content {
            display: none;
        }
        .content.active {
            display: block;
        }
        .region-list {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
        }
        .region-btn {
            background: #000000;
            color: #ffffff; /* Chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
    display: flex;
    margin-top: 10px;
    cursor: pointer;
    padding: 5px 10px; /* Tùy chỉnh khoảng cách bên trong */
    transition: transform 0.3s ease, background-color 0.3s ease; /* Hiệu ứng chuyển động mượt mà */
    border-radius: 10px;
    font-weight: bold;
}
        .region-btn:hover {
            background-color: #ffffff;
    color: #000000;

    transform: scale(1.1); /* Phóng to nút 10% */
        }
        .detail-info {
            display: none; /* Ẩn thông tin chi tiết ban đầu */
            background-color: #000000; /* Màu nền nút cam đậm */
            color: #fafafa;
            border-radius: 5px;

            margin-top: 20px;
        }
        .button-container {
    margin-top: 10px;
}

.info-button {
    background-color: #ffffff;
    color: #000000; /* Chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
    padding: 5px 10px; /* Điều chỉnh padding để thay đổi kích thước nút */
    border-radius: 5px;
    margin: 1px;
    font-weight: 750;
    cursor: pointer;
    font-size: 12px; /* Điều chỉnh kích thước chữ */
    width: 110px; /* Điều chỉnh chiều rộng của nút */
    height: 40px; /* Điều chỉnh chiều cao của nút */
    transition: transform 0.3s ease, background-color 0.3s ease; /* Hiệu ứng chuyển động mượt mà */
  }
.info-button:hover {
    background-color: #ffffff; /* Màu nền khi hover */
    color: #000000; /* Chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
    transform: scale(1.05); /* Phóng to nhẹ khi hover */
}
.info-button i {
    margin-right: 3px;
    
}
        .submit-btn {
    padding: 5px 10px;
    background-color: #000000; /* Màu nền nút cam đậm */
    color: #000000; /* Chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
    border: none;
     margin-top: -50px;
    border-radius: 5px;
    border: 2px solid #000000; /* Viền cam nhạt */
    cursor: pointer;
    transition: background-color 0.3s, transform 0.3s ease;
    box-shadow: 0 4px 8px #000000;

}

.submit-btn:hover {
    background-color: #ff3d00; /* Màu nền khi hover */
    transform: scale(1.05); /* Phóng to nhẹ khi hover */
}

        .locked {
            color: rgb(5, 0, 0); /* Màu sắc cho nút khóa */
            font-weight: bold;
            display: none; /* Ẩn nút khóa ban đầu */
        }
        
        
    </style>
</head>
<body>
    <!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
    <title>Chào mừng đến với LUXURY GIRL 🎀</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <link  href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
   
    <style>
    
    /* Container tổng thể */
      #chat-container {
            position: fixed;
            bottom: 20px;
            right: 20px;
            width: 360px;
            height: 700px;
            border: 3px solid #0c5d9d;
            display: flex;
            flex-direction: column;
            background: linear-gradient(135deg, #2e8bc0, #0c5d9d);
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
            overflow: hidden;
            z-index: 1000;
            font-family: 'Arial', sans-serif;
        }

        #chat-header {
            background: #0c5d9d;
            color: #fff;
            padding: 15px;
            text-align: center;
            font-weight: bold;
            font-size: 18px;
            text-transform: uppercase;
        }
        .banner-container {
          margin-top: -30px;
            overflow: hidden;
            background-color: linear-gradient(135deg, #ff7e5f, #feb47b);
            height: 300px;
             width: auto;
            transition: background-color 0.3s ease, transform 0.3s ease; /* Hiệu ứng chuyển đổi */
        }

        .banner {
            display: flex;
            animation: scroll 30s linear infinite;
            overflow: hidden;
    width: 100%; /* Đặt chiều rộng cho banner */ 
        }

        .banner-image {
            height: 200px;
            width: auto;
            margin-right: 10px;
            border: 2px solid linear-gradient(135deg, #ff6ec7, #ff3ac1); /* Nền gradient hồng */
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.6); /* Hiệu ứng đổ bóng */
            flex-shrink: 0; /* Đảm bảo ảnh không co lại */
        }

        .banner-container {
    width: 100%; /* Chiều rộng toàn bộ */
    overflow: hidden; /* Ẩn ảnh ngoài container */
}
        .carousel {
    position: relative;
    width: 100%;
    overflow: hidden;
}
.banner-slide {
    display: flex; /* Để các ảnh chạy theo chiều ngang */
    transition: transform 0.5s ease; /* Thêm hiệu ứng chuyển động */
}

.banner-slide img {
    width: 100%; /* Đảm bảo mỗi ảnh chiếm toàn bộ chiều rộng của container */
    flex-shrink: 0; /* Không co lại khi có quá nhiều ảnh */
}
.carousel-image {
    position: absolute;
    width: 100%;
    opacity: 0;
    transition: opacity 1s ease-in-out;
}

.carousel-image.active {
    opacity: 1;
}

        @keyframes scroll {
            0% { transform: translateX(0); }
            100% { transform: translateX(-100%); }
        }

      
.center-notification {
    display: none; /* Ẩn ban đầu */
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    padding: 15px;
    border-radius: 12px;
    font-weight: bold;
    font-size: 13px; /* Kích thước chữ */
    background: linear-gradient(45deg, #ff7eb9, #ff65a3); /* Nền hồng gradient */
    color: #ffffff; /* Màu chữ */
    border: 2px solid #000000; /* Viền */
    width: 220px; /* Chiều rộng */
    text-align: center;
    box-shadow: 0 4px 8px #000000;
    z-index: 1000; /* Đảm bảo nó ở trên các thành phần khác */
}

@media (max-width: 600px) {
    .center-notification {
        width: 90%; /* Đặt chiều rộng là 90% trên điện thoại */
        max-width: 300px; /* Giới hạn chiều rộng tối đa */
        font-size: 12px; /* Kích thước chữ nhỏ hơn */
        padding: 10px; /* Giảm padding */
    }
}
/* Hiệu ứng cho thông báo xuất hiện */
.center-notification.show-enter {
    opacity: 0; /* Ban đầu ẩn */
}
.success-notification {
    display: flex;
    align-items: center;
    background: linear-gradient(135deg, #f7a7c5, #d14d83); /* Nền hồng gradient */

    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
    border: 2px solid #C0C0C0; /* Viền bạc */
    border-radius: 5px; /* Bo góc cho viền */
  
    margin-top: 20px;
    font-weight: bold;
    font-size: 13px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Thêm bóng nhẹ cho khối */
}

.success-notification img {
    width: 30px;
    height: 30px;
    margin-right: 10px;
}


.menu {
    
   
    justify-content: space-around; /* Căn đều khoảng cách */
    
 
      
        border-radius: 20px;
        color: #000000; /* Chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
    }

    .menu-item {
        cursor: pointer;
       
        text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */

    border-radius: 5px; /* Bo góc cho viền */
    }

    


    .package-container {
        display: flex;
        flex-wrap: wrap;
        gap: 20px;
        justify-content: center;
        padding: 10px; /* Giảm padding tổng thể */
}
.package {
    padding: 5px; /* Giảm padding cho mỗi gói */
    margin-bottom: 10px; /* Giảm khoảng cách giữa các gói */
}
    #pricing-table .package {
        background-color: #131313; /* Màu nền bạc */

        color: #ffffff; /* Chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
        border-radius: 10px;
        
        text-align: center;
      
        transition: transform 0.3s ease, background-color 0.3s ease; /* Hiệu ứng chuyển động mượt mà */
    }

    #pricing-table .package h2 {
        margin-bottom: 10px;

    }

    .promo-image {
        width: 80px;
        height: auto;
        margin-bottom: 15px;
        border-radius: 5px;
    }
    </style>
    </head>
  <body>
   
 
    
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Chào mừng bạn đến với LUXURY GIRL BOOKING 🎀</h1>
        </div>
    
        <div class="banner-container">
            <div class="banner">
                <img src="https://i.ibb.co/Tkxd6RF/taoanhdep-lam-net-anh-92190.jpg" alt="Banner Image" class="banner-image">
                <img src="https://i.ibb.co/64r0Rkm/photo-2024-11-07-00-37-49-5.jpg" alt="Banner Image" class="banner-image">
                <img src="https://i.ibb.co/LCX2dKV/photo-2024-10-29-23-43-13.jpg" alt="Banner Image" class="banner-image">
                <img src="https://i.ibb.co/H7YvZVJ/photo-2024-10-29-23-42-21-3.jpg" alt="Banner Image" class="banner-image">
                <img src="https://i.ibb.co/d6D4CMS/photo-2024-10-29-23-42-21.jpg" alt="Banner Image" class="banner-image">
                <img src="https://i.ibb.co/12vWhwY/Flag-of-South-Korea-svg.png" alt="Banner Image" class="banner-image">
                <img src="https://i.ibb.co/5K5Nv9b/photo-2024-11-07-00-39-08.jpg" alt="Banner Image" class="banner-image">
                <img src="https://i.ibb.co/P9qtdvL/photo-2024-11-07-00-37-49-4.jpg" alt="Banner Image" class="banner-image">
                <img src="https://i.ibb.co/64r0Rkm/photo-2024-11-07-00-37-49-5.jpg" alt="Banner Image" class="banner-image">
                <img src="https://i.ibb.co/njHS0h8/photo-2024-11-07-00-37-49-6.jpg" alt="Banner Image" class="banner-image">
            </div>
        </div>
<style>
  
</style>
</head>
<body>
 


    </style>

    <head>
        <script>
            function showInputBox(babyName, type) {
                const code = prompt("Vui lòng nhập mã giới thiệu:");
                if (validCodes[babyName] && validCodes[babyName][type] === code) {
                    switch (type) {
                        case 'telegram':
                            window.location.href = validCodes[babyName].link;
                            break;
                        case 'images':
                            alert("Mã chính xác, hiển thị hình ảnh của " + babyName);
                            break;
                        case 'booking':
                            alert("Mã chính xác, bạn có thể đặt lịch với " + babyName);
                            break;
                        default:
                            alert("Mã chính xác, nhưng không có hành động cho loại này!");
                    }
                } else {
                    alert("Mã không chính xác!");
                }
            }
        </script>
    </head>

                    <div class="statistics-widget">
                        <h4>Thống kê người dùng</h4>
                        <ul>
                            <li>Online  <strong id="online">&nbsp;427</strong></li>
                            <li>Đã dùng dịch vụ  <strong id="vipMembers">&nbsp;3821</strong></li>
                            <li>Tổng lượt truy cập  <strong id="visitCount">&nbsp;105083</strong></li>
                        </ul>
                        </div>
              

       <!-- Breadcrumb -->
<div class="breadcrumb">
  <a href="#">Trang Chủ</a> / <a href="#">Luxury Girl Booking</a> 
</div>


<div class="menu">
    <div class="menu-item" data-target="my-region-section">
        <i class="fas fa-map-marker-alt"></i> Gần đây
    </div>
    <div class="menu-item" onclick="togglePricingTable()">
        <i class="fas fa-dollar-sign"></i> Bảng giá
    </div>
    <!-- Nút Chat sẽ ở sau Bảng giá -->
    <div class="menu-item" onclick="toggleChat()">
        <i class="fas fa-comment-dots"></i> Chat Box
    </div>
    <div class="menu-item" data-target="image-section">
        <i class="fas fa-image"></i> Ảnh 18+
    </div>
    <div class="menu-item" onclick="toggleSubmenu()">
        <i class="fas fa-film"></i> Phim 18+
    </div>
    <div class="menu-item" data-target="support-section">
        <i class="fas fa-life-ring"></i> Hỗ trợ
    </div>
</div>

<!-- Bảng giá -->
<div id="pricing-table" style="display: none;  background-color: #C0C0C0 color: #FFD700; border-radius: 10px;">
    <h4 style="text-align: center;">✨ Bảng giá dịch vụ - Trải nghiệm sự đặc biệt ✨</h4>
    
    <div class="package-container">
      <!-- Gói Thường -->
      <div class="package">
        <h2>Gói Thường - 1540 TWD ⭐</h2>
        <p><strong>Thời gian:</strong> 90 phút</p>
<img src="https://i.ibb.co/vsDwM4G/ngua-thai-500x500-removebg-preview.png" alt="Gói VIP"style="height: 100px; width: auto;">            <p><strong>Thời gian:</strong> 90 phút</p>
        <p><strong>Dịch vụ:</strong> <p>Tắm chung thư giãn,massage nhẹ nhàng</p>
            <p> HJ và BJ chuyên nghiệp</p> 
            <p>Quan hệ 2 lần</p>
        <p><em>Gói Thường là sự lựa chọn lý tưởng cho lần đầu trải nghiệm</em></p>
    </div>

    <!-- Gói VIP -->
    <div class="package">
        <h2>Gói VIP - 3000 TWD ⭐</h2>
        <img src="https://i.ibb.co/yg6830F/keo-sam-hamer-tang-cuong-sinh-ly-1-vien-jpg-removebg-preview.png" alt="Gói VIP"style="height: 100px; width: auto;">
        <img src="https://i.ibb.co/98401Xz/Sin-Su-nuoc-chinh-hang-removebg-preview.png" alt="Gói VIP"style="height: 100px; width: auto;">
        <img src="https://i.ibb.co/Np0XnMR/Untitled-design-36-removebg-preview.png" alt="Gói VIP"style="height: 100px; width: auto;">
        <p><strong>Thời gian:</strong> 180 phút</p>
        <p><strong>Dịch vụ:</strong><p>Massage kết hợp,HJ và BJ với kỹ thuật nóng/lạnh</p> 
        <p>Quan hệ 3 lần</p> 
        <p>Đặc biệt,hỗ trợ công cụ quay lại khoảnh khắc ân ái 30 phút</p>
        <p><em>Gói VIP nâng cao trải nghiệm với những khoảnh khắc đặc biệt</em></p>
    </div>

    <!-- Gói Luxury -->
    <div class="package">
        <h2>Gói Luxury - 5800 TWD ⭐</h2>
        <img src="https://i.ibb.co/yg6830F/keo-sam-hamer-tang-cuong-sinh-ly-1-vien-jpg-removebg-preview.png" alt="Gói VIP"style="height: 100px; width: auto;">
        <img src="https://i.ibb.co/vsDwM4G/ngua-thai-500x500-removebg-preview.png" alt="Gói VIP"style="height: 100px; width: auto;">            
        <img src="https://i.ibb.co/98401Xz/Sin-Su-nuoc-chinh-hang-removebg-preview.png" alt="Gói Luxury"style="height: 100px; width: auto;">
        <img src="https://i.ibb.co/Np0XnMR/Untitled-design-36-removebg-preview.png" alt="Gói VIP"style="height: 100px; width: auto;">
        <p><strong>Thời gian:</strong> 16 giờ</p>
        <p><strong>Dịch vụ:</strong> <p>Tắm chung, sử dụng đồ chơi cao cấp</p>
        <p>Massage kỹ thuật Nuru với dầu đặc biệt</p> 
        <p>HJ và BJ,xuất vào miệng kèm chơi some</p> 
        <p>Quan hệ không giới hạn</p> 
        <p>Hỗ trợ công cụ quay lại khoảnh khắc ân ái toàn gói dịch vụ</p>
        <p><em>Trải nghiệm đỉnh cao của sự xa hoa và tinh tế với gói Luxury</em></p>
    </div>

    <!-- Gói VIP Tour -->
    <div class="package">
        <h2>Gói VIP Tour - 9000 TWD ⭐</h2>
        <img src="https://i.ibb.co/Np0XnMR/Untitled-design-36-removebg-preview.png" alt="Gói VIP Tour"style="height: 100px; width: auto;">
       <img src="https://i.ibb.co/vsDwM4G/ngua-thai-500x500-removebg-preview.png" alt="Gói VIP"style="height: 100px; width: auto;">
       <img src="https://i.ibb.co/98401Xz/Sin-Su-nuoc-chinh-hang-removebg-preview.png" alt="Gói Luxury"style="height: 100px; width: auto;">
       <img src="https://i.ibb.co/yg6830F/keo-sam-hamer-tang-cuong-sinh-ly-1-vien-jpg-removebg-preview.png" alt="Gói VIP"style="height: 100px; width: auto;">
       <p><strong>Thời gian:</strong> 3 ngày</p>
        <p><strong>Dịch vụ:</strong><p>Tận hưởng toàn diện bao gồm tất cả các gói dịch vụ trên</p> 
        <p>Với sự phục vụ tận tình chu đáo hơn cả người yêu</p> 
        <p>Cam kết mang lại sự hài lòng tuyệt đối và những kỷ niệm không thể quên</p> 
        <p>Đặc biệt quay lại khoảnh khắc làm tình đổi gió Public</p>
        <p><em>Gói VIP Tour dành cho những khách hàng tìm kiếm sự kết hợp giữa dịch vụ cao cấp và sự gắn bó lâu dài  </em></p>
    </div>

    <!-- Khuyến mãi đặc biệt -->
    <div class="package promo-package">
        <h2>Khuyến mãi đặc biệt</h2>
        <img src="https://i.ibb.co/5xnBnZT/Untitled-design-34.png" alt="Image 1" style="height: 200px; width: 150px;">
        <img src="https://i.ibb.co/PcBrZqH/Untitled-design-33.png" alt="Image 2" style="height: 200px; width: 150px;">
        <img src="https://i.ibb.co/JxkW3Dd/Untitled-design-32.png" alt="Image 3" style="height: 200px; width: 150px;">
        <img src="https://i.ibb.co/NTZ2yJS/photo-2024-11-08-17-50-13.jpg" alt="Image 4" style="height: 200px; width: 150px;">
        <img src="https://i.ibb.co/zJfm74N/reup-bao-vy-2k3-cuc-pham-gai-xinh-trang-treo-body-cuc-nuot-3230131-original.jpg" alt="Image 5" style="height: 200px; width: 150px;">
        <img src="https://i.ibb.co/tz34g6N/reup-bao-vy-2k3-cuc-pham-gai-xinh-trang-treo-body-cuc-nuot-3230130-original.jpg" alt="Image 6" style="height: 200px; width: 150px;">
        <p><strong>Chi tiết:</strong> Tất cả các gói có quà tặng kèm theo nếu khách hàng có nhu cầu. Khách hàng có thể chọn cosplay theo mã số trang phục</p>
        <p><em>Đặc biệt gói VIP trở lên sẽ được hỗ trợ công cụ quay phim ghi lại khoảnh khắc ân ái cùng các bé</em></p>
    </div>
</div>
</div>
</div>

    <script>
        function togglePricingTable() {
            const pricingTable = document.getElementById('pricing-table');
            pricingTable.style.display = pricingTable.style.display === 'none' ? 'block' : 'none';
        }
</script>

 


 <!-- 4 nút phim 18+ hiển thị sau khi nhấn vào Phim 18+ -->
 <div id="submenu-phim-18" class="submenu" style="display:none;">
    <button class="phim-btn" onclick="window.open('https://quatvn.fit/onlyfans-vietnam/', '_blank')">Phim 18+ Việt Nam</button>
    <button class="phim-btn" onclick="window.open('https://quatvn.fit/cn/', '_blank')">Phim 18+ Trung</button>
    <button class="phim-btn" onclick="window.open('https://quatvn.fit/us/', '_blank')">Phim 18+ U.S</button>
    <button class="phim-btn" onclick="window.open('https://quatvn.fit/kr/', '_blank')">Phim 18+ Hàn</button>
    <button class="phim-btn" onclick="window.open('https://quatvn.fit/jp/', '_blank')">Phim 18+ Nhật Bản (JAV)</button>
    <button class="phim-btn" onclick="window.open">Gái Việt Du học sinh (Member Vip 💎)</button>
    <button class="phim-btn" onclick="window.open('https://quatvn.fit/onlyfans-thailand/', '_blank')">Phim 18+ Khác</button>
</div>

</div>
<!-- Script để ẩn/hiện 4 nút phim 18+ -->
<script>
    function toggleSubmenu() {
        var submenu = document.getElementById("submenu-phim-18");
        if (submenu.style.display === "none" || submenu.style.display === "") {
            submenu.style.display = "flex";
        } else {
            submenu.style.display = "none";
        }
    }
</script>


<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
    <title>Chat Tự Động</title>
    <style>
        /* Container tổng thể */
        #chat-container {
              position: fixed;
              bottom: 20px;
              right: 20px;
              width: 360px;
              height: 700px;
              border: 3px solid #0c5d9d;
              display: flex;
              flex-direction: column;
              background: linear-gradient(135deg, #2e8bc0, #0c5d9d);
              border-radius: 15px;
              box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
              overflow: hidden;
              z-index: 1000;
              font-family: 'Arial', sans-serif;
          }
  
          #chat-header {
              background: #0c5d9d;
              color: #fff;
              padding: 15px;
              text-align: center;
              font-weight: bold;
              font-size: 18px;
              text-transform: uppercase;
          }
  
  
          #chat-box {
              flex: 1;
              padding: 15px;
              border-radius: 15px;
              overflow-y: auto;
              background-color: #f4f4f4;
              border: 3px solid #0c5d9d;
          }
          /* Message Styling */
          .chat-message {
              display: flex;
              align-items: center;
              margin-bottom: 15px;
              max-width: 100%;
          }
  
          .chat-message.self {
              justify-content: flex-end;
          }
          .time-stamp {
              font-size: 12px;
              color: #aaa;
              margin-top: 5px;
              text-align: right;
          }
          .avatar {
              padding: -10px;
              width: 45px;
              height: 45px;
              border-radius: 50%;
              margin: 0 10px;
              border: 2px solid #0099ff;
          }
  
          .message-bubble {
              background-color: #e1f5fe;
              padding: 10px;
              border-radius: 10px;
              box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
              position: relative;
              max-width: 250px;
             
          }
  
          /* User messages on the right */
          .self .message-bubble {
              background-color: #007bff;
              color: white;
              text-align: right;
          }
  
          /* Character messages on the left */
          .character-message {
            
              color: black;
             
              border-radius: 10px;
          }
  
          /* Username and Status */
          .user-name {
              font-weight: bold;
              font-size: 14px;
              color: #008cff;
              padding: -10px;
          }
  
          .message-status {
              font-size: 12px;
              color: #0084ff;
              position: absolute;
              bottom: -15px;
              right: 0;
          }
  
          #chat-input-container {
              display: flex;
              align-items: center;
              padding: 10px;
              background-color: #f4f4f4;
              border-top: 1px solid #ddd;
          }
  
          #chat-input {
              flex: 1;
              padding: 10px;
              border-radius: 20px;
              border: 1px solid #ccc;
              margin-right: 10px;
          }
  
          #send-btn {
              padding: 10px 20px;
              background: #007bff;
              color: white;
              border: none;
              border-radius: 20px;
              cursor: pointer;
              font-weight: bold;
              transition: 0.3s;
          }
  
          #send-btn:hover {
              background: #0056b3;
          }
  
          /* Thanh cuộn */
          #chat-box::-webkit-scrollbar {
              width: 8px;
          }
  
          #chat-box::-webkit-scrollbar-thumb {
              background: #007bff;
              border-radius: 5px;
          }
  
          #chat-box::-webkit-scrollbar-track {
              background: #f1f1f1;
          }
  
          button {
             
     
              color: rgb(255, 255, 255);
            
              border-radius: 5px;
              cursor: pointer;
              transition: background-color 0.3s ease;
              margin-left: 5px;
          }
  
          button:hover {
              background-color: #000000;
              color: rgb(255, 255, 255);
          }
          /* Tắt thu phóng cho input trên thiết bị di động */
  input[type="text"] {
      font-size: 16px; /* Ít nhất 16px để tránh tự động phóng to */
      touch-action: manipulation; /* Tắt thu phóng khi chạm */
  }
  
  
      </style>
  </head>
  <body>
  
    <div id="chat-container">
        <div id="chat-box"></div>
        <div class="chat-controls">
            <h2>Nhập tên và chọn avatar</h2>
            <input type="text" id="user-name" placeholder="Tên của bạn" />
            <input type="file" id="user-avatar" accept="image/*" onchange="loadAvatar(event)" />
            <textarea id="chat-input" placeholder="Nhập tin nhắn..."></textarea>
            <button onclick="sendTextMessage()">Gửi</button>
            
            <!-- Thêm input để gửi hình ảnh -->
            <input type="file" id="image-upload" accept="image/*" style="display: none;" onchange="sendImageMessage(event)">
            <button onclick="document.getElementById('image-upload').click()">📷</button>
            
            <!-- Thêm input để gửi video -->
            <input type="file" id="video-upload" accept="video/*" style="display: none;" onchange="sendVideoMessage(event)">
            <button onclick="document.getElementById('video-upload').click()">🎥</button>
    
            <button onclick="toggleChat()">Ẩn/Hiện Chat</button>
            <button onclick="toggleDarkMode()">Chế độ tối</button>
        </div>
    </div>
    <script>
      let userName = "";
let userAvatar = "";
let recentMessages = [];
const maxNoRepeat = 400;
const characters = [
        {
            name: "Ạhhh",
                avatar: "https://i.ibb.co/Wcfz0GB/343515938-244275581449331-9003722689350715063-n.jpg",
                messages: [
                "Tôi đánh giá cao e này",
"E nào lộ clip xinh thế nhỉ",
"Xinh như tiên nữ cũng bị đụ như người phàm cả",
"Nay rôm rả quá mai nghỉ làm hả các bác",
"https://i.ibb.co/Vv485HL/photo-20-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/6YsFD2S/photo-20-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/Y2H2hjc/photo-21-2024-10-23-11-22-02.jpg",
"Làm gì nữa bác làm cả tuần rồi cho nghỉ 1 ngày còn xả tres chứ troi",
"Mai tôi vẫn làm đây mấy og sướng quá",
"Làm j nhiều vậy bác ơi kiếm tiền nuôi bác sĩ à",
"Có hàng ngon không chia sẻ với ông",
"Hàng ai nấy dùng chia sẻ chi gặp ông cũng thế",
                ],
            },
            {
                name: "Cuongyencl",
                avatar: "https://i.ibb.co/wNmgWBF/465167896-122182676612159132-2007701611047559668-n.jpg",
                messages: [
                "Dit nhau suot k nghi ngoi ha may cha",
"Tầm này chỉ có địt chứ lm gì nữa ông",
"Hẹn ẻm giờ mới tới mấy ông ơi vào việc luôn chứ nóng lắm rồi",
"https://i.ibb.co/nwRxCpD/photo-18-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/K07JMK8/photo-18-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/34bdKZQ/photo-19-2024-10-23-11-22-02.jpg",
"Ngon lành vậy dáng đẹp đó",
"Da trắng vú to lồn chắc đẹp nốt",
                ],
            },
            {
                name: "Chi Duong",
                avatar: "https://i.ibb.co/CmcCtzt/433005087-1177556326740003-4441578403532921158-n.jpg",
                messages: [
                "Ông thử có ny thì biết nói mồm hay lam",
"Ngày nào cung đit xem có chán ko",
"https://i.ibb.co/h8tGGt9/photo-17-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/BwTPBQ1/photo-18-2024-10-23-11-51-38.jpg",
"Đào cứ để tôi mấy bác khéo lo",
"Tò mò thì lên lịch cho ah ah cho em biết nhé hấp dẫn lắm",
"Cứ thế này mấy ông vơ hết hàng ngon còn đâu",
                ],
            },
            {
                name: "Bao Gia",
                avatar: "https://i.ibb.co/zFXPLjM/65310101-541864686353769-4378968674397061120-n.jpg",
                messages: [
                "Mấy ông đi chơi về hết chưa nào",
"Đã cái con cặc thật",
"Mới tới đây chờ bé tới đụ thôi",
"Chắc phải lên lịch gấp thôi chứ chiu ko được rồi",
"https://i.ibb.co/Hrc6qgX/photo-21-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/mz6Rm3Y/photo-21-2024-10-23-11-52-30.jpg",
"Nay ny bắt đi xem phim k đi đâu đc mấy ông ạ 😕",
"Cái gì ăn nhiều chẳng ngán",
"Ông nào có ny mới hiểu đc nhỉ 😂",
                ],
            },
            {
                name: "Quynho Nho",
                avatar: "https://i.ibb.co/J22y6hn/444488207-872332088248034-5363803169786148493-n.jpg",
                messages: [
                "Suóng như vua bác nhỉ",
"Má quần rách này mà vừa chơi vừa xé thì quá là đã",
"Bú kiểu này chịu k nổi là phọt thôi",
"https://i.ibb.co/XtT4qfm/photo-16-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/dp5Nr6k/photo-17-2024-10-23-11-22-02.jpg",
"Con em nhiệt tình quá còn gì",
"Nhìn mấy bác sướng nhỉ tôi còn đang bận chưa đi được",
"Tôi thì đi rồi giờ ngủ giấc thôi",
                ],
            },
            {
                name: "Join Trần",
                avatar: "https://i.ibb.co/rMQkxC7/358100874-839190984300475-2168315640853368908-n.jpg",
                messages: [
                "Mới về gửi luôn feedback cho bé nó 😘 Tiền nào của nấy thôi mấy bác",
"Con cac dài vậy ông chắc tới lỗ rún e nó",
"Cu vậy đụ mấy nhỏ mới la làng",
"https://i.ibb.co/PQW9xhQ/photo-16-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/ZSQCLwx/photo-16-2024-10-23-11-52-15.jpg",
"Đi có tiếng về rồi ak ông",
"Làm xong 2 cái về thôi ông ạ cũng tiếng rưỡi",
"À gói 90 phút à cũng ngon phết",
"Um gói đó 2 nháy ok mà",
                ],
            },
            {
                name: "Vì Em",
                avatar: "https://i.ibb.co/4p5CGDZ/410274561-926577562228483-5651142562609102213-n.jpg",
                messages: [
                "Qua đêm luôn sáng về ngủ nghỉ cho khỏe",
"Có tiền muốn gì cũng đc 😁",
"Tưởng mình tôi đi chơi sớm",
"https://i.ibb.co/Pt99432/photo-15-2024-10-23-11-22-02.jpg",
"https://i.ibb.co/DrGSf3Y/photo-15-2024-10-23-11-52-30.jpg",
"Mấy cụ này nứng sớm thế nhỉ",
"Giờ đéo nào cũng có ông đang đụ",
"Cái lồn nhìn hồng hào thế húp thôi ông",
                ],
            },
            {
                name: "A Lek",
                avatar: "https://i.ibb.co/KrFYSCX/265197999-478573007028943-6441174678854474607-n.jpg",
                messages: [
                "Quan trọng gần ôg ko thôi 😂",
"Mai nghỉ k phải lo bác ạ",
"Nay được nghỉ sớm tranh thủ đặt phòng đợi ẻm tới",
"https://i.ibb.co/44ZDr8r/photo-14-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/Jskcg6f/photo-14-2024-10-23-11-52-30.jpg",
"Đã lên lịch rồi hả bác bọn tôi còn chưa về mà bác đã đc địt r",
"Bác đi gói nào mà đi sớm v",
                ],
            },
            {
                name: "Hùng lầy",
                avatar: "https://i.ibb.co/SRp7bXn/436150779-961127358947273-8444883863744652412-n.jpg",
                messages: [
                "Không sao anh ơi nhỏ vậy gặp em bú cho cũng lên à",
"Em bú cho ah đc k em ơi",
"Mẹ mới đi hôm qua nay admin mới thông báo cay vl",
"Anh nào chưa đc em bú thì thử đi nè",
"https://i.ibb.co/qFmGMc1/photo-12-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/rZmGvC3/photo-14-2024-10-23-11-51-38.jpg",
"Giờ này ông nào ông nấy chắc đi làm về hết roi nhỉ",
"Tầm này an uong r book đào đi chơi thôi",
                ],
            },
            {
                name: "Nợ 3 tỉ",
                avatar: "https://i.ibb.co/mRMZ0VR/455712717-1257948285545076-7415265304110521698-n.jpg",
                messages: [
                "Nuôt nhỉ thích mấy e mình dây thế nà",
"Ông nói điều ai cũng biết cả",
"Càng nuột thì càng bị địt nhiều thôi ong",
"https://i.ibb.co/wN1BqR3/photo-12-2024-10-23-11-22-02.jpg",
"https://i.ibb.co/5986MWf/photo-12-2024-10-23-11-52-15.jpg",
"Tôi thì thích mấy bé vừa vừa ít ai rớ tới 😂",
"Tranh thủ đi chịch lấy feedback về lấy lại 30% thôi",
"Đi chung chứ địt chung là ko đc đâu nha",
                ],
            },
            {
                name: "T Anh",
                avatar: "https://i.ibb.co/0XFC6pq/avatar-trang-4.jpg",
                messages: [
                "Địt chung nâng tình cảm anh em lên chứ bác",
"Tôi đi chiến trc nhé ae. Lên lịch rồi 😁",
"https://i.ibb.co/7z8qP2r/photo-11-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/fHH0mMJ/photo-11-2024-10-23-11-52-30.jpg",
"Mấy ông ít nói mới hay đi nhất đấy còn mấy ông rãnh chat chắc tháng đi đc 1 lần",
"Thì rãnh mới ở đây xàm xàm chứ có tiền đã đi rồi kk",
"Sn bao nhiêu nhìn bé vậy ông",
                ],
            },
            {
                name: "Lee San ",
                avatar: "https://i.ibb.co/T13PkKz/463780581-527298090157663-601024373815710168-n.jpg",
                messages: [
                "Sao chịch yếu ớt thế sao e nó sướng đc",
"Tôi ở nhà hóng video mấy ông thôi",
"Tôi đang địt mà mấy ông nt hỏi lắm the nhỉ",
"https://i.ibb.co/Gxt99Mr/photo-10-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/m6m7z4Y/photo-11-2024-10-23-11-22-02.jpg",
"K đi chịch thì ở nhà coi phim sex thôi",
"Xem phim đâu có sướng bác",
                ],
            },
            {
               
                name: "15195 Tuan",
                avatar: "https://i.ibb.co/0XFC6pq/avatar-trang-4.jpg",
                messages: [
                "Ae ay có săn đc em nào chưa",
"Mấy bữa nay đi chịch nhiều quá giờ hơi đau lưng",
"Canh muộn muộn đi rồi về ngủ chứ đi sớm về lại mò vào nhóm xem lại thèm",
"Thèm thì đi tiếp thôi",
"https://i.ibb.co/7JcNcDN/photo-7-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/r3yhQ8Z/photo-8-2024-10-23-11-52-15.jpg",
"Sợ k có tiền chứ sợ gì thèm",
"Nay tranh thủ thế bác",
"Trải nghiệm xem ưu đãi mới thế nào ấy mà",
                ],
            },
            {
                name: "Cu li",
                avatar: "https://i.ibb.co/0XFC6pq/avatar-trang-4.jpg",
                messages: [
                "Tôi còn đang chọn đào mấy bác đã đi về cả rồi",
"Kết bé kia mà nay ẻm bận k đi đc chán quá",
"Og sợ thiếu gái hay gi mà k kiếm bé khác",
"https://i.ibb.co/pJcSpDp/photo-7-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/Q8D8dCG/photo-7-2024-10-23-11-52-15.jpg",
"Giờ này mấy ông chắc ấp ủ bên mấy e đào cả rồi",
"K địt trc ngkh địt mất xót lắm",
"Xinh vỗn cả lài",
                ],
            },
            {
                name: "Vu Manh Kien",
                avatar: "https://i.ibb.co/JztdF9T/453721020-122098035392441413-2102100990856763741-n.jpg",
                messages: [
                "Đù má ngon vậy kiểu này phải đi sớm",
"Ai có info e này k xin với",
"Tôi có tôi cũng giấu chứ cho làm gì kk",
"Tên đẹp người cũng đẹp xuất sắc quá",
"https://i.ibb.co/Lhwhq9W/photo-6-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/ZLjP2X8/photo-6-2024-10-23-11-52-30.jpg",
"Xinh thế này k chịch phí cả cuộc đời",
"Làm nốt ngày mai rồi đi chưa muộn đâu 😂",
"Giờ này book về 1 bé còn gì bằng nữa",
                ],
            },
            {
                name: "Linh a",
                avatar: "https://i.ibb.co/7vwCwD2/465146753-1634609844076820-5036638866219117952-n.jpg",
                messages: [
                "Lại ko được ngủ yên rồi",
"Giờ này book về 1 bé còn gì bằng nữa",
"https://i.ibb.co/8d7HBkN/photo-80-2024-10-23-11-52-15.jpg",
"Hôm nay k book mai chắc k còn đào để book luon quá",
"Đặt lịch trc cho chắc khéo mai hết thật 😂",
"https://i.ibb.co/9sKrvrr/photo-5-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/jyL34kM/photo-5-2024-10-23-11-52-30.jpg",
"Lại lên lịch đi chịch thôi chứ sao",
"Chốt kèo với con e rồi tối tiển thôi",
"Hẹn mà toàn ông đi trước đi sau ko à",
                ],
            },
            {
                name: "KK",
                avatar: "https://i.ibb.co/DWpmDXw/287503735-2569447153190823-6330025235431122917-n.jpg",
                messages: [
                "Thằng dưới ăn còn thằng trên nuôi hả bác",
"Toàn thằng nhỏ đc ăn thằng lớn phải cày cắm đầu",
"Ông nào rãnh k vào giao lưu với tôi vài game",
"Đồng môn đây rồi",
"https://i.ibb.co/yPfqdyy/photo-5-2024-09-28-20-48-55.jpg",
"https://i.ibb.co/8YftK71/photo-5-2024-10-23-11-22-02.jpg",
"Rủ nhau chơi game hôm nào rãnh kéo nhau đi địt chung cho vui",
"Bác nói hợp lý quá nhỉ",
"Ở bên này chơi game toàn quen mấy e  ở Vn đéo làm ăn gì đc",
"Chúng nó toàn thánh bào mà bảo 😂",
                ],
            },
            {
                name: "Nguyen Son",
                avatar: "https://i.ibb.co/PcGmbtB/464608602-3938705709699464-8297307432761372977-n.jpg",
                messages: [
                "Để tiền đi địt gái  sướng hơn",
"Nay có bé nào mới k nhỉ",
"https://i.ibb.co/fH5wrK3/photo-81-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/w76YbQ0/photo-82-2024-10-23-11-51-38.jpg",
"Ông đi đc hết gái ở đây chưa mà đòi mới",
"Tôi mới đi đc 3 em còn chưa dám than",
"Con hàng ngon ko mấy ôg",
"https://i.ibb.co/G353KZZ/photo-3-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/0Vz9NX4/photo-4-2024-10-23-11-52-30.jpg",
"Vú này chắc vú thật bóp nhìn đã thế mà",
"Để tôi bóp thử mới biết thật hay giả",
                ],
            },
            {
                name: "nam dangg",
                avatar: "https://i.ibb.co/BBwd7hN/464034358-122095125710589062-5303331676268128522-n.jpg",
                messages: [
                "E này dáng đẹp nhỉ thích mấy e kiểu vậy",
"Tại bác k biết thôi chứ trong này nhiều k thiếu",
"Này gu tôi này",
"Tôi cũng thích nhỏ nhắn như này",
"https://i.ibb.co/r7MTbCV/photo-2-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/3B3B02w/photo-3-2024-10-23-11-22-02.jpg",
"Húp đê ae review tôi xem",
"Tôi thích bé này ae để tôi đi trước nhe",
                ],
            },
            {
                name: "Van Trọng Nguyễn",
                avatar: "https://i.ibb.co/0XFC6pq/avatar-trang-4.jpg",
                messages: [
                "Có người làm hướng dẫn cho roi ngại gì nua kk",
"Đỡ tốn 1 khúc rồi mấy bác 😂😂",
"https://i.ibb.co/pZ4JDPs/photo-1-2024-10-23-11-22-02.jpg",
"https://i.ibb.co/C7LH58G/photo-1-2024-10-23-11-52-15.jpg",
"Ông nào cũng bú đc mấy bé vú ngon thế nhỉ",
"Hay mối quen giấu ăn mình vậy",
                ],
            },
            {

            name: "Nguyễn Thanh",
                avatar: "https://i.ibb.co/QXDVCMr/462452894-844678954503160-8051059654342602004-n.jpg",
                messages: [
                "Đi địt luôn cho máu chả phải hóng của ông nào",
"Vậy mới là chất chơi làm luôn cho nóng",
"Nhìn đã quá mà vẫn phải kiềm chế",
"https://i.ibb.co/GTJKm14/photo-1-2024-09-28-20-48-55.jpg",
"https://i.ibb.co/G03zXPt/photo-22-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/HhygWWL/photo-22-2024-10-23-11-52-30.jpg",
"Có con cu để sung sướng sao phải kiềm chế hả bác",
"Thủ tục sẵn sàng chờ nàng tới nắc",
                ],
            },
            {


                name: "mùa thu lá bay tình yêu tôi",
                avatar: "https://i.ibb.co/ysn0YTm/anh-avatar-trang-nam-11.jpg",
                messages: [
                "Vậy mới là chất chơi làm luôn cho nóng",
        "Nhìn đã quá mà vẫn phải kiềm chế",
        "https://i.ibb.co/s1kWhJ9/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321646.jpg",
"https://i.ibb.co/xYWkm7Q/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321645.jpg",
"https://i.ibb.co/GcQtzym/review-of-cu17cm-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-3263673-original.jpg",

        "Đi địt luôn cho máu chả phải hóng của ông nào",
        "Thủ tục sẵn sàng chờ nàng tới nắc",
        "Giờ này vẫn đc đi địt là sướng nhất rồi",

                ],
            },
            {
                name: "Cho 1 nắc",
                avatar: "https://i.ibb.co/wsVWCV4/Gallery-of-ready-made-prints-from-the-My-Stamp-Ready-online-stamp-maker.jpg",
                messages: [
                "Trông ngọt nước nhỉ,phải chi đc ké miếng thì",
        "Kéo nhau đi hết đi cho đỡ ồn ào",
        "https://i.ibb.co/s1kWhJ9/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321646.jpg",
"https://i.ibb.co/xYWkm7Q/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321645.jpg",
"https://i.ibb.co/GcQtzym/review-of-cu17cm-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-3263673-original.jpg",

        "Mấy ông đi đéo đi suốt ngày hỏi hỏi",
        "Nhìn dáng mấy e này ngon hết chỗ chê",
        "Hàng tuyển phải khác hàng dạt rồi",

                ],
            },
            {
                name: "Con cặc",
                avatar: "https://i.ibb.co/55zr4Jm/kisspng-computer-icons-information-image-logo-symbol-association-michel-voix-l39association-des-ar-5.jpg",
                messages: [
                "Giờ này k onl thì chắc chỉ có đi ngủ hoặc đi địt thôi",
        "Đoán hay quá bác 😂",
        "https://i.ibb.co/s1kWhJ9/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321646.jpg",
"https://i.ibb.co/xYWkm7Q/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321645.jpg",
"https://i.ibb.co/GcQtzym/review-of-cu17cm-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-3263673-original.jpg",

       
        "Các dân chơi hôm nay thế nào rồi",
        "Qua mới book 1 em giờ rệu rã hết cả người",

                ],
            },
            {
                name: "Phong Nguyen",
                avatar: "https://i.ibb.co/0cz42bL/kisspng-helpline-telephone-hotline-customer-service-swimmi-friendly-5b2b1d41705161-09937128152955219.png",
                messages: [
                "Phải nói là mấy ẻm khẩu dâm đụ hứng vcc",
        "Sợ gặp mấy em nằm như cục đá đéo có cảm hứng gì đúng k bác",
        "https://i.ibb.co/s1kWhJ9/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321646.jpg",
"https://i.ibb.co/xYWkm7Q/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321645.jpg",
"https://i.ibb.co/GcQtzym/review-of-cu17cm-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-3263673-original.jpg",

        "Là sao vậy mấy ông ai chỉ tôi với",
        "Chữ to thế k biết đọc à bác",
        "Hiểu rồi quả này mấy bố lại đi nhiều hơn cho xem",

                ],
            },
            {
                name: "Dũng",
                avatar: "",
                messages: [
                "Phải nói là mấy ẻm khẩu dâm đụ hứng vcc",
        "Sợ gặp mấy em nằm như cục đá đéo có cảm hứng gì đúng k bác",
        "https://i.ibb.co/s1kWhJ9/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321646.jpg",
"https://i.ibb.co/xYWkm7Q/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321645.jpg",
"https://i.ibb.co/GcQtzym/review-of-cu17cm-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-3263673-original.jpg",

        "Để tôi đi về cho mấy ông làm theo 😂",
        "Mới đi tối qua giờ được tính ko nhỉ hay tính từ sau thông báo ta",
        "Bác đui cũng thấy mờ mờ kể từ này hôm nay chứ",

                ],
            },
            {
                name: "Tâm",
                avatar: "https://i.ibb.co/0XFC6pq/avatar-trang-4.jpg",
                messages: [
                "Đấy lâu lâu phải thế này cho ae khô máu có tinh thần",
        "Chào các bác nha bua gio hóng giờ mới có thể vô chat 😝",
        "https://i.ibb.co/s1kWhJ9/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321646.jpg",
"https://i.ibb.co/xYWkm7Q/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321645.jpg",
"https://i.ibb.co/GcQtzym/review-of-cu17cm-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-3263673-original.jpg",
        "Chúc mừng tham gia hội đồng râm",
        "Haha thank bác nhiều nhé",
        "À thì ra mấy nay ông nt hỏi tôi suốt đó à",

                ],
            },
            {
            name: "Vũ anh",
            avatar: "https://i.ibb.co/0XFC6pq/avatar-trang-4.jpg",
            messages: [
              "https://i.ibb.co/R24khgC/photo-2024-11-08-17-50-12.jpg",
              "https://i.ibb.co/FsmffJ1/review-of-duy-anh-for-hot-girl-thu-thuy-lan-dau-tien-co-mat-gaito-3166745-original.jpg",
              
        "Nay buồn quá nhỉ nay có gì vui k anh em",
        "Tới phòng a đc ko a lười đi ks quá",
        "Lên tận  giường luôn hả e khoái rồi à nha",
            ],
          },
          {
            name: "Bebe",
            avatar:
              "https://i.ibb.co/x3jTBpZ/109351219-2969029043216925-2295414862108758346-n.jpg",
            messages: [
              "Có cụ nào từng gọi 2 em 1 lúc đi chơi chưa",
              "Hôm nào setup kèo 2 thằng gọi 2 con đi chơi đổi ca nhỉ. hay gọi vào 1 phòng chơi chung",
              "Đụ má chơi kiểu này hay này",
              "Đi chơi cho biết chứ cũng mất tiền chơi gái phải thử cái mới các cụ à",
              "Nào mấy bố đi quay video cho thẩm cái nhé",
              "Tranh thủ đụ đi mai phải đi làm r",
              "Nhìn cũng thèm lắm mà mới đi hôm qua k lẽ đi nữa",
              "Tôi nhập cuộc trước đây mấy cụ hưởng thụ sau nhé đang hứng 😝",
            ],
          },
          {
            name: "1 TIẾNG MỚI RA",
            avatar:
              "https://i.ibb.co/tKwGxxV/98450420-915018178938574-441821537687830528-n.jpg",
            messages: [
              "Mấy ông né né em ghệ của tôi ra nhé k tôi xót lắm",
              "Em nào đụ hết",
              "https://i.ibb.co/WW6G5zc/photo-25-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/ZX9kF2P/photo-26-2024-10-23-11-51-38.jpg",
              "Vkl bác thật nói thế mất tinh cam qua",
              "Đụ bừa đi quan tâm gì ghệ này ghệ nọ 😆",
              "https://i.ibb.co/RQ8gD5Y/review-of-jollibee-for-hot-girl-thu-thuy-lan-dau-tien-co-mat-gaito-3222277-original.jpg",
              "Chơi gái nhiều quá giờ phải ăn cơm vs trứng này",
              "Còn trứng để ăn là hp đấy",
              ],
            },
            {
                name: "Duy Quang",
                avatar: "https://i.ibb.co/hKQCWK5/453380460-2383644118498649-8155721825479697582-n.jpg",
                messages: [
                "Nét đấy các ôg mặtt dễ thương phết",
        "Quan trọng là ai húp trc thôi b 😌",
        "https://i.ibb.co/8cbkkB6/photo-23-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/KmjBP7Y/photo-23-2024-10-23-11-52-15.jpg",
    
          "Trc hay sau cũng địt dc cả mà lo chi hầy",
        "Anh e thấy khó quá thì cứ để tôi tôi xơi tuốt",
        "Ngon qá ae ơi đụ em này ko tiếc tiền đâu",
                ],
            },
            {
                name: "DUMA",
                avatar: "https://i.ibb.co/0XFC6pq/avatar-trang-4.jpg",
                messages: [
                "Tức dái lắm đúng k b kk",
        "Chả thế còn j đang thèm lại còn",
        "https://i.ibb.co/7nxq2Fn/review-of-nguyen-for-hot-girl-thu-thuy-lan-dau-tien-co-mat-gaito-3265174-original.jpg",
       
        "Không ngon đâu để lại tôi xử lý giúp cho",
        "Bữa giờ bận quá nay có tgian là húp luôn",
        "Chủ yếu là để khoe thẻ có đúng k 😆",
                ],
            },
            {
                name: "Anh Tuấn",
                avatar: "https://i.ibb.co/kmY3L7V/352382077-3179841912161446-5627824095159964225-n.jpg",
                messages: [
        "Để vào việc xem thế nào nóng ruột quá bác ạ",
        "https://i.ibb.co/RCzDHJT/photo-23-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/VSDdwBn/photo-24-2024-10-23-11-51-38.jpg",
        "Ko chén ngay thì lại hết phần đấy chứ đùa 😂",
        "Bú chưa anh e 😜",
      
        "Lại nứng cặc nữa roi đó",
        "Thèm địt thôi chứ có thèm bú đâu b",
                ],
            },
            {
                name: "Đi tìm chân ái",
                avatar: "https://i.ibb.co/3hKwxbX/358139466-2512362152257507-3962504851293990919-n.jpg",
                messages: [
                "Làm mấy phát về nghỉ ngơi là khỏe",
        "Tôi thik mấy em nhiệt tình thế này đây chơi mới cảm giác",
        "Thế thì phải bo thêm cho mấy em thôi",
        "https://i.ibb.co/3vtg5wN/caption-6.jpg",
        "Đơn giản cứ sướng là được 😆",
        "https://i.ibb.co/PrByBhq/hot-girl-linh-dan-nang-tho-xinh-dep-dang-chuan-nhu-model-3209378-original.png",
        "Ae cầm 100k qua mình x10 x20 x30 tk rồi đi hát có cả lan can luôn nha 🤣",
        "Oke xếp cho mình 1 vé đi b kk",
        "https://i.ibb.co/pr2xt5J/photo-82-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/8DqD10f/photo-83-2024-10-23-11-22-02.jpg",
        "X10 hay mất x10 thì chưa biết dc gian nan lắm",
        "B mất tôi cho tiền xe b về k phải lo",
        "https://i.ibb.co/Qdp0KPg/caption-7.jpg",
        "Lam giau khong kho nhi,ma giau cho cac bac ay 😂",
        "Lợi nhuận cao thế cũng hơi lo nha hhh",
                ],
            },
            {
                name: "Khang Anh",
                avatar: "https://i.ibb.co/6r0CzTX/452448952-500748632604966-6811140838307509192-n.jpg",
                messages: [
                "Làm đâu đấy bác cho xin chân nào",
        "Xa quá xa quá kk",
        "https://i.ibb.co/PcBrZqH/Untitled-design-33.png",
        "Mấy em gái đâu thấy cảnh này,địt dc mấy cái nói này nói kia 😂",
        "Có chak mấy cái ko chứ nge đồn b địt như cái máy đấy",
        "https://i.ibb.co/tcht2V3/photo-25-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/D9znnts/photo-25-2024-10-23-11-52-15.jpg",
        "Lời đồn thường không có thật 😑😑",
        "https://i.ibb.co/gTryjyf/caption-8.jpg",
        "Thỏa mãn rồi đó các bác thấy sao",
        "Dm nhất ôg rồi địt vậy mới chân thật dc",
                ],
            },
            {
                name: "chịch chịch cái nà",
                avatar: "https://i.ibb.co/JnkFG9b/449981297-2757549737738746-7208353843692482286-n.jpg",
                messages: [
                    "Mấy em này biết chơi hết rồi đấy",
                    "Đúng mốt chơi gái như thế này",
                    "https://i.ibb.co/7znT3v5/han-baby-nang-dam-nu-dang-dep-mong-to-mat-xinh-3271485-original.jpg",
                    "Tôi ngủ trc đây ae đi chơi vui vẻ nhé",
        "Nay có đi làm ko các bác êy",
        "https://i.ibb.co/dpnmNpg/caption-9.jpg",
        "Có thất nghiệp đâu mà k cày bố",
        "Com nc chi chưa onl sớm ri mấy cha",
                ],
            },
            {
                name: "Phanada",
                avatar: "https://i.ibb.co/0XFC6pq/avatar-trang-4.jpg",
                messages: [
                    "Bỏ qua mấy em nó đi, chơi cái khác thôi",
                    "Chơi gái không phải chuyện dễ",
                    "Lồn ngon nhỉ vừa khít con cu luôn 😁",
        "Nhấp gì yếu ớt thế chưa ăn cơm hả ôg 😂",
        "https://i.ibb.co/WW6G5zc/photo-25-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/ZX9kF2P/photo-26-2024-10-23-11-51-38.jpg",
        "Chắc đag cảm nhận hơi ấm kk",
        "https://i.ibb.co/nLWHX8g/caption.jpg",
        "Coi full móc vkl thật 😁",
        "Vú nó bơm nhưng mà đẹp thật nhỉ",
        "Coi mấy em show hàng còn nứng hơn mấy bố đụ ấy 🤣",
        "https://i.ibb.co/4f9ZXQ2/photo-83-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/wg4gy1q/photo-84-2024-10-23-11-51-38.jpg",
        "Làm ko lo làm xem sex suốt ngày rồi than nghèo 😌😌😌😌",
        "Tôi làm chắc b biết nhỉ 😒😒",

            ],
        },
        {
          name: "NANA",
          avatar: "https://i.ibb.co/PrByBhq/hot-girl-linh-dan-nang-tho-xinh-dep-dang-chuan-nhu-model-3209378-original.png",
          messages: [
            "Mình đi thôi anh yêu",
            "E nằm phơi mình đợi anh nè",
            "Em có thể phục vụ anh bất cứ lúc nào",
            "Ai muốn em chăm sóc và phục vụ mình nhỉ?",
            "Thư giãn bên em a sẽ không phải thất vọng đâu",
            "Hãy để em làm tất cả cho em rất vui khi được phục vụ",
            "E luôn mong chờ những phút giây bên anh kk",
            "chỉ cần anh gọi là em có mặt",
                ],
            },
            {
                name: "Duyquangdang",
                avatar: "https://i.ibb.co/VQfDRxN/439999497-2323079844555077-1613079290709043637-n.jpg",
                messages: [
                    "Mấy em này đúng chuẩn chơi hết rồi",
                    "Đừng so sánh nữa chơi thôi",
                    "https://i.ibb.co/HBthCXD/photo-27-2024-10-23-11-22-02.jpg",
"https://i.ibb.co/8jsvgp8/photo-27-2024-10-23-11-52-15.jpg",
                    "Nhịn lâu lắm rồi hay sao khổ thế",
                    "https://i.ibb.co/gMKQs1Q/review-of-kath-nguyen-for-reup-hottu-anh-hot-model-cuc-ky-loi-cuon-va-khong-the-choi-tu-2741787-orig.jpg",
        "Vã lắm r hả b còn k lo địt đi",
        "Mông ni doggy đúng cmn bài nhỉ",
        "Đụ lút cán luôn ấy bác hầy 🤣",
                ],
            },
            {
                name: "Hoàng phong",
                avatar: "https://i.ibb.co/4gShwVt/363310097-1450155849152375-8396000734777126-n.jpg",
                messages: [
                    "Chơi là phải đúng đỉnh, mấy em này thích hợp",
                    "Tôi thích mấy em này hơn",
                    "https://i.ibb.co/yXpRfRY/photo-28-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/W0rJLvD/photo-28-2024-10-23-11-52-30.jpg",
        "Ước dc nhảy vào phang e này luôn",
        "https://i.ibb.co/Lt9hmH7/review-of-kath-nguyen-for-reup-hottu-anh-hot-model-cuc-ky-loi-cuon-va-khong-the-choi-tu-2741788-orig.jpg",

        "Xoắn quần lên mà đi chờ đợi j 🥱🥱",
        "Làm 2 bìu bò này ngủ đến sáng",
                ],
            },
            {
                name: "Hồng Đăng",
                avatar: "https://i.ibb.co/HB587n8/44936471-527542047763163-5996408823554768896-n.jpg",
                messages: [
                    "Đây là lựa chọn tốt nhất rồi",
                    "Chơi thử chắc sẽ ok",
                    "https://i.ibb.co/BPsM4j7/review-of-long-dep-trai-1990-for-reup-hottu-anh-hot-model-cuc-ky-loi-cuon-va-khong-the-choi-tu-28614.jpg",
                    "Học than theo mấy bác mới có tiền dc kk",
                    "https://i.ibb.co/BtQVmfs/photo-30-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/cYjPG1x/photo-30-2024-10-23-11-52-15.jpg",
        "Giờ này chỉ có đi nhậu về nằm hưởng thụ đúng bài",
        "Để dành qua tháng đi hoài mì tôm k có mà ăn 😆😆",
        "Ăn vậy lúc nào cũng than khổ vl",
                ],
            },
            {
                name: "anh muốn địt em",
                avatar: "https://i.ibb.co/DKSYyrc/48360783-729235107453398-7758860129620983808-n.jpg",
                messages: [
                "Book đi đụ phát là biết thật hay bơm chứ đoán già đoán non làm gì",
                "https://i.ibb.co/yNr8tZj/photo-79-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/N6NKT3c/photo-79-2024-10-23-11-52-15.jpg",
        "Ngày mô cũng nhậu thế ni hỏng hết",
        "Đụ dc 5 phút vác dái đi về",
        "https://i.ibb.co/JFYSB1c/review-of-haotroc-for-re-up-angela-phuong-trinh-nu-hoang-cosplay-massage-fuck-3009171-original.jpg",
        "Ăn sau lại còn mời vkl",
        "Ông nào lên lịch tối nay chưa thế",
        "https://i.ibb.co/2sXtdq0/photo-77-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/GVDRKfG/photo-78-2024-10-23-11-52-15.jpg",
        "Tôi còn đang cắm đầu làm bác đã đi chơi gái rồi à",
        "Bác ko đi à sao còn ở đây thế",
        "https://i.ibb.co/KrGY6n3/review-of-h-saoke-for-re-up-angela-phuong-trinh-nu-hoang-cosplay-massage-fuck-3159348-original.jpg",
        "Đụ lút cán luôn phê lòi nhỉ 🤣",
        ],
        },

        {
          name: "QUỲNH ANH",
          avatar: "https://i.ibb.co/hRWg01V/review-of-dau-si-la-ma-for-reup-tieu-vy-xinh-dam-ngoan-3258118-original.jpg",
          messages: [
            "Em sẽ khiến a cảm thấy thoải mái luôn",
            "Đến với em nhen",
            "Chắc chắn anh sẽ thích thời gian bên e cho mà xem",
            "Em luôn ở đây để phục vụ anh",
        
            "A có muốn dành thời gian thư giãn với e k nè?",
            "Em hứa sẽ làm anh hài lòng,chỉ cần anh thử thui",
                ],
            },
            {
                name: "Tuấn An Đỗ",
                avatar: "https://i.ibb.co/PYd3Gf3/65965425-484218999000145-7695834040057724928-n.jpg",
                messages: [
                    "Chắc phải chọn lựa kĩ mới chơi được",
                    "https://i.ibb.co/5WwmC9V/photo-30-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/SfFcNJ9/photo-31-2024-10-23-11-52-15.jpg",
                    "Mấy ôg nhanh thế vừa vào đã húp mất rồi",
        "Nắc cho vậy mak bảo k sướng nữa thì...",
        "https://i.ibb.co/k1mfzzG/review-of-vu-nguyen-anh-quan-for-reup-tieu-vy-xinh-dam-ngoan-2711519-original.jpg",
        "Nhìn nứng cac thế nhỉ tôi mà đc như bác chắc tôi đụ cho bê lồn chạy",
        "Chịu khó đi nhiều nhiều là biết e nào ngon thôi",
        "Ngon nên mới phải thử trc chứ",
                ],
            },
            {
                name: "Tuấn",
                avatar: "https://i.ibb.co/0XFC6pq/avatar-trang-4.jpg",
                messages: [
                    "Chơi thử rồi cảm giác chơi cũng ok",
                    "Chơi kiểu này vẫn chưa đủ",
                    "https://i.ibb.co/tZLZbCN/review-of-vung-trom-for-reup-tieu-vy-xinh-dam-ngoan-2831885-original.jpg",
                    "Lò mò đi đụ sớm vậy tới lắm r à 🤣",
        "Cu bác vừa dài vừa to bảo sao e ấy k rên cho được",
        "https://i.ibb.co/dQ5D2GM/photo-31-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/bJ7btzF/photo-32-2024-10-23-11-51-38.jpg",
        "Ai đầu tư tiền để tôi đi check cho",
        "Tranh thủ book lẹ đi k hết đào đấy bạn nhé kk",
                ],
            },
            {
                name: "NgọcSơn",
                avatar: "https://i.ibb.co/2KJcQ2F/71565859-2330950190358150-5687197424787914752-n.jpg",
                messages: [
        "anh em ngồi tâm sự",
        "Mỗi lần tụ tập ăn uống đều có thêm đồ ăn ngon",
        "https://i.ibb.co/yXxbpVc/photo-32-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/syw8M2x/photo-33-2024-10-23-11-52-15.jpg",
        "Có thêm bạn hiền, chỗ ngồi nhậu nhẹt càng vui",
        "Cảm giác không thoải mái khi ở cùng bạn có người yêu kk",
        "Nhìn người đẹp cảm giác như diễn viên nước ngoài",
        "https://i.ibb.co/C987LV2/photo-84-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/cYF3WLM/photo-85-2024-10-23-11-22-02.jpg",
        "Nét quá bác ơi mặt này chắc xinh lắm",
                ],
            },
            {
                name: "ĐôngQuang",
                avatar: "https://i.ibb.co/2vwZvf5/82220736-1079023835772513-6462290643480739840-n.jpg",
                messages: [
                "Đang lên lịch tối nay book 1 e xinh tươi vú hồng",
        "Lồn hồng mới khó chứ vú hồng bt mà",
        "https://i.ibb.co/DRd6F1P/photo-34-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/8zV2FzQ/photo-35-2024-10-23-11-52-15.jpg",
        "Mấy bác đụ nhiệt tình quá khách sạn họ thích lắm",
        "Nhậu đê các ông say vào mới hứng chơi gái đuoc",
        "https://i.ibb.co/d5XkbGc/review-of-dai-gia-phuong-nam-for-reup-tieu-vy-xinh-dam-ngoan-2629009-original.jpg",
        "Tôi thích kiểu chơi này hơn",
                ],
            },
            {
                name: "BảoLong",
                avatar: "https://i.ibb.co/8cJZ16g/82334469-1079023799105850-3117550875644526592-n.jpg",
                messages: [
                    "Chơi kiểu này chắc cũng ổn",
                    "Mấy em này có vẻ vừa phải",
                    "Chơi kiểu này chưa thử bao giờ",
                    "https://i.ibb.co/xDfnDcm/review-of-tran-le-cong-for-reup-tieu-vy-xinh-dam-ngoan-2856816-original.jpg",
        "Chơi trong bồn tắm, cảm giác tung tóe nước thú vị",
        "Đổi không khí ra ban công cũng có cảm giác lạ",
        "Có người nhắn tin bảo đặt hẹn, hơi nổi da gà",
        "https://i.ibb.co/x1ccJNy/photo-75-2024-10-23-11-22-02.jpg",
"https://i.ibb.co/Xt1rVM5/photo-75-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/ZcQKwg2/photo-76-2024-10-23-11-51-38.jpg",
        "Đồng ý tham gia cho vui",
        ],
        },

        {
          name: "TRÂM ANH",
          avatar: "https://i.ibb.co/YpfzdNb/reup-tieu-vy-xinh-dam-ngoan-2716893-original.jpg",
          messages: [
            "Em luôn sẵn sàng cho các anh",
            "Có anh nào muốn lên đỉnh cùng em không",
            "E nhớ các anh lắm rồi đấy baby à",
            "Các anh đang làm gì đó súng đx lên đạn chưa",
            "E đang đợi các a gọi đây",
            "Em sẽ khiến các anh lên mây haha",
            "Các anh cần em không nè",
            "E sẽ làm các anh thư giãn nhức nách lun",
            ],
            },
            {
                name: "Duy An",
                avatar: "https://i.ibb.co/xSnjJCs/365675002-964747994746987-1739486736806920427-n.jpg",
                messages: [
                    "Chơi cũng ok đấy",
                    "Các em nó chơi có vẻ khéo léo",
                    "Đang ngồi hóng mấy ông khoe gái đít bự ăn cơm cho dễ nuốt 😁",
        "Cũng chỉ đụ thôi chứ gì mà màu mè hhh",
        "https://i.ibb.co/Sy32Kv0/review-of-ga-dau-troc-for-reup-tieu-vy-xinh-dam-ngoan-2717315-original.jpg",
        "Giờ này dc húp hàu rồi sướng thế",
        "https://i.ibb.co/qCfxVyM/review-of-sa-de-for-reup-eimi-fukada-body-goi-cam-service-chu-dao-3081515-original.jpg",
        "đc nắc em này sướng gì bằng nữa",
        "Hàng ngon thế vú đẹp vl thật",
                ],
            },
            {
                name: "Anhhuy5341",
                avatar: "https://i.ibb.co/0XFC6pq/avatar-trang-4.jpg",
                messages: [
                "Bú luôn chúc bác vui vẻ nhé",
        "Tôi giờ vẫn chưa lựa đuọc e nào thấy e nào cũng ngon",
        "https://i.ibb.co/bgh2gck/photo-35-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/m4PYmxp/photo-36-2024-10-23-11-52-15.jpg",
        "Mấy ông có thể đi suốt ngày suốt đêm k hết tiền ak",
        "Chỉ sợ k có sức mà đi thôi chứ tháng 5 6 lần vẫn dư sức",
        "https://i.ibb.co/SV88J2T/review-of-dau-si-la-ma-for-reup-tieu-vy-xinh-dam-ngoan-3258117-original.jpg",
        "Có ông nào đi chơi nhiều quá giờ hết ngổng nổi ko",
        "Vkl bác dùng thuốc tăng cường sinh lý đi",
                ],
            },

            {
                name: "quan88",
                avatar: "https://i.ibb.co/HKLtJsy/91995446-885014241938968-7102376830853709824-n.jpg",
                messages: [
                    "Bên này ok không các bác",
                    "Ai đã book mấy bé bên này chưa",
                    "https://i.ibb.co/rMh7PKc/review-of-jo-pang-for-reup-eimi-fukada-body-goi-cam-service-chu-dao-3152556-original.jpg",
                    "Tôi đang tìm phòng thoải mái ai biết chỗ nào không",
                    "Chỗ mình có phòng đẹp lắm các bác có muốn thử không",
                    "https://i.ibb.co/PYGCZ0C/photo-36-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/HDrJ7wf/photo-37-2024-10-23-11-52-30.jpg",
                    "Liên hệ ngay nếu cần phòng gấp mình sẽ giúp",
                ],
            },
            {
                name: "anhhuytran",
                avatar: "https://i.ibb.co/dtz5KBD/94361100-2489325074652782-6359101537343504384-n.jpg",
                messages: [
                    "Có em nào rảnh không bên này còn phòng không các bác",
                    "Tôi đang muốn book phòng ai biết chỗ nào tốt không",
                    "https://i.ibb.co/d40CFMJ/review-of-jo-pang-for-reup-eimi-fukada-body-goi-cam-service-chu-dao-3152555-original.jpg",
                    "Ai đã trải nghiệm bên này rồi cho tôi xin lời khuyên",
                    "Bên này có mấy bé xinh ai thử chưa",
                    "https://i.ibb.co/GR2ZWSM/photo-38-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/R0wDbK2/photo-38-2024-10-23-11-52-15.jpg",
                    "Chỗ này đúng chuẩn bác nào cần đặt thì báo mình",
                ],
            },
            {
                name: "quốc hùng54",
                avatar: "https://i.ibb.co/tKwGxxV/98450420-915018178938574-441821537687830528-n.jpg",
                messages: [
                "Có cụ nào từng gọi 2 em 1 lúc đi chơi chưa",
        "Hôm nào setup kèo 2 thằng gọi 2 con đi chơi đổi ca nhỉ. hay gọi vào 1 phòng chơi chung",
        "Đụ má chơi kiểu này hay này",
        "https://i.ibb.co/pQdcnZJ/rau-sach-be-bong-face-xinh-hang-ngon-nguc-dep-mong-to-3082477-original.jpg",
"https://i.ibb.co/YPHBH9p/review-of-phich-thu-for-reup-thuy-cherry-nhan-sac-diem-le-than-hinh-sexy-me-hoac-2938628-original.jpg",
"https://i.ibb.co/mNm6fH7/review-of-long-dep-trai-1990-for-reup-thuy-cherry-nhan-sac-diem-le-than-hinh-sexy-me-hoac-2914807-or.jpg",
        "Đi chơi cho biết chứ cũng mất tiền chơi gái phải thử cái mới các cụ à",
        "Nào mấy bố đi quay video cho thẩm cái nhé",
        "Tranh thủ đụ đi mai phải đi làm r",
        "https://i.ibb.co/WGs8pVb/photo-85-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/j8vfvgZ/photo-86-2024-10-23-11-22-02.jpg",
        "Nhìn cũng thèm lắm mà mới đi hôm qua k lẽ đi nữa",
        "Tôi nhập cuộc trước đây mấy cụ hưởng thụ sau nhé đang hứng 😝",
                ],
            },
            {
                name: "Tấn lực",
                avatar: "https://i.ibb.co/x3jTBpZ/109351219-2969029043216925-2295414862108758346-n.jpg",
                messages: [
                "Mấy ông né né em ghệ của tôi ra nhé k tôi xót lắm",
        "Em nào đụ hết",
        "Vkl bác thật nói thế mất tinh cam qua",
"https://i.ibb.co/5vJdDBW/review-of-thanh-bui-tien-for-reup-tieu-linh-2k4-xinh-tuoi-dang-nuot-na-vu-dep-bym-non-to-3203402-ori.jpg",
        "Đụ bừa đi quan tâm gì ghệ này ghệ nọ 😆",
        "Chơi gái nhiều quá giờ phải ăn cơm vs trứng này",
        "Còn trứng để ăn là hp đấy",
                ],
            },
            {
                name: "huyklkk",
                avatar: "https://i.ibb.co/0XFC6pq/avatar-trang-4.jpg",
                messages: [
                "Phải nói là mấy ẻm khẩu dâm đụ hứng vcc",
        "Sợ gặp mấy em nằm như cục đá đéo có cảm hứng gì đúng k bác",
        "https://i.ibb.co/s1kWhJ9/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321646.jpg",
"https://i.ibb.co/xYWkm7Q/review-of-lan-tan-chon-buoi-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-321645.jpg",
"https://i.ibb.co/GcQtzym/review-of-cu17cm-for-be-hani-2k-cute-xinh-xan-vu-dep-body-nong-bong-lan-dau-di-lam-3263673-original.jpg",
        "Tôi là tôi khoái mấy bé rên rên kiểu vậy đó",
        "Tui thì chỉ cần là con gái là được 😂",
        "https://i.ibb.co/XxG4yxw/photo-86-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/QKQCMwh/photo-87-2024-10-23-11-52-15.jpg",
        "Nay mấy bác rãnh lắm hay sao book mấy e xinh xinh kín lịch hết vậy nhỉ",

                ],
            },
            {
    
     
          name: "HÀ MY",
          avatar: "https://i.ibb.co/5vJdDBW/review-of-thanh-bui-tien-for-reup-tieu-linh-2k4-xinh-tuoi-dang-nuot-na-vu-dep-bym-non-to-3203402-ori.jpg",
          messages: [
            "Book em đi nào",
            "Tới đi a ơi",
            "Thèm lắm rồi à nha",
            "Lên lịch cho em đi",
            "Em sẵn sàng làm tất cả để anh cảm thấy thoải mái",
            "Chắc chắn sẽ không làm anh thất vọng đâu",
            "Em đang ở đây để làm anh vui vẻ",
            "Em sẽ làm anh bất ngờ đó",
            "Để em phục vụ anh nhé",
                    ],
            },
            {
    
                name: "YUMI",
                avatar: "https://i.ibb.co/SsZ2pgF/g1ixJ3Kw.jpg",
                messages: [
                    "Anh muốn thư giãn bên em k",
                    "Em ở đây đợi các a nãy h đó",
                    "Thử đi anh",
                    "Lên lịch cho em đi,em cho anh tới bến",
                    "Em có thể giúp anh thư giãn,anh nứng là đc",
                    "Anh cần gì cứ yêu cầu",
                    "Em rất vui khi được phục vụ anh hihi",
                    "Ai muốn thư giãn cùng em nào",
                    "Em sẽ làm anh bất ngờ với dịch vụ của e",

                ],
            },
            {
      
            
                name: "THIÊN AN",
                avatar: "https://i.ibb.co/px4G7Z6/review-of-hai-for-reup-huyen-my-nhe-nhang-tinh-cam-yeu-chieu-nhu-nguoi-yeu-3247539-original.jpg",
                messages: [
                    "Em luôn sẵn sàng",
                    "E sẽ khiến a cảm thấy thoải mái nhất có thể",
                    "Ai muốn tận hưởng khoảnh khắc tuyệt vời cùng e?",
                    "E đang rảnh chỉ cần a gọi là em có mặt",

                    "E sẵn sàng phục vụ a với tất cả sự nhiệt tình",
                    "Hãy để e mút chim cho a ha",
                    "K cần lo lắng e sẽ làm a cảm thấy như ở nhà",
                    "A sẽ không hối hận khi chọn em đâu",
                ],
            },
             {
     
                name: "anh yêu July",
                avatar: "https://i.ibb.co/H4hr8C5/119231544-2831857350465762-6729963575003338264-n.jpg",
                messages: [
                "Đúng nhờ địt che hết cả lồn hhh",
        "Gặp tôi phải 3 cái chơi mới thấm dc",
        "https://i.ibb.co/vDrbVH0/review-of-dam-dam-cong-tu-for-reup-huyen-my-nhe-nhang-tinh-cam-yeu-chieu-nhu-nguoi-yeu-3272192-origi.jpg",
        "3 cái mỗi cái 5 phút ai chả chơi được 🤣🤣",
        "Làm gì tệ thế dc ít cũng 10p chứ kk",
        "https://i.ibb.co/5RZs9QW/review-of-dark-for-reup-huyen-my-nhe-nhang-tinh-cam-yeu-chieu-nhu-nguoi-yeu-3220611-original.jpg",
"https://i.ibb.co/KFFGQjT/review-of-cuong-hoang-dang-vinh-for-reup-huyen-my-nhe-nhang-tinh-cam-yeu-chieu-nhu-nguoi-yeu-3228232.jpg",
        "Các bác ăn uống hết chưa ?",
        "Cả ngày bận bịu giờ mới vào đc",
        "Book e mô đi chơi chưa các ôg",
                ]
            },
            {
                name: "nguyenbao",
                avatar: "https://i.ibb.co/rmK5PCc/352379758-1477320172672258-7072304429330889757-n.jpg",
                messages: [
                "Say vào đừng book gái nữa nha b 😁",
        "Uống dc mấy lắm mà say",
        "https://i.ibb.co/WBF1cmv/review-of-map-for-rau-sach-be-thao-nhi-non-to-de-thuong-mon-mon-tuoi-moi-lon-3242824-original.jpg",
"https://i.ibb.co/Bzb4vWd/review-of-map-for-rau-sach-be-thao-nhi-non-to-de-thuong-mon-mon-tuoi-moi-lon-3242822-original.jpg",
        "Mấy e nhân viên đag chờ sẵn đấy đừng để mấy e thất vọng",
        "Ns thế ngta đánh giá tôi thì lm s",
        "https://i.ibb.co/mS9Th4H/photo-66-2024-10-23-11-22-02.jpg",
"https://i.ibb.co/drpJkD2/photo-66-2024-10-23-11-52-15.jpg",
        "K địt thì thôi đã địt phải ngon mới vừa lòng",
        "Cho mình hài lòng chút với nào 😁",
        ]
            },
            {
                name: "Luongnhat",
                avatar: "https://i.ibb.co/VpRxPtz/84800118-700943840309899-8909380622955315200-n.jpg",
                messages: [
                "Đc 3-4 lần ko được sờ cái là xong hả b",
                "https://i.ibb.co/xjPDHDw/photo-40-2024-10-23-11-52-15.jpg",
        "Nhanh lắm chắc định địt hết luôn giờ chắc còn đi",
"https://i.ibb.co/S0jkb2t/review-of-lang-tu-for-rau-sach-be-lucie-hotteen-mau-anh-non-to-xinh-xan-3152565-original.jpg",
        "Trc ngày nào đi là đi hết k cơm nước chi đg hả b",
        "Lần trước đi bị bỏ quên lâu wé kẹo ăn mà chứ",
                ]
            },
            {
                name: "tronghieu",
                avatar: "https://i.ibb.co/dmVbPqC/146645217-1840675756092820-270253680374749053-n.jpg",
                messages: [
                "Diễn tả nghe nứng cặc thật đấy mấy ông ơi",
        "Anh e giờ này lâm trận hết cả rồi nhỉ 😆",
        "https://i.ibb.co/60SbS0p/review-of-the-la-het-for-reup-minh-anh-mat-xinh-da-trang-body-boc-lua-3228179-original.jpg",
"https://i.ibb.co/hc6ZZ9n/review-of-hao-for-reup-minh-anh-mat-xinh-da-trang-body-boc-lua-3235021-original.jpg",
        "Còn tôi vs bác đây thây kk",
        "Mai đi làm rồi chơi bời chi giờ ni",
        "Sáng đi lm là chuyện của buổi sáng lo gì 🤣🤣",
                ]
            },
            {
                name: "minhluan",
                avatar: "https://i.ibb.co/HDzXCcq/215367314-2897466637173500-1538921034047321931-n.jpg",
                messages: [
                "Tiền bạc đâu mà ăn vs uống kk",
        "Hít lắm thế mà vẫn nuốt dc cơ à",
        "https://i.ibb.co/QcbFmCm/photo-41-2024-10-23-11-51-38.jpg",
        "Chắc đồ ngon quá đó b 😆",
        "https://i.ibb.co/dBFppLm/review-of-bungbu12-for-reup-hot-be-thao-vy-baby-nong-bong-xinh-dep-diu-dang-3235218-original.jpg",
        "Nay húp dc em nào chưa vậy ae",
        "Nướng khoai sớm thế b",
                ]
            },
            {
                name: "phucdung97",
                avatar: "https://i.ibb.co/K5HF4VJ/428230343-2268725836657145-7035186052846929012-n.jpg",
                messages: [
                    "Nhiều ae chắc mê body e này lắm nhỉ em này bú quá chuyên nghiệp luôn",
                    "Đừng gạ gẫm nữa mấy em call mà mấy e cứ móc bướm cho xem sao chịu nổi",
                    "https://i.ibb.co/sFgN3ff/photo-40-2024-10-23-11-52-30.jpg",
                    "Mà bé này ở teku đấy ae nào gần thì nhanh test thử",
                    "https://i.ibb.co/7Kqsbz8/20200403-205530-largejpg.jpg",
                    "Nhăn tin đặt bảo đặt bé an nhiên nhé bé này nc nôi ae khỏi phải chê đi",
                ]
            },
            {
                name: "Lehoangbaonam",
                avatar: "https://i.ibb.co/q0tfwvZ/226491311-3103868136598014-9122348726549110625-n.jpg",
                messages: [
                "Nhìn đã vãi loz vú múp thế",
                    "Kiếm bé nào đi chat sex mấy ông ơi",
                    "https://i.ibb.co/Gv4XS42/photo-43-2024-10-23-11-22-02.jpg",
                    "Book mak đụ chat làm j cho nứng",
                    "https://i.ibb.co/FhpMt3S/dh-naissance-friendly.jpg",
                    "K phải móc đâu để a đến a đụ cho sướng em ơi",
                    ]
            },
            {
                name: "SELINA",
                avatar: "https://i.ibb.co/sRvKkpc/reup-hot-be-thao-vy-baby-nong-bong-xinh-dep-diu-dang-3203116-original.jpg",
                messages: [
                "A muốn lên lịch với e chưa",
        "E đang rảnh để book a đây",
        "Book e ngay để có cuộc hẹn tuyệt vời nha",
        "A đã lên lịch chưa hay muốn e phục vụ ngay",
        "E luôn sẵn sàng cho a khi cần",
                ]
            },
            {
                name: "tùng dương",
                avatar: "https://i.ibb.co/TbB9FZP/241280385-2011849205642140-8610168309376988925-n.jpg",
                messages: [
                "Dễ thương thế k book thì phí",
                "https://i.ibb.co/091Nsdr/photo-43-2024-10-23-11-52-15.jpg",
                    "E nó đang nứng quá đấy bác",
                    "https://i.ibb.co/CbgMhX5/glue-hotel.jpg",
                    "Em móc thế hỏng hết hàng họ em ơi",
                    "Mấy bé hôm nay vắng khách nên nứng quá à",
                ]
            },
            {
                name: "điệp",
                avatar: "https://i.ibb.co/54R9nZv/242726891-2058879164272477-4153675998582393962-n.jpg",
                messages: [
                "Mấy em hôm nay k ông nào chơi chắc lắm nc lắm đây",
                "https://i.ibb.co/HgRhj8D/photo-43-2024-10-23-11-52-30.jpg",
                    "Các em đợi a tối a đến a chiều mấy em cho bớt nứng",
                    "Chơi ngày đầu tuần này là mấy e nó nhiều nc hơn",
                    "Ông bạn cái j cũng biết nhỉ",
                    "https://i.ibb.co/m64NW1j/caption.jpg",
                    "Nói gì thì nói chứ cái nc lồn này ae nào muốn bú k",
                    "E này nc dâm thủy thì đúng nhiều luôn vừa động vào cái đã chảy nc rồi",
                    "Cũng k ăn thua ngày làm ngày nghỉ chỉ đủ ăn thôi",
                    "Làm mệt về có các em nó tâm sự cũng đỡ mệt các bác ạ",
                ]
            },
            {
                name: "thachbinh",
                avatar: "https://i.ibb.co/NCk7t5P/272220237-2110103892483337-2781115009146832995-n.jpg",
                messages: [
                "Giờ này ae đang nướng khoai hết r nhỉ",
                "https://i.ibb.co/fYY996j/photo-44-2024-10-23-11-51-38.jpg",
        "Chắc k đợi bác nhắc đâu 😆",
        "Tôi tăng 1 chưa xong mà ae đã tăng 2 tăng 3 rồi ak",
        "Thôi xong .. combo nay xong ngồi bắn cá thì hết bài",
        "Mất ngủ. Đến sáng mới tỉnh. Vì. Hít quá. Sâu",
        "Cuối cùng cũng dc húp 😁",
        "https://i.ibb.co/x5b94BF/glue-hotel-1.jpg",
        "Giờ này ae đang nướng khoai hết r nhỉ",
        "Dáng người đẹp hàng cũng ngon nữa😆",
        "E này mà bú cu thì đúng sướng lắm đây",
        "Mấy em gầy gầy này bú cặc giỏi mà đụ cũng sướng nữa",
        "https://i.ibb.co/7VHyZZS/photo-64-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/y4sDqq2/photo-65-2024-10-23-11-52-15.jpg",
        "Em này mới đi hôm nọ thấy cũng ok nên rivew cho ae ấy mà",
        "Call mấy e nó phải call ngay k nhiều ae call liên tục",
    
                ]
            },
                {

                name: "JULY",
                avatar: "https://i.ibb.co/QMkTVpc/395590541-1042794623814007-9064456112968543170-n.jpg",
                messages: [
                    "A muốn thư giãn cùng em ko nek",
                    "Em đang rảnh để phục vụ a đây",
                    "Anh cần gì em có cái đó :V",
                    "Em sẵn sàng phục vụ a",
                    "Để em làm anh hài lòng nhen",
                    "Thư giãn với em đi a",
                    "A cần em lúc nào cũng được",
                    "E ở đây để làm anh vui",
                    "Hãy để em chăm sóc a",
                    ]
            },
            {
                name: "Minh tuấn",
                avatar: "https://i.ibb.co/pKmXwrY/272866135-337414368258588-1908917876419985919-n.jpg",
                messages: [
                "Thế sao bác ko xơi mak còn ở đây 😆",
        "Đơn giản thôi. Hết tiền 😐😐",
        "https://i.ibb.co/pjSHRhc/photo-44-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/WyBRncv/photo-45-2024-10-23-11-22-02.jpg",
        "Vú này kh ngon thì vú mô ngon nữa",
        "Đưa tôi bú thử biết liền",
        "Địt thì địt đi ngon hay dở bọn tôi có ăn dc đâu vl 😐",
                ]
            },
            {
                name: "khaiminh",
                avatar: "https://i.ibb.co/g41VJkW/272882107-1743526929177041-8680476091434594245-n.jpg",
                messages: [
                "Ae đi cày mà lấy tiền đi đụ đĩ",
                    "Dễ thương lắm bé ơi",
                    "Mấy bé chụp hình dễ thương mà ở ngoài còn dễ thương hơn",
                    "https://i.ibb.co/SvrxbV1/photo-45-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/hCtwGhB/photo-46-2024-10-23-11-52-15.jpg",
                    "1 lúc mấy e thế kia có mà ngại chết sức đâu mà địt cho nổi",
                    "Cuộc sống đại gia mới dám chơi kiểu này chứ đi cày bục mặt tiền đâu mà chơi 1 lúc mấy e",
                    "Chơi để điện ngắm các em cho sướng chứ tắt làm j ông",
                    "Thôi ae chơi bình dân 1 mình 1 em thôi chơi gì mà mình 3 em có mà đi k nổi",
                ]
            },
            {
                name: "minhchinh11",
                avatar: "https://i.ibb.co/D4fNcr1/273051301-4626795057440307-6858749945339263461-n.jpg",
                messages: [
                "Làm 2 nháy lô thì dữ tiền đi nên k thành vấn đề",
                    "Kaka nhiều lúc ae phải thử cảm giác lạ chứ sống mà k thử sau già hối hận đấy",
                    "Mệt mỏi j có gái nằm đợi sẵn thế kia mỏi đến mấy cũng đè ra đụ cái",
                    "https://i.ibb.co/ZBL16zc/photo-47-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/F8htkCL/photo-48-2024-10-23-11-22-02.jpg",
                    "Quá mệt mỏi rồi k biết nên làm gì tiếp đây",
                    "Mấy bác gọi mấy e nó đến phục vụ đi tầm này là giờ đẹp rồi",
                    "Bú liếm mà mặt e nó nhìn phê phê",
                    "Nhìn ngon nhỉ zú căng chắc thủ gọi e nó check hàng phát",
                ]
            },
            {
                name: "huyduong",
                avatar: "https://i.ibb.co/L6jL23M/277773094-370824451584246-7873142226701853158-n.jpg",
                messages: [
                "Mẹ kiếp lại phải ra khách sạn gọi 1 em đến phục vụ",
                    "Có ae ở cùng có ng yêu đôi lúc khó chịu phết nhỉ",
                    "Ae nó có hàng đưa về mừng cho nó chứ",
                    "Đồ ngon đấy có bạn hiền gái đẹp nữa là ok",
                    "https://i.ibb.co/47jG43K/photo-49-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/KNDSTNF/photo-50-2024-10-23-11-52-15.jpg",
                    "Mẹ các bố kiếm gái đi chơi hay j thì nt cho nó đúng ng bố khỉ tự dung có thằng nt đến bảo book e đi chơi nổi da gà",
                    "Bế e nó ra ban công chơi cho cảm giác lạ",
                    "Đc đấy nhỉ chơi kiểu này tung tóe nc",
                    "Chơi e nó trong bồn tắm cảm giác nó phê thì hết chỗ nói",
                    "Má nó chứ gọi call mấy e tý mà các e nó bận quá",
                    "https://i.ibb.co/FbGD5wD/photo-62-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/Dg19W52/photo-62-2024-10-23-11-52-15.jpg",
                    "Bác kết em ngon thế này đúng quá ok",
                    ] 
            },
            {
                name: "QUỲNH HƯƠNG",
                avatar: "https://i.ibb.co/1TJpcNr/review-of-hai-thien-for-new-hai-duong-teen-2k-nang-tho-cua-moi-checker-gap-la-me-3268642-original.jpg",
                messages: [
                "E rảnh đây có anh nào cần k",
        "Đêm nay e ở đây chờ các a đặt lịch nhé",
        "Có muốn lên lịch với e không",
        "E luôn sẵn sàng đợi a book",
        "A nào muốn đặt lịch book e chưa",
                ]
            },
            {
                name: "sangdai2001",
                avatar: "https://i.ibb.co/4MP92k3/292415446-2231900230303702-1960046090389404713-n.jpg",
                messages: [
                "Mối quen mà chơi cho nó bú liếm hehe",
                    "Mấy e ở đây e nào chả trẻ với ngon mà cứ đặt mấy e hot",
                    "Thiếu j em ngon đâu bác",
                    "Có mấy em đang hot trên web kìa ae lên đặt lịch ngay kẻu lại hết phần",
                    "E nó bảo a ơi bắn vào mồm e nhé",
                    "https://i.ibb.co/GPhbK9W/photo-51-2024-10-23-11-51-38.jpg",
"https://i.ibb.co/bgh2gck/photo-35-2024-10-23-11-52-30.jpg",
                    "Chơi 1 em đã cứng mẹ giò rồi còn đâu mà có sức chơi mấy em 1 lúc hả b",
                    "Xuất xong e nó bú mà k chịu nổi",
                    "Má lên chọn mấy e mà thấy e nào cũng ngon",
                    "Mấy e mái đây cắt tỉa lông lồn gọn gàng nhỉ",
                    "Đéo như mấy quán hát với massa kia đéo biết làm tình j hết chơi chán vl",
                    ]
            },
            {
                name: "datlanday",
                avatar: "https://i.ibb.co/z7xGM2z/301855321-467074835292540-5086007929985430333-n.jpg",
                messages: [
                "Mà đéo có gái là con cu nó hỏng",
        "Mông má nhìn đúng tiêu chuẩn rồi",
        "https://i.ibb.co/55PGJHx/photo-52-2024-10-23-11-22-02.jpg",
"https://i.ibb.co/D1b6Ngv/photo-53-2024-10-23-11-22-02.jpg",
        "Ae thấy e hàng này dáng nuột k",
        "https://i.ibb.co/sHTf8QH/travelodge-dongadaemun.jpg",
        "Đã đứng kiểu nMà chơi mấy chị lớn tuổi có khả năng kỹ năng làm tình thì thôi rồi nhỉ hôm nào thử phát lái máy bay xem sao kkkk",
        ]
            },
            {
                name: "longtu",
                avatar: "https://i.ibb.co/7tMsbq6/301881035-3391721564479335-5156237668196575911-n.jpg",
                messages: [
                "Mấy ae lên web đặt lịch nay t thấy có mấy bé nhìn ngon đòn lắm",
        "Đúng k có gái là con cu đéo biết xả ở đâu",
        "https://i.ibb.co/ncjgPsG/photo-39-2024-10-23-11-52-30.jpg",
"https://i.ibb.co/YPc3hBG/photo-56-2024-10-23-11-22-02.jpg",
        "Vú này kh ngon thì vú mô ngon nữa",
        "https://i.ibb.co/7GjkJcg/travelodge-dongadaemun-1.jpg",
        "Thi thoảng làm tý cho nó thông thái cái đầu óc",
        "Đặt lịch mấy e đó khó lắm toàn phải đặt trước 2 3 ngày thôi",
                ]
            },
            {
                name: "Phucquy",
                avatar: "https://i.ibb.co/HFmN3VJ/307175241-485972230069467-1336353791094509721-n.jpg",
                messages: [
                "Hàng mới cập nhật trên web ông bạn k xem à",
                "https://i.ibb.co/0GmtgRX/photo-61-2024-10-23-11-22-02.jpg",
"https://i.ibb.co/kGQtzb0/photo-61-2024-10-23-11-52-15.jpg",
        "T chơi cũng nhiều chỗ rồi mà mấy e ở đây làm tình đúng giỏi",
        "https://i.ibb.co/mDgpphk/photo-2024-07-17-22-06-53.jpg",
        "sợ mấy CLB vl giờ mới biết ở đây toàn gái ngon",
        "Mất thì nghỉ đit có chi đâu",
                ]
            },
            {
                name: "Đạt09",
                avatar: "https://i.ibb.co/d0xbBQS/332691797-3517976848448705-7386835105659429453-n.jpg",
                messages: [
                "Địt đi rồi review tôi xem phát kk",
        "Thế đợi hóng nha 😂😂",
        "Múp máp đấy mà nhậu ít lại nha b 😁",
        "https://i.ibb.co/yVJ0YX6/photo-56-2024-10-23-11-52-15.jpg",
"https://i.ibb.co/Dfg6cwr/photo-60-2024-10-23-11-52-15.jpg",
        "Đụ vào NGÀY THƯỜNG thì tha hồ mà chọn gái ngon",
          
            ],
          },
        ];
        function startChat() {
    userName = document.getElementById("user-name").value;
    if (!userName || !userAvatar) {
        alert("Vui lòng nhập tên và chọn ảnh đại diện.");
        return;
    }
    document.getElementById("user-setup").style.display = "none";
    document.getElementById("chat-container").style.display = "flex";
}

function loadAvatar(event) {
    const file = event.target.files[0];
    if (file) {
        const reader = new FileReader();
        reader.onload = function (e) {
            userAvatar = e.target.result;
        };
        reader.readAsDataURL(file);
    }
}

function getRandomMessage(character) {
    let message;
    do {
        const randomIndex = Math.floor(Math.random() * character.messages.length);
        message = character.messages[randomIndex];
    } while (recentMessages.includes(message) && recentMessages.length < maxNoRepeat);

    recentMessages.push(message);
    if (recentMessages.length > maxNoRepeat) recentMessages.shift();

    return message;
}

function sendRandomMessage() {
    const chatBox = document.getElementById("chat-box");
    const character = characters[Math.floor(Math.random() * characters.length)];
    const randomMessage = getRandomMessage(character);

    const messageElement = document.createElement("div");
    messageElement.classList.add("chat-message", "character-message");

    const avatarElement = document.createElement("img");
    avatarElement.src = character.avatar;
    avatarElement.classList.add("avatar");

    const messageBubble = document.createElement("div");
    messageBubble.classList.add("message-bubble");

    const userNameElement = document.createElement("div");
    userNameElement.classList.add("user-name");
    userNameElement.textContent = character.name;

    const messageContentElement = document.createElement("div");
    messageContentElement.classList.add("message-content");

    if (isValidImageUrl(randomMessage)) {
        const imgElement = document.createElement("img");
        imgElement.src = randomMessage;
        imgElement.style.maxWidth = "100%";
        imgElement.style.height = "auto";
        messageContentElement.appendChild(imgElement);
    } else if (isValidVideoUrl(randomMessage)) {
        const videoElement = document.createElement("video");
        videoElement.src = randomMessage;
        videoElement.controls = true;
        videoElement.style.maxWidth = "100%";
        videoElement.style.height = "auto";

        // Mute/unmute button for video
        const muteButton = document.createElement("button");
        muteButton.textContent = "Mute";
        muteButton.classList.add("mute-button");
        muteButton.onclick = function () {
            videoElement.muted = !videoElement.muted;
            muteButton.textContent = videoElement.muted ? "Unmute" : "Mute";
        };
        messageContentElement.appendChild(muteButton);
        messageContentElement.appendChild(videoElement);
    } else {
        messageContentElement.textContent = randomMessage;
    }

    const messageStatus = document.createElement("span");
    messageStatus.classList.add("message-status");
    messageStatus.textContent = "✓";

    setTimeout(() => {
        messageStatus.textContent = "✓✓";
    }, 3000);

    messageBubble.appendChild(userNameElement);
    messageBubble.appendChild(messageContentElement);
    messageBubble.appendChild(messageStatus);

    messageElement.appendChild(avatarElement);
    messageElement.appendChild(messageBubble);

    chatBox.appendChild(messageElement);
    chatBox.scrollTop = chatBox.scrollHeight;

    // Check if the chat box is visible
    const chatContainer = document.getElementById("chat-container");
    if (chatContainer.style.display === "none") {
        newMessagesCount++;
        document.title = `(${newMessagesCount}) New Message(s)`;
    }

    const randomInterval = Math.random() * (5000 - 2000) + 2000; // Interval from 2 to 5 seconds
    setTimeout(sendRandomMessage, randomInterval);
}

function isValidImageUrl(url) {
    return url.match(/\.(jpeg|jpg|gif|png|bmp)$/i);
}

function isValidVideoUrl(url) {
    return url.match(/\.(mp4|webm|ogg)$/i);
}

function sendImageMessage(event) {
    const file = event.target.files[0];
    if (file) {
        const reader = new FileReader();
        reader.onload = function (e) {
            createMessageElement(userName, userAvatar, e.target.result, true);
        };
        reader.readAsDataURL(file);
    }
}

function sendVideoMessage(event) {
    const file = event.target.files[0];
    if (file) {
        const reader = new FileReader();
        reader.onload = function (e) {
            createMessageElement(userName, userAvatar, e.target.result, false, true);
        };
        reader.readAsDataURL(file);
    }
}

function sendTextMessage() {
    const chatInput = document.getElementById("chat-input");
    const message = chatInput.value.trim();
    if (message) {
        createMessageElement(userName, userAvatar, message);
        chatInput.value = "";
    }
}

function createMessageElement(name, avatar, content, isImage = false, isVideo = false) {
    const chatBox = document.getElementById("chat-box");

    const messageElement = document.createElement("div");
    messageElement.classList.add("chat-message", "self");

    const avatarElement = document.createElement("img");
    avatarElement.src = avatar;
    avatarElement.classList.add("avatar");

    const messageBubble = document.createElement("div");
    messageBubble.classList.add("message-bubble");

    const userNameElement = document.createElement("div");
    userNameElement.classList.add("user-name");
    userNameElement.textContent = name;

    const messageContentElement = document.createElement("div");
    messageContentElement.classList.add("message-content");

    if (isImage) {
        const imgElement = document.createElement("img");
        imgElement.src = content;
        imgElement.style.maxWidth = "100%";
        imgElement.style.height = "auto";
        messageContentElement.appendChild(imgElement);
    } else if (isVideo) {
        const videoElement = document.createElement("video");
        videoElement.src = content;
        videoElement.controls = true;
        videoElement.style.maxWidth = "100%";
        videoElement.style.height = "auto";
        messageContentElement.appendChild(videoElement);
    } else {
        messageContentElement.textContent = content;
    }

    const messageStatus = document.createElement("span");
    messageStatus.classList.add("message-status");
    messageStatus.textContent = "✓";

    setTimeout(() => {
        messageStatus.textContent = "✓✓";
    }, 3000);

    messageBubble.appendChild(userNameElement);
    messageBubble.appendChild(messageContentElement);
    messageBubble.appendChild(messageStatus);

    messageElement.appendChild(avatarElement);
    messageElement.appendChild(messageBubble);

    chatBox.appendChild(messageElement);
    chatBox.scrollTop = chatBox.scrollHeight;
}

function toggleChat() {
    const chatContainer = document.getElementById("chat-container");
    chatContainer.style.display = chatContainer.style.display === "flex" ? "none" : "flex";

    // Reset new message count when opening chat
    if (chatContainer.style.display === "flex") {
        newMessagesCount = 0;
        document.title = "Chat App";
    }
}

function toggleDarkMode() {
    document.body.classList.toggle("dark-mode");
    const chatBox = document.getElementById("chat-container");
    const isDarkMode = document.body.classList.contains("dark-mode");

    // Change background color of chat box based on dark mode
    chatBox.style.backgroundColor = isDarkMode ? "#333" : "#fff";
    chatBox.style.color = isDarkMode ? "#fff" : "#000";
}

// Start sending random messages
sendRandomMessage();
    </script>
</body>
</html>


<!-- CSS cho các nút phim 18+ -->
<style>
.submenu {
    display: none;
    flex-wrap: wrap; /* Cho phép nút xuống hàng khi không đủ không gian */
    gap: 10px;
}

.phim-btn {
    font-size: 13px;
    padding: 5px 9px;
    background: #000000;
    color: #ffffff; /* Chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
    border-radius: 5px;
    font-weight: 750; /* Chữ đậm nhưng nhẹ hơn */
    cursor: pointer;
    flex-basis: 22%; /* Chiều rộng mỗi nút */
    text-align: center;
    box-sizing: border-box;
    border: 2px solid #C0C0C0; /* Viền bạc */
    transition: background-color 0.3s ease, transform 0.3s ease; /* Hiệu ứng chuyển đổi */
}

.phim-btn:hover {
    background-color: #ffffff; /* Màu nền khi hover */
    transform: scale(1.05); /* Phóng to nhẹ khi hover */
}
</style>


<style>
    /* Điều chỉnh kích thước các nút menu */
   
    
  
    .menu-item:hover {
        background-color: #ffffff; /* Màu nền khi hover */
        color: #000000; /* Màu chữ vàng */
    }
    
  a {
    text-decoration: none;
  }

  .support-button {
    display: block; /* Để các nút xếp dọc */
    padding: 5px 10px;
    margin: 10px 0;
    background: #000000;
    color: #ffffff; /* Chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
    text-decoration: none;
    width: 150px;
    border-radius: 5px;
    text-align: center;
    transition: background-color 0.3s ease, transform 0.3s ease; /* Hiệu ứng chuyển đổi */
    border: 2px solid #ffffff; /* Viền bạc */
}

.support-button:hover {
    background-color: #ffffff; /* Màu nền khi hover */
    color: #000000; /* Chữ đen */
    transform: scale(1.05); /* Phóng to nhẹ khi hover */
}

.support-button i {
    margin-right: 8px; /* Khoảng cách giữa icon và chữ */
}


</style>


<!-- Hỗ trợ nhanh -->
<div id="support-section" class="content">
    <h2>Hỗ trợ</h2>
    <p>Để nhận được hỗ trợ nhanh hơn bạn vui lòng liên hệ qua Telegram nhé:</p>
    <a href="https://t.me/phuongthaoinh" target="_blank" class="support-button">
        <i class="fab fa-telegram-plane"></i> Hỗ trợ tổng
    </a>
    <a href="https://Honganhxin" target="_blank" class="support-button">
        <i class="fab fa-telegram-plane"></i> Hỗ trợ viên 2
    </a>
    <a href="https://yennhi1999aa" target="_blank" class="support-button">
        <i class="fab fa-telegram-plane"></i> Hỗ trợ viên 3
    </a>
    <a href="" target="thuongvy8386aa" class="support-button">
        <i class="fab fa-telegram-plane"></i> Hỗ trợ viên 4
    </a>
    
</div>

<!-- JavaScript để quản lý chat -->
<script>
    const messagesDiv = document.getElementById('messages');
    const sendBtn = document.getElementById('send-btn');
    const nicknameInput = document.getElementById('nickname');
    const chatInput = document.getElementById('chat-input');

    // Khi nhấn nút gửi
    
    sendBtn.addEventListener('click', function() {
        const nickname = nicknameInput.value.trim();
        const message = chatInput.value.trim();

        if (nickname && message) {
            // Tạo một dòng tin nhắn mới
            const newMessage = document.createElement('div');
            newMessage.textContent = `${nickname}: ${message}`;
            messagesDiv.appendChild(newMessage);

            // Xóa nội dung tin nhắn sau khi gửi
            chatInput.value = '';
        } else {
            alert("Vui lòng nhập tên và tin nhắn.");
        }
    });
</script>


</body>
</html>



<div id="image-section" class="content">
    <h2>Ảnh sex</h2>
    
    <!-- Thêm các nút cho từng danh mục -->
    <div class="image-buttons">

        <button class="image-btn" onclick="showContent('vietnamese-girls')">
            Ảnh Gái Trung
        </button>
        <button class="image-btn" onclick="showContent('call-girls-share')">
            Share Gái Gọi
        </button>
        <button class="image-btn" onclick="showContent('asian-girls')">
            Ảnh Gái Châu Á
        </button>
        <button class="image-btn" onclick="showContent('stolen-photos')">
            Chụp Lén - Lộ Hàng
        </button>
    </div>
    
    <!-- Các phần nội dung hiển thị khi bấm vào nút -->
    <div id="upcoming" class="image-content" style="display:none;">
        <p>Bạn chưa đủ điều kiện để truy cập vào các dịch vụ đặc biệt của hệ thống 💎</p>
        <img src="https://i.ibb.co/RcJCBVD/photo-3-2024-10-23-11-52-30.jpg" alt="Hàng Sắp Lên Sóng" style="width:150px; height:auto; margin:10px;">
    </div>

    <div id="vietnamese-girls" class="image-content" style="display:none;">
        <p>Ảnh gái Trung với dàn mỹ nữ hấp dẫn 💎</p>
        <img src="https://i.ibb.co/Qk3G8wz/photo-2024-07-10-17-13-32.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/GCjdNtx/photo-2024-09-18-13-45-33-2.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/17WDq5j/photo-2024-09-18-13-45-33.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/6v1tmrc/photo-2024-09-18-13-45-09.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/5xtKL6Z/photo-2024-10-21-17-32-43.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/T06zgX2/photo-2024-10-21-17-32-42-3.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/093GT80/photo-2024-10-21-17-32-42-2.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/tcJBTbH/photo-2024-10-21-17-32-42.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/fSYLJd6/photo-2024-10-21-17-32-41.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/sgpjqm0/photo-2024-10-21-17-32-40.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/rb39Mrr/photo-2024-10-21-17-32-38.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Ld1BwS6/photo-2024-10-21-17-32-37.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Xp0btSJ/photo-2024-10-21-14-04-39.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/0KWPgyC/photo-2024-10-21-14-04-37.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/rvs3q7z/photo-2024-10-21-14-04-35.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/N1gFXm6/photo-2024-10-21-14-04-33.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/VQjhHkb/photo-2024-10-21-13-41-02.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/JjQmQRr/photo-2024-10-21-13-45-21.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/3M4mQCY/photo-2024-10-20-17-09-47.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/9V2Lt9V/photo-2024-10-20-20-15-28.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Qm0mSkG/photo-2024-10-20-19-33-52.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/vDhPdsQ/photo-2024-10-20-19-33-51.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/RYT9ww2/photo-2024-10-20-19-33-50.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/bFs7KGH/photo-2024-10-20-19-33-49.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/D4RMtBW/photo-2024-10-20-16-39-12.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/bdxHhdS/photo-2024-10-20-16-39-07-2.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/KXN8R9W/photo-2024-10-20-16-39-07.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/T8YyX9Y/photo-2024-10-20-16-39-06.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/5nYPQVt/photo-2024-10-18-19-06-20.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/NYphctp/photo-2024-10-18-19-06-19-2.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/vvR4TGZ/photo-2024-10-18-19-06-19.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/XLzcVGV/photo-2024-10-18-19-06-18.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/S6QF7Mm/photo-2024-10-18-19-06-13.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/9HwnNqt/photo-2024-10-18-19-06-09.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/h1RGKMq/photo-2024-10-19-23-20-48.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/WygYWcn/photo-2024-10-19-23-09-11.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/PDvK9q0/photo-2024-10-19-23-09-12.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/cghMmPY/photo-2024-10-19-23-20-47.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/ZJx2SKR/photo-2024-09-22-16-55-21.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/TcnYGrJ/photo-2024-09-22-16-55-19.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/0QjsB7D/photo-2024-09-22-16-55-20.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/MkCSGF3/photo-2024-09-22-16-55-18.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Wgxrh6M/photo-2023-08-18-17-23-44.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/YcNs51k/photo-2023-08-18-17-23-43.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
 <img src="https://i.ibb.co/CB2DBDc/photo-2023-08-18-17-23-41.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/3sSDDN5/photo-2023-08-18-17-20-51.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/gTqn2C6/photo-2024-09-20-15-57-28.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/smGnhFx/photo-2024-09-20-15-57-26.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/98rdtdN/photo-2024-09-20-15-57-25.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/mhGHhvd/photo-2024-09-20-15-57-24-2.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/GJdLtRV/photo-2024-09-20-15-57-24.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/x79x9dr/photo-2024-09-20-15-57-23.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/PW1Pc82/photo-2024-09-20-15-57-22.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/mDp6jhs/photo-2024-09-20-15-57-21.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/3SqVSK4/photo-2024-10-19-18-56-08.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/t8Sct1S/photo-2024-10-19-15-55-51.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/9pdsVCB/photo-2024-10-19-15-55-50-6.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/6ZJwzpB/photo-2024-10-19-15-55-50-5.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/0n9NYNz/photo-2024-10-19-15-55-50-4.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/W0vkMqF/photo-2024-10-19-15-55-50-3.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/44RLD14/photo-2024-10-19-15-55-50-2.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/mJLGTx5/photo-2024-10-19-15-55-50.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/GQwhJdH/photo-2024-10-18-21-32-00.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/crS583t/photo-2024-10-18-21-31-38.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Q6KT80y/photo-2024-10-18-21-31-20.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/PNsXg1K/photo-2024-10-18-21-31-04.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/R4cPs0S/photo-2024-10-18-21-30-55.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/2nkw2Yd/photo-2024-10-18-21-30-50.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/vBRjQns/photo-2024-10-17-22-10-32.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/CQDHrwM/photo-2024-09-14-15-40-34.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/qRqNJw5/photo-2024-09-14-15-40-33.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/tBtrbZm/photo-2024-09-14-15-40-32.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/3WmZtsj/photo-2024-09-14-15-40-26.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/S5QxH6k/photo-2024-10-17-19-19-54.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/KqrvZg0/photo-2024-10-17-19-19-53.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;"> 
<img src="https://i.ibb.co/RC5YYFs/photo-2024-10-17-19-19-57.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/TBRDN7P/photo-2024-10-17-19-19-25.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/4N5LhSt/photo-2024-10-17-19-19-55.jpg" alt="Ảnh Gái Trung" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/cFT7Xdv/photo-2024-10-12-21-28-05.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/cLTVGQD/photo-2024-10-12-21-38-15.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Qk3G8wz/photo-2024-07-10-17-13-32.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/rtPmgjb/photo-2024-07-10-17-13-34.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/r6XvW70/photo-2024-07-10-17-13-35-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/xM4yCDZ/photo-2024-07-10-17-13-35.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/wMFqXbc/photo-2024-10-13-14-43-22.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/PDjrtbk/photo-2024-10-13-14-43-21.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/cYTPtyF/photo-2024-09-23-21-56-07.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/JBwCvf7/photo-2024-09-14-19-57-25.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/K500cBb/photo-2024-09-14-19-57-28.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/6WQMXvN/photo-2024-09-14-19-57-29-3.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/wYx9VNR/photo-2024-09-14-19-57-29-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/VM5wJWH/photo-2024-09-14-19-57-29.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/9HkwjTW/photo-2024-10-13-19-40-12-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/mt1Yd02/photo-2024-10-13-19-40-12.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/4fWFxPR/photo-2024-10-13-19-40-13.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/2h37d5L/photo-2024-10-13-19-40-15.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/KctRfv2/photo-2024-10-13-19-40-16.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/ydp0gh8/photo-2024-10-13-19-40-17.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/3mBrgWb/photo-2024-10-14-11-11-07.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/P4cf9fY/photo-2024-10-14-11-11-08-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/9wXQjxm/photo-2024-10-14-11-11-08.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/w7RGs20/photo-2024-10-14-11-11-09.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Lx39B33/photo-2024-10-14-11-11-10.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/RcsP2Dy/photo-2024-10-14-11-11-11.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/tq4jVwY/photo-2024-10-14-11-11-12.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/5hRTBz6/photo-2024-10-14-11-11-13.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/j5tr3VR/photo-2024-10-14-11-11-14.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/9GXh2bS/photo-2024-10-14-12-48-02.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/p0pRVDG/photo-2024-10-14-12-48-03.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/SR0FWRr/photo-2024-10-14-12-48-04.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Hdqwzrd/photo-2024-10-14-12-48-05.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/6gysvRb/photo-2024-10-14-12-48-06-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/gdQ5bBD/photo-2024-10-14-12-48-06.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/1bLZVxv/photo-2024-10-14-20-24-17.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/SBz1FKb/photo-2024-10-14-20-24-02.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/P6G9ZVM/photo-2024-10-14-20-42-13.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/P6G9ZVM/photo-2024-10-14-20-42-13.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/z5bz2jT/photo-2024-10-14-20-32-22-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/m8G5cfM/photo-2024-10-14-20-32-22.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/8bK2bj3/photo-2024-10-15-21-29-25.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/GQnhfgY/photo-2024-10-15-21-56-17.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/XDmv5Nf/photo-2024-10-15-21-56-18-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/jLHkJwf/photo-2024-10-15-21-56-18.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/rpDP372/photo-2024-10-15-21-56-19.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/N1BVgkM/photo-2024-09-06-20-30-01.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/16TFgg7/photo-2024-09-06-20-29-59.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/QvNRr3k/photo-2024-09-06-20-30-09.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Kz7ZSph/photo-2024-09-06-20-30-10.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/7jjDMYp/photo-2024-09-06-20-30-12.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/DrY7DCC/photo-2024-09-06-20-30-07.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/nQPCKrJ/photo-2024-10-16-19-27-04-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/jZtqt3G/photo-2024-10-16-19-27-04.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/pdbnRgS/photo-2024-10-24-21-55-05.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/N1Xysv6/photo-2024-10-24-21-55-00.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/6wWFk1Z/photo-2024-10-24-21-54-58.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/WBjqRX6/photo-2024-10-24-21-54-55.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/hDB7H91/photo-2024-10-24-21-54-52.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/X7jyMrb/photo-2024-09-14-00-09-24.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/F8zv4pT/photo-2024-09-14-00-09-23.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/MVvpQgT/photo-2024-09-14-00-09-21.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/tmdncQL/photo-2024-09-14-00-09-17.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/pJ6wg7K/photo-2024-10-23-21-37-11.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/2dhg0m3/photo-2024-10-23-21-37-10.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/3M4mQCY/photo-2024-10-20-17-09-47.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/SXZ7ccK/photo-2024-09-11-14-10-34.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/pjhGqgj/photo-2024-09-11-14-10-33-3.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/9qBXbtP/photo-2024-09-11-14-10-33-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/CtSpPcD/photo-2024-09-11-14-10-33.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/7tL5cyM/photo-2024-09-11-14-10-32-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Lk5Cp82/photo-2024-09-11-14-10-32.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/cFHdQCq/photo-2024-10-22-20-33-27-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/zb7htds/photo-2024-10-22-20-33-27.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/86tNb8k/photo-2024-10-22-20-33-26.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/RCRbrY8/photo-2024-10-22-20-33-25.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/gyvRCzd/photo-2024-09-18-13-45-33-4.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/DRFVwJy/photo-2024-09-18-13-45-33-3.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/P5ptQM5/photo-2023-11-29-21-50-11.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/v1cHvYj/photo-2023-11-29-21-50-15.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Tcn5tSB/photo-2023-11-29-21-50-17.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/W612CtQ/photo-2023-11-29-21-50-21.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/fvPDWm7/photo-2023-11-29-21-50-23.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/XjFCRwH/photo-2023-11-29-21-50-25.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/27vzBdN/photo-2023-11-29-21-50-47.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/cDZX9X3/photo-2023-11-29-21-50-28.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/HC7bKYg/photo-2023-11-29-21-50-31.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/W09fwTB/photo-2024-09-28-22-03-41.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/PmrbN35/photo-2024-09-28-22-03-21.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/zV1m6sm/photo-2024-09-28-22-03-12.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/kh6Z8qD/photo-2024-09-28-22-03-02.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/WDkhdvb/photo-2024-09-28-22-02-42.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/3BT5TCV/photo-2024-09-28-22-02-29.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/VYnz5DX/photo-2024-09-28-22-02-17.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/db4CPbL/photo-2024-09-29-21-07-57.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/wQQG8SK/photo-2024-09-29-21-07-58.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/09qSvH6/photo-2024-09-29-21-07-59-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/DM8spTR/photo-2024-09-29-21-07-59.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/j6BTqy3/photo-2024-09-29-21-08-00.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/WVNcrcq/photo-2024-09-29-21-08-01-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/F7BRPH1/photo-2024-09-29-21-08-01.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/qWHGdSH/photo-2024-09-30-18-39-29.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/kqWxrym/photo-2024-09-30-18-39-30.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/84z66nz/photo-2024-09-30-18-39-31-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/7QDJQQd/photo-2024-09-30-18-39-31.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/mz0PPnL/photo-2024-09-30-18-39-34-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/hXJj5gW/photo-2024-09-30-18-39-34.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Xx0VXr0/photo-2024-09-30-18-39-35.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/vXqhg7P/photo-2024-09-30-18-39-33.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/sCxG9SL/photo-2024-09-30-18-39-32-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Q808KVD/photo-2024-09-30-18-39-32.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/bJTDgtC/photo-2024-09-30-20-58-57.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/qgqFRBL/photo-2024-09-30-20-58-50.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Kx2Xt2J/photo-2024-09-30-20-58-54.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/7JBRTW6/photo-2024-09-30-20-51-54.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/QjCjGVY/photo-2024-09-30-20-52-01.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/WxpFwwn/photo-2024-09-30-20-52-07.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/pR2QCYb/photo-2024-09-30-20-52-10.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/f81k6zn/photo-2024-09-30-20-52-18.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/yNxjz6J/photo-2024-10-02-15-07-09.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/2ZsGyxY/photo-2024-10-02-15-07-06.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/ypkdZkP/photo-2024-10-02-15-07-08.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/8D8zr0N/photo-2024-10-02-15-07-05.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Gs6gCY1/photo-2024-10-02-15-07-03.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/LZXr89N/photo-2024-10-04-22-58-28-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/YL4zspV/photo-2024-10-04-22-58-28.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/jGyGY0p/photo-2024-10-06-16-13-45.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/421rZyS/photo-2024-10-06-16-13-46.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/YLkfQRr/photo-2024-10-06-16-13-47-3.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/McB0RV3/photo-2024-10-06-16-13-47-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/d6Y6RPd/photo-2024-10-06-16-13-47.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/KKqXRXh/photo-2024-10-06-20-11-13.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/fxrWZqG/photo-2024-10-06-20-11-19.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/bs8RNHb/photo-2024-10-06-20-11-24.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/5MK1xbx/photo-2024-10-06-20-11-30.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/v1pFX3R/photo-2024-10-06-20-11-36.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/QYScc53/photo-2024-10-06-20-11-42.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/drVHHPS/photo-2024-10-06-20-11-47.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/gDp1hK0/photo-2024-10-07-14-19-54.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/MV5F6n4/photo-2024-10-07-14-19-56.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/b1fvvWZ/photo-2024-10-07-14-20-00.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/fCg3N1c/photo-2024-10-07-14-20-05.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Wf0CdCY/photo-2024-10-07-14-20-07.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/g42dzyy/photo-2024-10-07-14-20-11.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Ss7qkzL/photo-2024-10-07-14-20-14.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/TtBnfvd/photo-2024-10-07-14-20-18.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/DV7ST2X/photo-2024-10-07-14-52-21.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/nkxNJYQ/photo-2024-10-07-14-52-24.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/HFhKcpZ/photo-2024-10-07-14-52-28.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/RHsZT40/photo-2024-10-07-14-52-31.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/4d9q1hv/photo-2024-10-07-14-52-35.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/d6rwyK2/photo-2024-10-07-14-52-38.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/BgfNWW4/photo-2024-09-09-17-00-04-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/VCywgYG/photo-2024-09-09-17-00-05-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/RPNjt2X/photo-2024-09-09-17-00-06-4.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/KFwvBq2/photo-2024-09-09-17-00-06-3.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/1KYHcqg/photo-2024-10-07-16-49-51.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/nRZpvSj/photo-2024-10-07-16-49-54.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/jvSS1Sm/photo-2024-10-07-16-50-03.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/KwjpR6V/photo-2024-10-07-16-50-07.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/BgfNWW4/photo-2024-09-09-17-00-04-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/VCywgYG/photo-2024-09-09-17-00-05-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/RPNjt2X/photo-2024-09-09-17-00-06-4.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/KFwvBq2/photo-2024-09-09-17-00-06-3.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/D9CDmmx/photo-2024-09-09-17-00-07-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/5Y8hWhZ/photo-2024-09-09-17-00-07.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Lz1nJwG/photo-2024-09-09-17-00-08.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/YDmhNQm/photo-2024-10-08-22-25-41.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Mnf6V8h/photo-2024-10-08-22-25-42.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/vczY23Q/photo-2024-10-08-22-25-43.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/hMVFMh6/photo-2024-10-08-22-25-46.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/9TgKZWf/photo-2024-10-08-22-25-49.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/qd56vFH/photo-2024-10-08-22-49-28.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/BcRsrDm/photo-2024-10-08-22-49-31.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/42w410J/photo-2024-10-08-22-49-29.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/jVskYxM/photo-2024-10-08-22-49-32.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/K5BZrjL/photo-2024-10-08-22-49-33.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/X7tD8q1/photo-2024-10-08-22-49-34.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/fYqHDGs/photo-2024-10-08-22-49-35.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/NSxx001/photo-2024-10-08-22-49-36.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/m0SB7cW/photo-2024-10-09-17-14-16.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/0fz6RpW/photo-2024-10-09-17-14-21.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/n0Yp49N/photo-2024-10-09-18-39-19.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/KswqnKq/photo-2024-10-09-18-39-21.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/59JSdHh/photo-2024-10-09-18-39-26.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/3Wb9p31/photo-2024-10-09-18-39-29-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/3Wb9p31/photo-2024-10-09-18-39-29-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/L6smf4k/photo-2024-10-09-18-39-34.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/cwyPR0K/photo-2024-10-09-19-46-48.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/99ZmS2W/photo-2024-10-09-19-46-57.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/YTH8J9q/photo-2024-10-09-19-47-09.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/k8TmGVT/photo-2024-10-09-19-47-29.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/1m0bC1m/photo-2024-10-09-19-47-30.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/jwwhDjC/photo-2024-10-09-19-47-31.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Nj24sZc/photo-2024-10-09-20-03-30.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/wWMT7RG/photo-2024-10-09-20-03-31.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/5xZQzjV/photo-2024-10-09-20-03-33.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Y3mwh2Q/photo-2024-06-15-21-46-37.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/bsmQ6Kz/photo-2024-06-15-21-46-39.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/W04gzPj/photo-2024-06-15-21-46-34.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/pLhtSVB/photo-2024-06-15-21-46-42.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/r6z0S1t/photo-2024-06-15-21-46-35.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/SXtHPY1/photo-2024-06-15-21-46-31.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Hr59j6H/photo-2024-09-07-22-54-54.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/nRFQtLC/photo-2024-09-07-14-02-44-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/7Gm6LJg/photo-2024-09-07-14-02-44.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/QJZLn3N/photo-2024-09-07-14-14-00.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Gx6gKL7/photo-2024-09-07-22-55-01.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/bghRdWc/photo-2024-09-07-14-15-51.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/JjGgT1q/photo-2024-09-07-14-02-45.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/zbMz9fn/photo-2024-09-07-14-16-29.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/JFhddBX/photo-2024-09-07-22-55-10.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/jrSL9BT/photo-2024-10-11-22-06-55.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/F5LVP9K/photo-2024-10-11-22-06-59-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/f4qbVZm/photo-2024-10-11-22-06-56.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/bd84N4W/photo-2024-10-11-22-06-58.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/F5LVP9K/photo-2024-10-11-22-06-59-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/prL0mgw/photo-2024-10-11-22-33-08.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/SndmLyc/photo-2024-10-11-22-33-09.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/CQRrVMZ/photo-2024-10-11-22-33-10-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/J2qYprC/photo-2024-10-11-22-33-10.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/s2k4Xnq/photo-2024-10-11-22-33-11.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/rQDWnnf/photo-2024-10-11-22-33-12.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/ZcqRhdq/photo-2024-10-12-16-27-24.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/5RNJ7ds/photo-2024-10-12-16-27-26.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/M2GV78B/photo-2024-10-12-16-27-28.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Dr46334/photo-2024-10-12-16-27-30.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Tm2FmMw/photo-2024-10-12-21-28-02.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/1sjyfR3/photo-2024-10-12-21-28-03-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/nkB1cwy/photo-2024-10-12-21-28-03.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/xYnT7fb/photo-2024-10-12-21-28-05-2.jpg" alt="Ảnh" style="width:150px; height:auto; margin:10px;">
</div>

    <div id="call-girls-share" class="image-content" style="display:none;">
        <p>Bộ ảnh chia sẻ gái gọi nóng bỏng và hấp dẫn !</p>
   <img src="https://i.ibb.co/LxN44d6/taoanhdep-lam-net-anh-1528.jpg" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/PG99N7b/photo-1-2024-10-23-11-52-15.jpg" alt="Image 2" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/Nr5qKL2/photo-1-2024-10-23-11-52-30.jpg" alt="Image 3" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/H7gHRfp/photo-2-2024-10-23-11-52-15.jpg" alt="Image 4" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/0jrgC38/photo-2-2024-10-23-11-52-30.jpg" alt="Image 5" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/xSsFcHq/photo-3-2024-10-23-11-22-02.jpg" alt="Image 6" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/WsNDbnK/photo-3-2024-10-23-11-52-15.jpg" alt="Image 7" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/RcJCBVD/photo-3-2024-10-23-11-52-30.jpg" alt="Image 8" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/Pt3cqrf/photo-4-2024-10-23-11-51-38.jpg" alt="Image 9" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/p2vNxfh/photo-4-2024-10-23-11-52-15.jpg" alt="Image 10" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/R9bZwr9/photo-4-2024-10-23-11-52-30.jpg" alt="Image 11" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/2jv4sMs/photo-5-2024-10-23-11-22-02.jpg" alt="Image 12" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/L0n93cz/photo-5-2024-10-23-11-52-15.jpg" alt="Image 13" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/WzXRhQg/photo-5-2024-10-23-11-52-30.jpg" alt="Image 14" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/hMqKzQ9/photo-6-2024-10-23-11-51-38.jpg" alt="Image 15" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/ZBmG87y/photo-6-2024-10-23-11-52-30.jpg" alt="Image 16" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/MB3Gct7/photo-7-2024-10-23-11-51-38.jpg" alt="Image 17" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/X8922pL/photo-7-2024-10-23-11-52-15.jpg" alt="Image 18" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/p4XzgtY/photo-7-2024-10-23-11-52-30.jpg" alt="Image 19" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/y6Pt5MW/photo-8-2024-10-23-11-51-38.jpg" alt="Image 20" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/b2BxRcW/photo-8-2024-10-23-11-52-15.jpg" alt="Image 21" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/n0Xhxs4/photo-9-2024-10-23-11-22-02.jpg" alt="Image 22" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/ZXQz03b/photo-9-2024-10-23-11-52-15.jpg" alt="Image 23" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/PQHwdMm/photo-9-2024-10-23-11-52-30.jpg" alt="Image 24" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/YXh9kKb/photo-10-2024-10-23-11-22-02.jpg" alt="Image 25" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/tbypMvJ/photo-10-2024-10-23-11-52-15.jpg" alt="Image 26" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/2yHwZhZ/photo-10-2024-10-23-11-52-30.jpg" alt="Image 27" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/X5ks6CP/photo-11-2024-10-23-11-22-02.jpg" alt="Image 28" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/vVNVr7n/photo-11-2024-10-23-11-52-15.jpg" alt="Image 29" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/865k7YW/photo-11-2024-10-23-11-52-30.jpg" alt="Image 30" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/k3hTjQD/photo-12-2024-10-23-11-22-02.jpg" alt="Image 31" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/Tk833Hn/photo-12-2024-10-23-11-52-15.jpg" alt="Image 32" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/3cPH7hj/photo-12-2024-10-23-11-52-30.jpg" alt="Image 33" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/dBv8yd2/photo-13-2024-10-23-11-22-02.jpg" alt="Image 34" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/SNmpdgf/photo-13-2024-10-23-11-52-15.jpg" alt="Image 35" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/71Y3C62/photo-14-2024-10-23-11-51-38.jpg" alt="Image 36" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/ykbKDdF/photo-14-2024-10-23-11-52-15.jpg" alt="Image 37" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/0sYx3Dn/photo-14-2024-10-23-11-52-30.jpg" alt="Image 38" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/12mwWRg/photo-15-2024-10-23-11-22-02.jpg" alt="Image 39" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/Bnytcwr/photo-15-2024-10-23-11-52-15.jpg" alt="Image 40" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/g7nCYc4/photo-15-2024-10-23-11-52-30.jpg" alt="Image 41" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/d2FxT6x/photo-16-2024-10-23-11-51-38.jpg" alt="Image 42" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/nP596XN/photo-16-2024-10-23-11-52-15.jpg" alt="Image 43" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/54G8SY8/photo-16-2024-10-23-11-52-30.jpg" alt="Image 44" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/7CS5z7s/photo-17-2024-10-23-11-22-02.jpg" alt="Image 45" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/d0Cvktp/photo-17-2024-10-23-11-52-15.jpg" alt="Image 46" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/vLcGbVx/photo-18-2024-10-23-11-51-38.jpg" alt="Image 47" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/hKvSffj/photo-18-2024-10-23-11-52-15.jpg" alt="Image 48" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/ZXQJP5M/photo-18-2024-10-23-11-52-30.jpg" alt="Image 49" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/gM42Djp/photo-19-2024-10-23-11-22-02.jpg" alt="Image 50" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/cQ5jYtH/photo-19-2024-10-23-11-52-15.jpg" alt="Image 51" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/tHxqtYY/photo-19-2024-10-23-11-52-30.jpg" alt="Image 52" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/fdC2Vqn/photo-20-2024-10-23-11-51-38.jpg" alt="Image 53" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/RCknckF/photo-20-2024-10-23-11-52-15.jpg" alt="Image 54" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/WfYvTpm/photo-20-2024-10-23-11-52-30.jpg" alt="Image 55" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/rMrN3cG/photo-21-2024-10-23-11-22-02.jpg" alt="Image 56" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/vJYf7L9/photo-21-2024-10-23-11-52-15.jpg" alt="Image 57" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/yP9ncXw/photo-21-2024-10-23-11-52-30.jpg" alt="Image 58" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/D7GbY8f/photo-22-2024-10-23-11-51-38.jpg" alt="Image 59" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/c67kgkx/photo-22-2024-10-23-11-52-15.jpg" alt="Image 60" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/MCpyBrv/photo-22-2024-10-23-11-52-30.jpg" alt="Image 61" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/HD57mqY/photo-23-2024-10-23-11-51-38.jpg" alt="Image 62" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/Nxzm4Yx/photo-23-2024-10-23-11-52-15.jpg" alt="Image 63" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/mcc9Jch/photo-23-2024-10-23-11-52-30.jpg" alt="Image 64" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/4jrXQNZ/photo-24-2024-10-23-11-51-38.jpg" alt="Image 65" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/YT4c4nJ/photo-24-2024-10-23-11-52-15.jpg" alt="Image 66" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/xqDhW0z/photo-24-2024-10-23-11-52-30.jpg" alt="Image 67" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/dct9kbk/photo-25-2024-10-23-11-51-38.jpg" alt="Image 68" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/g6pRYnX/photo-25-2024-10-23-11-52-15.jpg" alt="Image 69" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/8x69dFT/photo-25-2024-10-23-11-52-30.jpg" alt="Image 70" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/TKZmfVX/photo-26-2024-10-23-11-51-38.jpg" alt="Image 71" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/Dfkft9Q/photo-26-2024-10-23-11-52-15.jpg" alt="Image 72" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/WKQv69w/photo-26-2024-10-23-11-52-30.jpg" alt="Image 73" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/BjBdytt/photo-27-2024-10-23-11-22-02.jpg" alt="Image 74" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/M9kGpQd/photo-27-2024-10-23-11-52-15.jpg" alt="Image 75" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/Zdz7ccR/photo-27-2024-10-23-11-52-30.jpg" alt="Image 76" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/ZcjJLfm/photo-28-2024-10-23-11-51-38.jpg" alt="Image 77" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/yqBdFZ2/photo-28-2024-10-23-11-52-15.jpg" alt="Image 78" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/QYvQ7Lg/photo-28-2024-10-23-11-52-30.jpg" alt="Image 79" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/cFspDv7/photo-29-2024-10-23-11-22-02.jpg" alt="Image 80" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/23tXYk1/photo-29-2024-10-23-11-52-15.jpg" alt="Image 81" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/ZxcVz07/photo-29-2024-10-23-11-52-30.jpg" alt="Image 82" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/JvZS9tb/photo-30-2024-10-23-11-51-38.jpg" alt="Image 83" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/CzTtsR9/photo-30-2024-10-23-11-52-15.jpg" alt="Image 84" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/vwVW6Nd/photo-30-2024-10-23-11-52-30.jpg" alt="Image 85" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/JkYFptc/photo-31-2024-10-23-11-22-02.jpg" alt="Image 86" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/kMBRC35/photo-31-2024-10-23-11-52-15.jpg" alt="Image 87" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/kmfqKf4/photo-31-2024-10-23-11-52-30.jpg" alt="Image 88" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/1ffHXMs/photo-32-2024-10-23-11-51-38.jpg" alt="Image 89" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/fdc02bY/photo-32-2024-10-23-11-52-15.jpg" alt="Image 90" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/3c4BNyW/photo-32-2024-10-23-11-52-30.jpg" alt="Image 91" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/h2HCB93/photo-33-2024-10-23-11-52-15.jpg" alt="Image 92" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/c10kMTh/photo-33-2024-10-23-11-52-30.jpg" alt="Image 93" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/bNyRhZw/photo-34-2024-10-23-11-51-38.jpg" alt="Image 95" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/ydrVJgN/photo-34-2024-10-23-11-52-15.jpg" alt="Image 96" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/XxZDK60/photo-34-2024-10-23-11-52-30.jpg" alt="Image 97" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/zFh3ctK/photo-35-2024-10-23-11-52-15.jpg" alt="Image 99" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/g9zB1yT/photo-35-2024-10-23-11-52-30.jpg" alt="Image 100" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/CvJ5dtT/photo-36-2024-10-23-11-51-38.jpg" alt="Image 101" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/4jK2HKv/photo-36-2024-10-23-11-52-15.jpg" alt="Image 102" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/dfQ7HVP/photo-36-2024-10-23-11-52-30.jpg" alt="Image 103" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/z5zvrFM/photo-37-2024-10-23-11-22-02.jpg" alt="Image 104" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/7JS9cvr/photo-37-2024-10-23-11-52-15.jpg" alt="Image 105" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/MBp1GHC/photo-37-2024-10-23-11-52-30.jpg" alt="Image 106" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/1KSwRvG/photo-38-2024-10-23-11-51-38.jpg" alt="Image 107" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/8xvq1R8/photo-38-2024-10-23-11-52-15.jpg" alt="Image 108" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/B3G330L/photo-38-2024-10-23-11-52-30.jpg" alt="Image 109" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/R2gpfZK/photo-39-2024-10-23-11-22-02.jpg" alt="Image 110" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/R2mJy7H/photo-39-2024-10-23-11-52-15.jpg" alt="Image 111" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/1003y4f/photo-39-2024-10-23-11-52-30.jpg" alt="Image 112" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/6gvCGfr/photo-40-2024-10-23-11-22-02.jpg" alt="Image 113" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/dmBbHSn/photo-40-2024-10-23-11-52-15.jpg" alt="Image 114" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/VNb6F5w/photo-40-2024-10-23-11-52-30.jpg" alt="Image 115" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/pRnwn46/photo-41-2024-10-23-11-51-38.jpg" alt="Image 116" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/m5j7Jqh/photo-41-2024-10-23-11-52-15.jpg" alt="Image 117" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/qyvrhgn/photo-41-2024-10-23-11-52-30.jpg" alt="Image 118" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/Nm9Lv4q/photo-42-2024-10-23-11-52-15.jpg" alt="Image 119" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/XDHQbfZ/photo-42-2024-10-23-11-52-30.jpg" alt="Image 120" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/rx9jSZQ/photo-43-2024-10-23-11-22-02.jpg" alt="Image 121" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/kD7bhqN/photo-43-2024-10-23-11-52-15.jpg" alt="Image 122" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/0CMXh01/photo-43-2024-10-23-11-52-30.jpg" alt="Image 123" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/3vkh61X/photo-44-2024-10-23-11-51-38.jpg" alt="Image 124" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/7bydhNh/photo-44-2024-10-23-11-52-15.jpg" alt="Image 125" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/Tw21fCf/photo-45-2024-10-23-11-22-02.jpg" alt="Image 126" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/MZ1MsXK/photo-45-2024-10-23-11-52-15.jpg" alt="Image 127" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/0qZ2gsz/photo-46-2024-10-23-11-22-02.jpg" alt="Image 128" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/VSt9JFV/photo-46-2024-10-23-11-52-15.jpg" alt="Image 129" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/fDYSpwj/photo-47-2024-10-23-11-51-38.jpg" alt="Image 130" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/HXSWP3b/photo-47-2024-10-23-11-52-15.jpg" alt="Image 131" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/D1Shf39/photo-48-2024-10-23-11-22-02.jpg" alt="Image 132" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/xJyRkGQ/photo-49-2024-10-23-11-51-38.jpg" alt="Image 133" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/3kysnCy/photo-49-2024-10-23-11-52-15.jpg" alt="Image 134" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/qsbySLD/photo-50-2024-10-23-11-51-38.jpg" alt="Image 135" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/KVgNP74/photo-50-2024-10-23-11-52-15.jpg" alt="Image 136" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/PF1Zsjh/photo-51-2024-10-23-11-51-38.jpg" alt="Image 137" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/CwNr7Nc/photo-52-2024-10-23-11-22-02.jpg" alt="Image 138" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/dfQ7HVP/photo-36-2024-10-23-11-52-30.jpg" alt="Image 139" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/QX2mDJy/photo-53-2024-10-23-11-22-02.jpg" alt="Image 140" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/BZJ6yxQ/photo-54-2024-10-23-11-51-38.jpg" alt="Image 141" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/gPj9DgB/photo-93-2024-10-23-11-52-15.jpg" alt="Image 142" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/B6ZddPC/photo-94-2024-10-23-11-51-38.jpg" alt="Image 143" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/hdQf9sT/photo-94-2024-10-23-11-52-15.jpg" alt="Image 144" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/kcRrfp4/photo-95-2024-10-23-11-51-38.jpg" alt="Image 145" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/FnL87cT/photo-95-2024-10-23-11-52-15.jpg" alt="Image 146" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/FKs7rYX/photo-96-2024-10-23-11-51-38.jpg" alt="Image 147" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/nRdVX4Z/photo-96-2024-10-23-11-52-15.jpg" alt="Image 148" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/WxLNfwB/photo-97-2024-10-23-11-22-02.jpg" alt="Image 149" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/KxBmrT4/photo-97-2024-10-23-11-52-15.jpg" alt="Image 150" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/DYg1S19/photo-98-2024-10-23-11-22-02.jpg" alt="Image 151" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/nzJgzTt/photo-98-2024-10-23-11-52-15.jpg" alt="Image 152" style="width:150px; height:auto; margin:10px;">
</div>
    
        

 

    <div id="asian-girls" class="image-content" style="display:none;">
        <p>Bạn chưa đủ điều kiện để truy cập vào các dịch vụ đặc biệt của hệ thống 💎</p>
         <img src="https://i.ibb.co/7XC0YLX/photo-2022-10-08-18-52-42.jpg" alt="Image 1" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/VNmggsG/photo-2022-10-08-18-52-46.jpg" alt="Image 2" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/6nkzCXY/photo-2022-10-08-18-52-45.jpg" alt="Image 3" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/GRjCgrS/photo-2022-10-08-18-52-44.jpg" alt="Image 4" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/2cqRD5T/photo-2022-12-04-21-24-39.jpg" alt="Image 5" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/WFByYt6/photo-2024-09-14-08-14-57.jpg" alt="Image 6" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/93SzQH6/photo-2024-09-14-08-14-58.jpg" alt="Image 7" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/p0CNGXD/photo-2024-01-07-11-24-49.jpg" alt="Image 8" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/LgTdBZH/photo-2024-01-07-11-24-44.jpg" alt="Image 9" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/k2qxM1S/photo-2023-01-22-19-34-23.jpg" alt="Image 10" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/ZmNNVSh/photo-2024-05-20-13-35-57.jpg" alt="Image 11" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/pztt9WL/photo-2024-05-20-13-36-00.jpg" alt="Image 12" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Wchf4tQ/photo-2024-05-20-13-35-51-2.jpg" alt="Image 13" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/PNJvt23/photo-2024-05-20-13-35-51.jpg" alt="Image 14" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/QNYd9jd/photo-2024-05-20-13-35-52-4.jpg" alt="Image 15" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/kG0QcX6/photo-2024-05-20-13-35-52-3.jpg" alt="Image 16" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/KFwDh5r/photo-2024-05-20-13-35-52-2.jpg" alt="Image 17" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/PNhKXnR/photo-2024-05-20-13-35-52.jpg" alt="Image 18" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/THMH9S1/photo-2024-05-20-13-35-53-2.jpg" alt="Image 19" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/ws0x3B1/photo-2024-05-20-13-35-54.jpg" alt="Image 20" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/9YZ4fFg/photo-2024-05-20-13-35-53.jpg" alt="Image 21" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/X4ncVn6/photo-2022-09-09-02-13-18.jpg" alt="Image 22" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/vDgkpgY/photo-2022-09-09-02-13-19.jpg" alt="Image 23" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/HCfgZk3/photo-2022-09-09-02-13-21.jpg" alt="Image 24" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/PNNwByZ/photo-2024-09-19-10-00-00-3.jpg" alt="Image 25" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/fQZjGx5/photo-2024-09-19-10-00-00-2.jpg" alt="Image 26" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/R45Jy8s/photo-2024-09-19-10-00-00.jpg" alt="Image 27" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/1v3qtV2/photo-2024-09-25-14-53-12.jpg" alt="Image 28" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Jy3kczR/photo-2024-09-30-17-54-39.jpg" alt="Image 29" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/ZgkV74L/photo-2024-09-30-17-54-53.jpg" alt="Image 30" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/MZQxzqZ/photo-2024-09-30-20-00-19.jpg" alt="Image 31" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/0fPpMbG/photo-2024-09-30-21-32-50.jpg" alt="Image 32" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/kSGR6DM/photo-2024-08-22-12-55-44.jpg" alt="Image 33" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/wYfmJRs/photo-2024-10-09-19-17-54.jpg" alt="Image 34" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/VTspds3/photo-2024-09-10-09-38-31-2.jpg" alt="Image 35" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/GCVQpvJ/photo-2024-09-10-09-38-31.jpg" alt="Image 36" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/0X2x7np/photo-2024-10-05-02-07-14-3.jpg" alt="Image 37" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/T4VKmj7/photo-2024-10-05-02-07-14-2.jpg" alt="Image 38" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/TRvVDk3/photo-2024-10-05-02-07-14.jpg" alt="Image 39" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/yVfrLKf/photo-2024-10-04-16-31-08.jpg" alt="Image 40" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/QN9s3Yj/photo-2024-10-04-16-31-07-2.jpg" alt="Image 41" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Ssg2SmY/photo-2024-10-04-16-31-07.jpg" alt="Image 42" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/c1h759H/photo-2024-10-14-15-40-01.jpg" alt="Image 43" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/8YZmk40/photo-2024-10-14-15-40-02-2.jpg" alt="Image 44" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/GMKSpv2/photo-2024-10-14-15-40-02.jpg" alt="Image 45" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/ZKfvZyC/photo-2024-10-14-22-30-50.jpg" alt="Image 46" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/gJXjD5h/photo-2024-10-15-22-09-06-2.jpg" alt="Image 47" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/41ZqJ1Y/photo-2024-10-15-22-09-06.jpg" alt="Image 48" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/r0zhH0q/photo-2024-10-15-22-09-07.jpg" alt="Image 49" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Zg0yGYS/photo-2024-10-15-22-09-08.jpg" alt="Image 50" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/VM0SphT/photo-2024-10-15-22-09-14-2.jpg" alt="Image 51" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/QvV5f3x/photo-2024-10-15-22-09-14.jpg" alt="Image 52" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/q0cnWqD/photo-2024-10-15-22-09-13.jpg" alt="Image 53" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/rk6H8j5/photo-2024-10-15-22-09-20-4.jpg" alt="Image 54" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/41xZ31s/photo-2024-10-15-22-09-19.jpg" alt="Image 55" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/HH5G3Z0/photo-2024-10-15-22-09-20-3.jpg" alt="Image 56" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/hDgChpp/photo-2024-10-15-22-09-20-2.jpg" alt="Image 57" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/rk6H8j5/photo-2024-10-15-22-09-20-4.jpg" alt="Image 58" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/k4zDTtn/photo-2024-10-16-15-57-16.jpg" alt="Image 59" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/BLw37s5/photo-2024-10-18-12-22-35.jpg" alt="Image 60" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/9njHWkz/photo-2024-10-18-12-22-36.jpg" alt="Image 61" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Nyd2M6D/photo-2024-10-19-08-01-33.jpg" alt="Image 62" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/LvQwq3x/photo-2024-10-19-08-07-57-3.jpg" alt="Image 63" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/C77wpYR/photo-2024-10-19-08-07-57-2.jpg" alt="Image 64" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Tm0cLW6/photo-2024-10-19-08-07-57.jpg" alt="Image 65" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/C0cXQ0d/photo-2024-10-19-08-07-58.jpg" alt="Image 66" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/y6wQvWL/photo-2024-10-19-08-07-59-3.jpg" alt="Image 67" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Zg4zGHJ/photo-2024-10-19-08-07-59-2.jpg" alt="Image 68" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/N3pmwSy/photo-2024-10-19-08-07-59.jpg" alt="Image 69" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/hF9cTxf/photo-2024-10-19-08-08-00-4.jpg" alt="Image 70" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/C2VgrXG/photo-2024-10-19-08-08-00-3.jpg" alt="Image 71" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/SyGRfLb/photo-2024-10-19-08-08-00-2.jpg" alt="Image 72" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/QYmhDnQ/photo-2024-10-19-08-08-00.jpg" alt="Image 73" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/wYqn78P/photo-2024-10-26-12-29-12.jpg" alt="Image 74" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/xfsGJZD/photo-2024-10-19-08-08-01.jpg" alt="Image 75" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/ZXpRPsX/photo-2024-10-19-08-08-02-2.jpg" alt="Image 76" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/dGRfPDb/photo-2024-10-19-08-08-02.jpg" alt="Image 77" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/fDJwBPT/photo-2024-10-19-08-08-10.jpg" alt="Image 78" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/7bNVGFf/photo-2024-10-25-14-54-29.jpg" alt="Image 79" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/hBnHrN0/photo-2024-10-26-08-13-47.jpg" alt="Image 80" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Nrv4YvW/photo-2024-10-26-08-13-54.jpg" alt="Image 81" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/0ZhVvgP/photo-2024-10-26-08-14-01.jpg" alt="Image 82" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/hsbv23R/photo-2024-10-26-08-14-11.jpg" alt="Image 83" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/Ky50qmW/photo-2024-08-20-07-44-24.jpg" alt="Image 84" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/C16KWqn/photo-2024-08-20-07-44-25.jpg" alt="Image 85" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/JBk4wtN/photo-2024-08-20-07-44-23.jpg" alt="Image 86" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/1bRgtPn/photo-2024-08-19-18-39-29.jpg" alt="Image 87" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/7WW4LrB/photo-2024-08-19-18-39-28-2.jpg" alt="Image 88" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/SN2bcJj/photo-2024-08-19-18-39-28.jpg" alt="Image 89" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/ZYK7Fcj/photo-2024-08-19-06-47-25.jpg" alt="Image 90" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/sFV03cm/photo-2024-08-19-06-47-23-2.jpg" alt="Image 91" style="width:150px; height:auto; margin:10px;">
<img src="https://i.ibb.co/ccrmQ47/photo-2024-08-19-06-47-23.jpg" alt="Image 92" style="width:150px; height:auto; margin:10px;">
</div>

    <div id="diary" class="image-content" style="display:none;">
        <p>Check hàng</p>
        <img src="https://i.ibb.co/0mbvHY4/reup-trieu-uyen-cuc-pham-sieu-non-to-nong-bong-ngot-ngao-dang-yeu-2961977-original.jpg" alt="Check Những siêu phẩm mất ăn mất ngủ" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/TWvnGsX/review-of-tokuda272-for-reup-hang-vip-sumy-tran-co-the-cuc-pham-nhu-vuu-vat-tay-ha-3215824-original.jpg" alt="Nhật Ký Mây Mưa 1" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/54rhsPC/review-of-tam-tung-for-reup-be-ana-pga-chuan-mat-xinh-body-dep-vu-to-dam-tiep-cac-boss-3238838-original.jpg" alt="Nhật Ký Mây Mưa 2" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/8r6cpWx/review-of-duc-toan-for-reup-be-ana-pga-chuan-mat-xinh-body-dep-vu-to-dam-tiep-cac-boss-3255192-original.jpg" alt="Nhật Ký Mây Mưa 3" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/zQZWmck/review-of-doi-bo-for-re-up-ngoc-tuyen-de-nhat-my-nhan-la-day-dep-ngat-ngay-3249052-original.jpg" alt="Nhật Ký Mây Mưa 4" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/ssZkzn3/review-of-doi-bo-for-re-up-ngoc-tuyen-de-nhat-my-nhan-la-day-dep-ngat-ngay-3249023-original.jpg" alt="Nhật Ký Mây Mưa 5" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/1fGQ4Y6/review-of-hai-truong-for-hot-girl-linh-dan-nang-tho-xinh-dep-dang-chuan-nhu-model-3215399-original.jpg" alt="Nhật Ký Mây Mưa 6" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/376ShPb/review-of-hoang-hung-for-hot-girl-linh-dan-nang-tho-xinh-dep-dang-chuan-nhu-model-3216337-original.jpg" alt="Nhật Ký Mây Mưa 7" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/JRnGGV4/review-of-hoang-hung-for-hot-girl-linh-dan-nang-tho-xinh-dep-dang-chuan-nhu-model-3216314-original.jpg" alt="Nhật Ký Mây Mưa 8" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/Mh7bym6/review-of-hoang-hung-for-hot-girl-linh-dan-nang-tho-xinh-dep-dang-chuan-nhu-model-3216312-original.jpg" alt="Nhật Ký Mây Mưa 9" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/PGPSk3m/review-of-tinh-gia-for-hot-girl-linh-dan-nang-tho-xinh-dep-dang-chuan-nhu-model-3223342-original.jpg" alt="Nhật Ký Mây Mưa 10" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/ThCTjf8/review-of-tinh-gia-for-hot-girl-linh-dan-nang-tho-xinh-dep-dang-chuan-nhu-model-3223340-original.jpg" alt="Nhật Ký Mây Mưa 11" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/Y70wmc1/review-of-tinh-gia-for-hot-girl-linh-dan-nang-tho-xinh-dep-dang-chuan-nhu-model-3223337-original.jpg" alt="Nhật Ký Mây Mưa 12" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/tD9p59f/review-of-hung-phi-for-hot-girl-linh-dan-nang-tho-xinh-dep-dang-chuan-nhu-model-3258843-original.jpg" alt="Nhật Ký Mây Mưa 13" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/dBv8yd2/photo-13-2024-10-23-11-22-02.jpg" alt="Nhật Ký Mây Mưa 1" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/0sYx3Dn/photo-14-2024-10-23-11-52-30.jpg" alt="Nhật Ký Mây Mưa 2" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/D7GbY8f/photo-22-2024-10-23-11-51-38.jpg" alt="Nhật Ký Mây Mưa 3" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/h2HCB93/photo-33-2024-10-23-11-52-15.jpg" alt="Nhật Ký Mây Mưa 4" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/7bydhNh/photo-44-2024-10-23-11-52-15.jpg" alt="Nhật Ký Mây Mưa 5" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/2cDrw6c/photo-76-2024-10-23-11-51-38.jpg" alt="Nhật Ký Mây Mưa 6" style="width:150px; height:auto; margin:10px;">
        <img src="https://i.ibb.co/N2SKVSV/photo-99-2024-10-23-11-51-38.jpg" alt="Nhật Ký Mây Mưa 7" style="width:150px; height:auto; margin:10px;">
        
    </div>

    <div id="stolen-photos" class="image-content" style="display:none;">
        <p>Bạn chưa đủ điều kiện để truy cập vào các dịch vụ đặc biệt của hệ thống 💎</p>
    </div>

</div>
<style>
    
 .introduce {
    font-size: 16px;
    color: #ffffff !important; /* Màu mặc định cho phần chữ "Hoạt động:" */
}

</style>


<style>
    .image-btn {
        font-size: 13px; /* Kích thước chữ */
        padding: 6px 12px; /* Khoảng cách trong nút */
        background-color: #000000; /* Màu nền của nút (hồng đậm) */
        color: #ffffff; /* Màu chữ */
        border: 1px solid #ffffff; /* Viền cam nhạt */
        font-weight: 750; /* Chữ đậm nhưng nhẹ hơn */
        border-radius: 5px; /* Bo góc cho nút */
        margin: 2px 1px; /* Khoảng cách giữa các nút */
        cursor: pointer; /* Hiển thị con trỏ chuột khi hover */
        transition: background-color 0.3s ease, transform 0.3s ease; /* Hiệu ứng chuyển động khi hover */
    }

    .image-btn:hover {
        background-color: #ffffff; /* Màu nền khi hover */
    transform: scale(1.05); /* Phóng to nhẹ khi hover */
}
        
    
</style>

<!-- JavaScript để hiển thị nội dung -->
<script>
    function showContent(category) {
        // Ẩn tất cả các phần nội dung
        const contents = document.querySelectorAll('.image-content');
        contents.forEach(content => {
            content.style.display = 'none';
        });
        
        // Hiển thị phần nội dung tương ứng
        const selectedContent = document.getElementById(category);
        selectedContent.style.display = 'block';
    }
</script>
</style>
</head>
<body>



</script>
    <script>
        function redirectTo(url) {
            window.location.href = url;
        }
    </script>
</body>
</html>

<!-- Gái gọi gần tôi -->
<div id="my-region-section" class="content">
    <h2>Đề xuất gần bạn</h2>
    <div class="region-list">
        <div class="region-btn" onclick="showDetails('JULY')">
            <i class="fas fa-female"></i> July 
        </div>
        <div class="region-btn" onclick="showDetails('YUMI')">
            <i class="fas fa-female"></i> Yumi 
             </div>
        <div class="region-btn" onclick="showDetails('HaHuyen')">
            <i class="fas fa-female"></i> Hà Huyền 
        </div>
        <div class="region-btn" onclick="showDetails('AMY')">
            <i class="fas fa-female"></i> Amy 
        </div>
         <div class="region-btn" onclick="showDetails('HaMy')">
          <i class="fas fa-female"></i> Hà My 
        </div>
        <div class="region-btn" onclick="showDetails('MINA')">
            <i class="fas fa-female"></i> Mina 
        </div>
        <div class="region-btn" onclick="showDetails('LUCY')">
            <i class="fas fa-female"></i> Lucy  
        </div>
        <div class="region-btn" onclick="showDetails('SHISHI')">
            <i class="fas fa-female"></i> Shishi 
            </div>
      <div class="region-btn" onclick="showDetails('QuynhAnh')">
          <i class="fas fa-female"></i> Q.Anh
        </div>
        <div class="region-btn" onclick="showDetails('Chang')">
            <i class="fas fa-female"></i> Chang 
        </div>
    </div>
</div>


<div id="bookingInfoModal" class="modal">
    <div class="modal-content">
        <h4>Đặt Lịch</h4>
        <label for="timeInput">Thời gian:</label>
        <input type="datetime-local" id="timeInput">
        
        <label for="locationInput">Địa điểm:</label>
        <input type="text" id="locationInput" placeholder="Nhập địa điểm">
        
        <label for="servicePackage">Gói dịch vụ:</label>
        <select id="servicePackage">
            <option value="basic">Gói Thường </option>
            <option value="vip">Gói VIP</option>
            <option value="luxury">Gói Luxury</option>
            <option value="vip-tour">Gói VIP Tour</option>
        </select>
          <div id="character-status">
        <p id="status">Trạng thái: Đang hoạt động</p>
    </div>
           
        <button onclick="confirmBookingInfo()">Xác nhận</button>
    </div>
</div>

<!-- Modal nhập mã đặt lịch -->
<div id="bookingCodeModal" class="modal" style="display: none;">
    <div class="modal-content">
        <h4>Nhập Mã Đặt Lịch</h4>
        
        <p>Mã xác nhận đặt lịch của anh là:</p>
        <input type="text" id="bookingCodeInput" placeholder="Nhập mã đặt lịch">
        
        <button onclick="submitBookingCode()">Xác nhận</button>
        <button onclick="closeModal('bookingCodeModal')">Đóng</button>
        
        <p>
            <a href="https://t.me/thuongvy8386aa" class="button-link">Lần đầu sử dụng dịch vụ bấm tại đây</a>
        </p>
    </div>
</div>


 <!-- Thông báo thành công -->
 <div id="successNotification" class="success-notification">
    <img src="https://i.ibb.co/xF4Rq7n/Pngtree-green-check-mark-vector-7885995-removebg-preview.png" alt="Tích xanh">
    Đặt lịch thành công!
</div>

<div id="errorNotification" class="success-notification" style="display: none;">
    <p>Mã đặt lịch không chính xác. Vui lòng thử lại.</p>
    <p>Liên hệ hỗ trợ tại: <a href="https://t.me/yennhi1999aa">đây</a></p>
    <p><a href="https://t.me/huongvy8386aa">Trợ giúp trực tuyến</a></p>
</div>


<script>
const correctBookingCode = "88889999";
const errorRedirectUrl = "https://example.com/error"; // Thay đổi đường dẫn theo ý bạn
// Mở modal nhập thông tin đặt lịch
function openBookingModal() {
    document.getElementById("bookingInfoModal").style.display = "flex";
}

// Đóng modal
function closeModal(modalId) {
    document.getElementById(modalId).style.display = "none";
}

// Xác nhận thông tin đặt lịch và chuyển qua nhập mã đặt lịch
function confirmBookingInfo() {
    const time = document.getElementById("timeInput").value;
    const location = document.getElementById("locationInput").value;
    const package = document.getElementById("servicePackage").value;

    if (time && location && package) {
        closeModal("bookingInfoModal");
        document.getElementById("bookingCodeModal").style.display = "flex";
    } else {
        alert("Vui lòng nhập đầy đủ thông tin.");
    }
}

// Xác nhận mã đặt lịch
function submitBookingCode() {
    const bookingCode = document.getElementById("bookingCodeInput").value;

    if (bookingCode === correctBookingCode) {
        closeModal("bookingCodeModal");
        showSuccessNotification();
    } else {
        alert("Mã đặt lịch không chính xác. Vui lòng thử lại.");
    }
}

// Hiển thị thông báo thành công
function showSuccessNotification() {
    const notification = document.getElementById("successNotification");
    notification.style.display = "block";
    setTimeout(() => {
        notification.style.display = "none";
    }, 3000);
}
// Hiển thị thông báo lỗi
function showErrorNotification() {
    const errorNotification = document.getElementById("errorNotification");
    errorNotification.style.display = "block";
    setTimeout(() => {
        errorNotification.style.display = "none";
    }, 8000); // Hiển thị trong 8 giây
}
// Đóng thông báo
function closeNotification() {
    document.getElementById("successNotification").style.display = "none";
}

// Ví dụ mở modal đặt lịch
// openBookingModal();
</script>
</body>
</html>
</script>

<style>
     #bookingInfoModal .modal-content label {
        font-family: 'Poppins", sans-serif; /* Thay đổi thành font khác nếu cần */
        font-size: 15px;
        color: #000000; /* Màu chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
    }
    /*  
    CSS cơ bản cho modal và thông báo thành công */
    .modal {
        display: none;
        position: fixed;
        top: 0; left: 0; right: 0; bottom: 0;
        background: rgba(0, 0, 0, 0.5);
        justify-content: center;
        align-items: center;
    }
    .modal-content {
        background: linear-gradient(135deg, #ffb3c6, #ff6ec7); /* Nền hồng nhạt */
        padding: 20px;
        border-radius: 10px;
        width: 250px; /* Điều chỉnh chiều rộng phù hợp */
        color: #000000; /* Màu chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
    border: 2px solid #fff5f5; /* Viền vàng */
        display: flex;
        flex-direction: column;
        gap: 15px;
        font-weight: bold;
        transition: background-color 0.3s, transform 0.3s, box-shadow 0.3s;
    margin-top:-30px;
    }
       
    
    .success-notification {
        display: none;
        position: fixed;
        width: 250px;
        top: 20px;
        right: 20px;
        font-weight: 700; /* Chữ đậm hơn */
        background-color: #000000;
        color: rgb(255, 255, 255);
        padding: 15px;
        border-radius: 10px;
        border: 2px solid #ffffff; /* Viền trắng */
        font-weight: bold; /* Chữ đậm */
    top: 50%; /* Vị trí giữa theo chiều dọc */
    left: 50%; /* Vị trí giữa theo chiều ngang */
    transform: translate(-50%, -50%); /* Căn chỉnh giữa hoàn toàn */
    }
    .success-notification.show {
        display: block;
    }
    .success-notification img {
            width: 20px; /* Kích thước logo tích xanh */
            height: 20px;
            margin-right: 10px; /* Khoảng cách giữa logo và văn bản */
        }
    
</style>  
  
<!-- Thông tin chi tiết cho từng bé -->
        <div id="details-container">
            <!-- Chi tiết JULY -->
            <div id="detail-JULY" class="detail-info">
              <h3>JULY</h3>
              <div class="button-container">
                  <button class="info-button" onclick="toggleContent('JULY', 'info')">
                      <i class="fas fa-info-circle"></i> Thông tin 
                  </button>
                  <button class="info-button" onclick="toggleContent('JULY', 'images')">
                      <i class="fas fa-images"></i> Hình ảnh
                  </button>
                    <button onclick="openBookingModal('JULY')">Đặt lịch</button>
                  
                </button>
              </div>
          
              <!-- Thông tin chi tiết -->
              <div id="info-JULY" style="display: none">
                  <h4>Thông tin</h4>
                  <div class="info-content">
                      <img src="https://ibb.co/s56HByh"><img src="https://i.ibb.co/s56HByh/photo-17-2024-09-20-08-41-30.jpg" alt="JULY Image" class="info-image" style="height: 250px;">
                      <div class="info-text">
                        <p><i class="fas fa-money-bill-wave"></i> <strong></strong></p>
                        <div id="contact-info" class="hidden-info">
                          <p><i class="fas fa-phone"></i> <strong></strong></p>
                            <div class="location-info">
                             
                          </div>
                            <style>
                              /* styles.css */
                              .location-info {
                                  font-size: 17px;
                                  color: #00ff00; /* Màu xanh lá */
                                  font-weight: bold;
                              }
                              .info-image { 
                                  height: 250px; 
                              }
                              .button-container, .detail-info { 
                                  text-align: center; 
                              }
                                .active-status {
        font-weight: bold;
        color: #00ff22;  /* Màu xanh cho trạng thái hoạt động */
    }
    .active-status.busy {
        color: #dc3545;  /* Màu đỏ cho trạng thái bận */
    }
    .active-status.booked {
        color: #ffc107;  /* Màu vàng cho trạng thái đã được đặt lịch */
    }
    .active-status.idle {
        color: #0088ff;  /* Màu xám cho trạng thái chưa được đặt lịch */
    }
                          </style>
                       <script>
                        // Hàm khởi tạo vị trí
                        function requestLocation() {
                            if (navigator.geolocation) {
                                // Yêu cầu lấy vị trí của người dùng
                                navigator.geolocation.getCurrentPosition(
                                    (position) => {
                                        const latitude = position.coords.latitude;
                                        const longitude = position.coords.longitude;
                    
                                        // Gọi Kakao Maps API để lấy thông tin khu vực từ vĩ độ và kinh độ
                                        fetch(`https://dapi.kakao.com/v2/local/geo/coord2regioncode.json?x=${longitude}&y=${latitude}`, {
                                            method: 'GET',
                                            headers: {
                                                'Authorization': 'KakaoAK 12873a4a25a298774293ab8c899a1432'  // Thay YOUR_KAKAO_API_KEY bằng API Key thực tế của bạn
                                            }
                                        })
                                        .then(response => response.json())
                                        .then(data => {
                                          if (data.documents && data.documents.length > 0) {
                            const region1 = data.documents[0].region_1depth_name;  // Quận hoặc khu vực
                            const region2 = data.documents[0].region_2depth_name;  // Thị trấn hoặc xã
                            const region3 = data.documents[0].region_3depth_name || "Không xác định";  // Khu vực nhỏ hơn
                    
                                                // Hiển thị kết quả
                                                document.getElementById('location-range-JULY').textContent = `Vị trí của bạn: ${region1} - ${region2} - ${region3}`;
                                            } else {
                                                document.getElementById('location-range-JULY').textContent = "Đang xác định";
                                            }
                                        })
                                        .catch(err => {
                                            console.error("Lỗi khi lấy vị trí:", err);
                                            document.getElementById('location-range-JULY').textContent = "Lỗi khi lấy thông tin vị trí.";
                                        });
                                    },
                                    (error) => {
                                        console.error("Lỗi khi lấy vị trí:", error);
                                        alert("Không thể lấy vị trí. Vui lòng kiểm tra cài đặt vị trí của bạn.");
                                    }
                                );
                            } else {
                                alert("Trình duyệt của bạn không hỗ trợ Geolocation.");
                            }
                        }
                    
                        // Gọi hàm yêu cầu vị trí khi trang được tải
                        requestLocation();
                    </script>
                    
                    <!-- HTML phần tử hiển thị vị trí -->
                    <div class="location-info">
                        <span id="location-range-JULY">Đang xác định</span>
                    </div>
                    
                                    </script>
                                
                                </body>
                                </html>
                        </div>
                        <button onclick="showInputBox('JULY', 'phone')">SDT</button>
<button onclick="showInputBox('JULY', 'telegram')">Telegram</button>
                          <p><i class="fas fa-clock"></i> <strong>Thời gian gia nhập:</strong> 29/05/2024 10:30</p>
                          <p><i class="fas fa-user"></i> <strong>Hoạt động:</strong> <span id="active-status-JULY" class="active-status">Đang hoạt động</span></p>                        </p>
                      </div>
                  </div>


                    <h4>Giới thiệu</h4>
                  <p>
                    <p>Em gái nuột nà,đẹp lung linh tuổi Teen</p> 
                        <p>Mặt xinh như tiểu thư , body sịn 100% ko thẩm mỹ</p> 
                            <p>Thơm phưc tự nhiên</p>
                                <p>Phải đích mục sở thị thì mới biết</p>
                                    <p>Đến với bé để cảm nhận cuộc đời nhé !          
                </p>
                <p><i class="fas fa-birthday-cake"></i> <strong>Năm sinh:</strong> 2001</p>
                <p><i class="fas fa-ruler-vertical"></i> <strong>Cao (cm):</strong> 163</p>
                <p><i class="fas fa-weight-hanging"></i> <strong>Nặng (kg):</strong> 49</p>
                <p><i class="fas fa-tape"></i> <strong>Vòng 1 (cm):</strong> 86</p>
                <p><i class="fas fa-tape"></i> <strong>Vòng 2 (cm):</strong> 60</p>
                <p><i class="fas fa-tape"></i> <strong>Vòng 3 (cm):</strong> 91</p>
                <p><i class="fas fa-smile"></i> <strong>Khuôn mặt:</strong> Dịu dàng và quyến rũ</p>
                <p><i class="fas fa-eye"></i> <strong>Nhận dạng:</strong> Thân hình quyến rũ, phong cách trẻ trung, tự tin</p>
                <p><i class="fas fa-clock"></i> <strong>Hoạt động:</strong> Giờ nào cũng làm</p>
            </div>
          
              <div id="review-container-JULY" class="review-section">
                <h4>Đánh giá của bạn cho JULY</h4>
                <div class="stars">
                    <span class="star" onclick="rateStar('JULY', 1)">&#9733;</span>
                    <span class="star" onclick="rateStar('JULY', 2)">&#9733;</span>
                    <span class="star" onclick="rateStar('JULY', 3)">&#9733;</span>
                    <span class="star" onclick="rateStar('JULY', 4)">&#9733;</span>
                    <span class="star" onclick="rateStar('JULY', 5)">&#9733;</span>
                </div>
            </div> 
        </div>         
        <script>
   
            function rateStar(character, star) {
             const result = document.getElementById(`rating-result-${character}`);
         
             if (result) {
                 // Hiển thị thông báo đánh giá
                 result.innerText = `Bạn đã đánh giá ${star} sao cho ${character}!`;
         
                 // Sau 3 giây, hiển thị thông báo cảm ơn và ẩn đi sau đó
                 setTimeout(() => {
                     result.innerText = `Cảm ơn bạn đã đánh giá cho ${character}. Mỗi lượt đánh giá của bạn góp phần thay đổi thứ hạng của cô ấy! Chỉ tính lần đầu trong ngày ❤️`;
         
                     // Ẩn thông báo sau thêm 2 giây nữa
                     setTimeout(() => {
                         result.innerText = ''; // Xóa nội dung để ẩn đi
                         result.style.display = 'none'; // Ẩn phần tử
                     }, 2000);
                 }, 3000);
             } else {
                 console.error("Không tìm thấy phần tử kết quả đánh giá!");
             }
         }
         
         // Tạo phần tử để hiển thị kết quả đánh giá trong HTML (nếu chưa có)
         document.querySelectorAll('.review-section').forEach(section => {
             const character = section.id.split('-')[2]; // Lấy tên nhân vật từ ID
             if (!document.getElementById(`rating-result-${character}`)) {
                 const resultElement = document.createElement('p');
                 resultElement.id = `rating-result-${character}`;
                 section.appendChild(resultElement);
             }
         });
             
         </script>
            <style>
                .review-section {
    margin-top: 20px;
    padding: 10px;
    background-color: #000000; /* Màu nền */
    color: #ffffff;
    border-radius: 5px;
    max-width: 100%; /* Giới hạn chiều rộng */
    overflow: hidden; /* Ngăn nội dung bị tràn ra ngoài */
    box-sizing: border-box; /* Đảm bảo padding không làm thay đổi chiều rộng */
}
                
                .stars {
                    font-size: 12px;
                    color: #ffffff;
                }
                .star {
                    cursor: pointer;
                }
                   
                            

            </style>
            
              
              <!-- Hình ảnh -->
<div id="images-JULY" style="display: none">
  <h4>Hình ảnh</h4>
  <a href="https://ibb.co/6vys84c"><img src="https://i.ibb.co/6vys84c/photo-1-2024-09-20-08-41-30.jpg" alt="Image New 1" style="height: 190px; width: auto;"></a>
  <a href="https://ibb.co/NKn7g62"><img src="https://i.ibb.co/NKn7g62/photo-2-2024-09-20-08-41-30.jpg" alt="Image New 2" style="height: 190px; width: auto;"></a>
  <a href="https://ibb.co/J5GP9FZ"><img src="https://i.ibb.co/J5GP9FZ/photo-4-2024-09-20-08-41-30.jpg" alt="Image New 3" style="height: 190px; width: auto;"></a>
  <a href="https://ibb.co/XSvCbdv"><img src="https://i.ibb.co/XSvCbdv/photo-5-2024-09-20-08-41-30.jpg" alt="Image New 4" style="height: 190px; width: auto;"></a>
  <a href="https://ibb.co/1MVVxSg"><img src="https://i.ibb.co/1MVVxSg/photo-9-2024-09-20-08-41-30.jpg" alt="Image New 5" style="height: 190px; width: auto;"></a>
  <a href="https://ibb.co/d55W38g"><img src="https://i.ibb.co/d55W38g/photo-15-2024-09-20-08-41-30.jpg" alt="Image New 6" style="height: 190px; width: auto;"></a>
  <a href="https://ibb.co/j6x96Wy"><img src="https://i.ibb.co/j6x96Wy/photo-18-2024-09-20-08-41-30.jpg" alt="Image New 8" style="height: 190px; width: auto;"></a>
  <a href="https://ibb.co/jWwdDhF"><img src="https://i.ibb.co/jWwdDhF/427795242-1104148964345239-7093685406088560536-n.jpg" alt="Image New 9" style="height: 190px; width: auto;"></a>
  <a href="https://ibb.co/tCKJvGb"><img src="https://i.ibb.co/tCKJvGb/photo-2024-09-05-04-54-14.jpg" alt="Image New 10" style="height: 190px; width: auto;"></a>
  <a href="https://ibb.co/Pr3HRMn"><img src="https://i.ibb.co/Pr3HRMn/photo-2024-09-05-04-54-15-2.jpg" alt="Image New 11" style="height: 190px; width: auto;"></a>
  <a href="https://ibb.co/b518sDH"><img src="https://i.ibb.co/b518sDH/Untitled-design-14.png" alt="Image New 13" style="height: 190px; width: auto;"></a>
  
</div>
          
              <!-- Số lượt book -->
<div id="bookings-JULY" style="display: none">
    <h4>Đặt lịch</h4>
    <p><i class="fas fa-book"></i> <strong>Hướng dẫn đặt lịch:</strong>
      HÃY LÀ MỘT CHECKER VĂN MINH !</p>
    <p><i class="fas fa-calendar-alt"></i> <strong>Vui lòng đăng nhập để đặt lịch !</strong></p>
</div>
          
              <!-- Giới thiệu -->
              <div id="bio-JULY" style="display: none">
                  <h4>Giới thiệu</h4>
                  <p>
                      Với dịch vụ tận tâm và phong cách chuyên nghiệp, cô ấy luôn làm hài lòng khách hàng.
                  </p>
              </div>
          </div>
          

            <!-- Chi tiết YUMI -->
            <div id="detail-YUMI" class="detail-info">
              <h3>YUMI</h3>
              <div class="button-container">
                  <button class="info-button" onclick="toggleContent('YUMI', 'info')">
                      <i class="fas fa-info-circle"></i> Thông tin
                  </button>
                  <button class="info-button" onclick="toggleContent('YUMI', 'images')">
                      <i class="fas fa-images"></i> Hình ảnh
                  </button>
                <button onclick="openBookingModal('YUMI')">Đặt lịch</button>
                  </button>
              </div>
          
              <!-- Thông tin chi tiết -->
              <div id="info-YUMI" style="display: none">
                  <h4>Thông tin</h4>
                  <div class="info-content">
                    <img src="https://i.ibb.co/SsZ2pgF/g1ixJ3Kw.jpg" alt="Image New" class="info-image" style="height: 250px;">
                      <div class="info-text">
                      
                          <style>
                            /* styles.css */
                            .location-info {
                                font-size: 17px;
                                color: #00ff00; /* Màu xanh lá */
                                font-weight: bold;
                            }
                            .info-button {
    color: #000000; /* Màu chữ vàng */
    padding: 11px 22px;
    border-radius: 20px;
    border: 2px solid #ffffff; /* Viền bạc */
    font-weight: bold;
    display: inline-flex;
    align-items: center;
    cursor: pointer;
    justify-content: center; /* Đảm bảo chữ căn giữa cả theo chiều ngang và dọc */
    text-align: center; /* Căn giữa chữ */
    font-size: 13px;
}
.info-button:hover {
    background-color: #000000; /* Màu nền khi hover */
    color: #ffffff; /* Màu chữ khi hover */
    transform: scale(1.05); /* Hiệu ứng phóng to nhẹ khi hover */
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.8); /* Hiệu ứng đổ bóng đậm */
}
                            .info-image { 
                                height: 250px; 
                            }
                            .button-container, .detail-info { 
                                text-align: center; 
                       
    }
                        </style>
                        
                        <script>
                            // Hàm khởi tạo vị trí
                        function requestLocation() {
                            if (navigator.geolocation) {
                                // Yêu cầu lấy vị trí của người dùng
                                navigator.geolocation.getCurrentPosition(
                                    (position) => {
                                        const latitude = position.coords.latitude;
                                        const longitude = position.coords.longitude;
                    
                                        // Gọi Kakao Maps API để lấy thông tin khu vực từ vĩ độ và kinh độ
                                        fetch(`https://dapi.kakao.com/v2/local/geo/coord2regioncode.json?x=${longitude}&y=${latitude}`, {
                                            method: 'GET',
                                            headers: {
                                                'Authorization': 'KakaoAK 12873a4a25a298774293ab8c899a1432'  // Thay YOUR_KAKAO_API_KEY bằng API Key thực tế của bạn
                                            }
                                        })
                                        .then(response => response.json())
                                        .then(data => {
                                          if (data.documents && data.documents.length > 0) {
                            const region1 = data.documents[0].region_1depth_name;  // Quận hoặc khu vực
                            const region2 = data.documents[0].region_2depth_name;  // Thị trấn hoặc xã
                            const region3 = data.documents[0].region_3depth_name || "Không xác định";  // Khu vực nhỏ hơn
                                                        // Hiển thị thông tin thị trấn - quận - thành phố bằng tiếng Hàn
                                                        document.getElementById('location-range-YUMI').textContent = `${town} (${data.results[0].components.town}) - ${district} (${data.results[0].components.district}) - ${city} (${data.results[0].components.city})`;
                                                    } else {
                                                        document.getElementById('location-range-YUMI').textContent = "Đang xác định";
                                                    }
                                                })
                                                .catch(err => {
                                                    console.error("Error getting location:", err);
                                                    document.getElementById('location-range-YUMI').textContent = "Lỗi khi lấy vị trí.";
                                                });
                                        },
                                        (error) => {
                                            console.error("Geolocation error:", error);
                                            alert("Không thể lấy vị trí. Vui lòng kiểm tra cài đặt vị trí của bạn.");
                                        }
                                    );
                                } else {
                                    alert("Trình duyệt của bạn không hỗ trợ Geolocation.");
                                }
                            }
                        
                            // Gọi hàm yêu cầu vị trí khi trang được tải
                            requestLocation();
                        </script>
                        
                        <!-- HTML phần tử hiển thị vị trí -->
                        <div class="location-info">
                            <span id="location-range-YUMI">Đang xác định</span>
                        </div>
                          <button onclick="showInputBox('YUMI', 'phone')">SDT</button>
                         
                          <button onclick="showInputBox('YUMI', 'telegram')">Telegram</button>
                          <p><i class="fas fa-clock"></i> <strong>Thời gian gia nhập:</strong> 29/08/2024 10:30</p>
                          <p><i class="fas fa-user"></i> <strong>Hoạt động:</strong> <span id="active-status-YUMI" class="active-status">Đang hoạt động</span></p>                        </p>

                        </p>
                      </div>
                  </div>

                              
                    
                      
                  <h4>Giới thiệu</h4>
                  <p>
                    Bé sở hữu thân hình căng mọng,mịn màng ko tì vết</p>
                <p>Gương mặt đậm chất dâm dục của bé sẽ làm các anh cuồng loạn</p>
            <p>Một làn da mượt mà trắng bóc và mịn như em bé</p> 
        <p>Quá nhiều trò chơi khoái cảm khi ở cạnh bé này</p>
    <p>Hàng chuẩn chất lượng cao !
                </p>
                <p><i class="fas fa-birthday-cake"></i> <strong>Năm sinh:</strong> 2001</p>
                <p><i class="fas fa-ruler-vertical"></i> <strong>Cao (cm):</strong> 160</p>
                <p><i class="fas fa-weight-hanging"></i> <strong>Nặng (kg):</strong> 46</p>
                <p><i class="fas fa-tape"></i> <strong>Vòng 1 (cm):</strong> 86</p>
                <p><i class="fas fa-tape"></i> <strong>Vòng 2 (cm):</strong> 58</p>
                <p><i class="fas fa-tape"></i> <strong>Vòng 3 (cm):</strong> 90</p>
                <p><i class="fas fa-smile"></i> <strong>Khuôn mặt:</strong> Baby dễ thương</p>
        <p><i class="fas fa-eye"></i> <strong>Nhận dạng:</strong> Mình dây, phong cách đáng yêu và quyến rũ</p>
                <p><i class="fas fa-clock"></i> <strong>Hoạt động:</strong> 24/24</p>
            </div>
          
              <div id="review-container-YUMI" class="review-section">
                <h4>Đánh giá của bạn cho YUMI</h4>
                <div class="stars">
                    <span class="star" onclick="rateStar('YUMI', 1)">&#9733;</span>
                    <span class="star" onclick="rateStar('YUMI', 2)">&#9733;</span>
                    <span class="star" onclick="rateStar('YUMI', 3)">&#9733;</span>
                    <span class="star" onclick="rateStar('YUMI', 4)">&#9733;</span>
                    <span class="star" onclick="rateStar('YUMI', 5)">&#9733;</span>
                </div>
            </div>
            
            <script>
   
                function rateStar(character, star) {
                 const result = document.getElementById(`rating-result-${character}`);
             
                 if (result) {
                     // Hiển thị thông báo đánh giá
                     result.innerText = `Bạn đã đánh giá ${star} sao cho ${character}!`;
             
                     // Sau 3 giây, hiển thị thông báo cảm ơn và ẩn đi sau đó
                     setTimeout(() => {
                         result.innerText = `Cảm ơn bạn đã đánh giá cho ${character}. Mỗi lượt đánh giá của bạn góp phần thay đổi thứ hạng của cô ấy! Chỉ tính lần đầu trong ngày ❤️`;
             
                         // Ẩn thông báo sau thêm 2 giây nữa
                         setTimeout(() => {
                             result.innerText = ''; // Xóa nội dung để ẩn đi
                             result.style.display = 'none'; // Ẩn phần tử
                         }, 2000);
                     }, 3000);
                 } else {
                     console.error("Không tìm thấy phần tử kết quả đánh giá!");
                 }
             }
             
             // Tạo phần tử để hiển thị kết quả đánh giá trong HTML (nếu chưa có)
             document.querySelectorAll('.review-section').forEach(section => {
                 const character = section.id.split('-')[2]; // Lấy tên nhân vật từ ID
                 if (!document.getElementById(`rating-result-${character}`)) {
                     const resultElement = document.createElement('p');
                     resultElement.id = `rating-result-${character}`;
                     section.appendChild(resultElement);
                 }
             });
                 
             </script>
            
            <style>
                .review-section {
                    margin-top: 20px;
                    padding: 10px;
                    background-color: #000000; /* Màu nền nút cam đậm */
                    color: #ffffff; /* Màu chữ trắng */
                    border-radius: 5px;
                }
                .stars {
                    font-size: 20px;
                    color: #ffcc00;
                }
                .star {
                    cursor: pointer;
                }
            </style>

              <!-- Hình ảnh -->
              <div id="images-YUMI" style="display: none">
                  <h4>Hình ảnh</h4>
<a href="https://ibb.co/nBCy6wt"><img src="https://i.ibb.co/nBCy6wt/442414576-1907317203050273-7272925531125045232-n.jpg" alt="Image 6" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/tMkQrPS"><img src="https://i.ibb.co/tMkQrPS/photo-2024-09-05-04-55-41.jpg" alt="Image 8" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/6RKR3x0"><img src="https://i.ibb.co/6RKR3x0/photo-2024-09-05-04-55-42-2.jpg" alt="Image 9" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/9v5mDwW"><img src="https://i.ibb.co/9v5mDwW/photo-2024-09-05-04-55-42-5.jpg" alt="Image 10" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/jb0L2Dh"><img src="https://i.ibb.co/jb0L2Dh/photo-2024-09-05-04-55-42-6.jpg" alt="Image 11" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/8rrgt7x"><img src="https://i.ibb.co/8rrgt7x/photo-2024-09-05-04-55-42-7.jpg" alt="Image 12" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/Z65Lthb"><img src="https://i.ibb.co/Z65Lthb/photo-2024-09-05-04-55-42-8.jpg" alt="Image 13" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/bg77KGJ"><img src="https://i.ibb.co/bg77KGJ/photo-2024-09-05-04-55-42-9.jpg" alt="Image 14" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/7yndCcr"><img src="https://i.ibb.co/7yndCcr/photo-2024-09-05-04-55-43-2.jpg" alt="Image 15" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/tzrpMXw"><img src="https://i.ibb.co/tzrpMXw/photo-2024-09-05-04-55-43-3.jpg" alt="Image 16" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/y0FbHdL"><img src="https://i.ibb.co/y0FbHdL/photo-2024-09-05-04-55-43-4.jpg" alt="Image 17" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/zx3Y05J"><img src="https://i.ibb.co/zx3Y05J/photo-2024-09-05-04-55-43-5.jpg" alt="Image 18" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/ZNd6qKR"><img src="https://i.ibb.co/ZNd6qKR/photo-2024-09-05-04-55-45-2.jpg" alt="Image 19" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/k8wKwXT"><img src="https://i.ibb.co/k8wKwXT/photo-2024-09-05-04-55-45.jpg" alt="Image 20" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/kJjD5YG"><img src="https://i.ibb.co/kJjD5YG/taoanhdep-lam-net-anh-52903.jpg" alt="Image 22" style="height: 190px; width: auto;"></a>

                  
                </div>
          
              <!-- Số lượt book -->
              <div id="bookings-YUMI" style="display: none">
                  <h4>Đặt lịch</h4>
                  <p><i class="fas fa-book"></i> <strong>Hướng dẫn đặt lịch:</strong>
                    * HÃY LÀ MỘT CHECKER VĂN MINH !</p>
                  <p><i class="fas fa-calendar-alt"></i> <strong>Vui lòng đăng nhập để đặt lịch !</strong></p>
              </div>
          
              <!-- Giới thiệu -->
              <div id="bio-YUMI" style="display: none">
                  <h4>Giới thiệu</h4>
                  <p>
                      Cô ấy luôn biết cách thu hút mọi ánh nhìn.
                  </p>
              </div>
          </div>
          


 <!-- Chi tiết Hà Huyền -->
<div id="detail-HaHuyen" class="detail-info">
  <h3>Hà Huyền</h3>
  <div class="button-container">
      <button class="info-button" onclick="toggleContent('HaHuyen', 'info')">
          <i class="fas fa-info-circle"></i> Thông tin
      </button>
      <button class="info-button" onclick="toggleContent('HaHuyen', 'images')">
          <i class="fas fa-images"></i> Hình ảnh
      </button>
      <button onclick="openBookingModal('HaHuyen')">Đặt lịch</button>
  </div>

  <!-- Thông tin chi tiết -->
  <div id="info-HaHuyen" style="display: none">
      <h4>Thông tin</h4>
      <div class="info-content">
        <img src="https://i.ibb.co/S5cZB7m/419418603-1508797216580744-6598850606428340490-n.jpg" alt="Image 11" class="info-image" style="height: 250px;">
        <div class="info-text">
         
              <style>
                /* styles.css */
                .location-info {
                    font-size: 17px;
                    color: #00ff00; /* Màu xanh lá */
                    font-weight: bold;
                }
                .info-image { 
                    height: 250px; 
                }
                .button-container, .detail-info { 
                    text-align: center; 
                }
                
            </style>
    <script>
       // Hàm khởi tạo vị trí
                        function requestLocation() {
                            if (navigator.geolocation) {
                                // Yêu cầu lấy vị trí của người dùng
                                navigator.geolocation.getCurrentPosition(
                                    (position) => {
                                        const latitude = position.coords.latitude;
                                        const longitude = position.coords.longitude;
                    
                                        // Gọi Kakao Maps API để lấy thông tin khu vực từ vĩ độ và kinh độ
                                        fetch(`https://dapi.kakao.com/v2/local/geo/coord2regioncode.json?x=${longitude}&y=${latitude}`, {
                                            method: 'GET',
                                            headers: {
                                                'Authorization': 'KakaoAK 12873a4a25a298774293ab8c899a1432'  // Thay YOUR_KAKAO_API_KEY bằng API Key thực tế của bạn
                                            }
                                        })
                                        .then(response => response.json())
                                        .then(data => {
                                          if (data.documents && data.documents.length > 0) {
                            const region1 = data.documents[0].region_1depth_name;  // Quận hoặc khu vực
                            const region2 = data.documents[0].region_2depth_name;  // Thị trấn hoặc xã
                            const region3 = data.documents[0].region_3depth_name || "Không xác định";  // Khu vực nhỏ hơn

                                // Hiển thị kết quả
                                document.getElementById('location-range-HAHUYEN').textContent = `Vị trí của bạn: ${region1} - ${region2} - ${region3}`;
                            } else {
                                document.getElementById('location-range-HAHUYEN').textContent = "Đang xác định";
                            }
                        })
                        .catch(err => {
                            console.error("Lỗi khi lấy vị trí:", err);
                            document.getElementById('location-range-HAHUYEN').textContent = "Lỗi khi lấy thông tin vị trí.";
                        });
                    },
                    (error) => {
                        console.error("Lỗi khi lấy vị trí:", error);
                        alert("Không thể lấy vị trí. Vui lòng kiểm tra cài đặt vị trí của bạn.");
                    }
                );
            } else {
                alert("Trình duyệt của bạn không hỗ trợ Geolocation.");
            }
        }

        // Gọi hàm yêu cầu vị trí khi trang được tải
        requestLocation();
    </script>
    <!-- HTML phần tử hiển thị vị trí -->
<div class="location-info">
    <p><i class="fas fa-user"></i> <strong>Hoạt động:</strong> <span id="active-status-Hahuyen" class="active-status">Đang hoạt động</span></p>                        </p>
</div>
              <button onclick="showInputBox('HaHuyen', 'phone')">SDT</button>
              <button onclick="showInputBox('HaHuyen', 'telegram')">Telegram</button>
              <p><i class="fas fa-clock"></i> <strong>Thời gian gia nhập:</strong> 12/07/2024 11:26</p>
          </div>
      </div>

    
        <h4>Giới thiệu</h4>
        <p>
      Gặp em ấy là chỉ cảm thấy yêu thôi</p> 
  <p>Xinh xắn dễ thương không chịu được</p> 
  <p>Em ấy sở hữu một làn da trắng ngần không tỳ vết</p>
  <p>Khuôn mặt xinh đẹp không góc chết</p>
  <p>Ngực to, eo thon thả không mỡ thừa,mông to cong cớn cực dâm</p>
  <p> Người con gái mà ai cũng cần phải gặp một lần
        </p>
      <p><i class="fas fa-birthday-cake"></i> <strong>Năm sinh:</strong> 2003</p>
      <p><i class="fas fa-ruler-vertical"></i> <strong>Cao (cm):</strong> 162</p>
      <p><i class="fas fa-weight-hanging"></i> <strong>Nặng (kg):</strong> 49</p>
      <p><i class="fas fa-tape"></i> <strong>Vòng 1 (cm):</strong> 85</p>
      <p><i class="fas fa-tape"></i> <strong>Vòng 2 (cm):</strong> 62</p>
      <p><i class="fas fa-tape"></i> <strong>Vòng 3 (cm):</strong> 90</p>
      <p><i class="fas fa-smile"></i> <strong>Khuôn mặt:</strong> Dịu dàng, thân thiện và rất dễ gần</p>
      <p><i class="fas fa-eye"></i> <strong>Nhận dạng:</strong> Nét đẹp tự nhiên, thân hình quyến rũ và trẻ trung</p>
      <p><i class="fas fa-clock"></i> <strong>Hoạt động:</strong> Luôn sẵn sàng phục vụ</p>
  </div>

  <div id="review-container-HaHuyen" class="review-section">
      <h4>Đánh giá của bạn cho Hà Huyền</h4>
      <div class="stars">
          <span class="star" onclick="rateStar('HaHuyen', 1)">&#9733;</span>
          <span class="star" onclick="rateStar('HaHuyen', 2)">&#9733;</span>
          <span class="star" onclick="rateStar('HaHuyen', 3)">&#9733;</span>
          <span class="star" onclick="rateStar('HaHuyen', 4)">&#9733;</span>
          <span class="star" onclick="rateStar('HaHuyen', 5)">&#9733;</span>
      </div>
  </div>
  <script>
   
    function rateStar(character, star) {
     const result = document.getElementById(`rating-result-${character}`);
 
     if (result) {
         // Hiển thị thông báo đánh giá
         result.innerText = `Bạn đã đánh giá ${star} sao cho ${character}!`;
 
         // Sau 3 giây, hiển thị thông báo cảm ơn và ẩn đi sau đó
         setTimeout(() => {
             result.innerText = `Cảm ơn bạn đã đánh giá cho ${character}. Mỗi lượt đánh giá của bạn góp phần thay đổi thứ hạng của cô ấy! Chỉ tính lần đầu trong ngày ❤️`;
 
             // Ẩn thông báo sau thêm 2 giây nữa
             setTimeout(() => {
                 result.innerText = ''; // Xóa nội dung để ẩn đi
                 result.style.display = 'none'; // Ẩn phần tử
             }, 2000);
         }, 3000);
     } else {
         console.error("Không tìm thấy phần tử kết quả đánh giá!");
     }
 }
 
 // Tạo phần tử để hiển thị kết quả đánh giá trong HTML (nếu chưa có)
 document.querySelectorAll('.review-section').forEach(section => {
     const character = section.id.split('-')[2]; // Lấy tên nhân vật từ ID
     if (!document.getElementById(`rating-result-${character}`)) {
         const resultElement = document.createElement('p');
         resultElement.id = `rating-result-${character}`;
         section.appendChild(resultElement);
     }
 });
     
 </script>
  <!-- Hình ảnh -->
  <div id="images-HaHuyen" style="display: none">
      <h4>Hình ảnh</h4>
      <a href="https://ibb.co/8X5ZpbB"><img src="https://i.ibb.co/8X5ZpbB/408725612-1489117888548677-7938195270057156128-n.jpg" alt="Image 1" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/8cRzwDV"><img src="https://i.ibb.co/8cRzwDV/383756409-1450607245733075-4818141408238196370-n.jpg" alt="Image 2" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/v3N3FMT"><img src="https://i.ibb.co/v3N3FMT/353017933-1399626904164443-3384725205729918730-n.jpg" alt="Image 3" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/QHWWJTN"><img src="https://i.ibb.co/QHWWJTN/316169388-1274408853352916-7077694155830683169-n.jpg" alt="Image 4" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/qWQyC06"><img src="https://i.ibb.co/qWQyC06/275138413-1100935457366924-6396910769917078980-n.jpg" alt="Image 5" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/4gTJxwt"><img src="https://i.ibb.co/4gTJxwt/292884473-1178618856265250-175000647134861741-n.jpg" alt="Image 6" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/sgzNtNf"><img src="https://i.ibb.co/sgzNtNf/303105942-1215513462575789-707884256299403241-n.jpg" alt="Image 7" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/z2rms6r"><img src="https://i.ibb.co/z2rms6r/395638247-1467304944063305-5512392484449680736-n.jpg" alt="Image 8" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/D879vKQ"><img src="https://i.ibb.co/D879vKQ/405127006-1479894232804376-7434074654868707497-n.jpg" alt="Image 9" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/ZRjvVd4"><img src="https://i.ibb.co/ZRjvVd4/432771239-1544995982960867-630242919755697340-n.jpg" alt="Image 10" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/S5cZB7m"><img src="https://i.ibb.co/S5cZB7m/419418603-1508797216580744-6598850606428340490-n.jpg" alt="Image 11" style="height: 190px; width: auto;"></a>

      
  </div>

  <!-- Số lượt book -->
  <div id="bookings-HaHuyen" style="display: none">
      <h4>Đặt lịch</h4>
      <p><i class="fas fa-calendar-alt"></i> <strong>Vui lòng đăng nhập để đặt lịch</strong></p>
  </div>

  <!-- Giới thiệu -->
  <div id="bio-HaHuyen" style="display: none">
      <h4>Giới thiệu</h4>
      <p>
          Hà Huyền luôn tạo ra những trải nghiệm đáng nhớ với sự chuyên nghiệp và tận tâm. Cô ấy là một trong những gương mặt nổi bật tại Diamond Club.
      </p>
  </div>
</div>



          
        
        
    <div id="detail-AMY" class="detail-info">
        <h3>AMY</h3>
        <div class="button-container">
            <button class="info-button" onclick="toggleContent('AMY', 'info')">
                <i class="fas fa-info-circle"></i> Thông tin
            </button>
            <button class="info-button" onclick="toggleContent('AMY', 'images')">
                <i class="fas fa-images"></i> Hình ảnh
            </button>
             <button onclick="openBookingModal('AMY')">Đặt lịch</button>
        </button>
    </div>
              
                   <!-- Thông tin chi tiết -->
        <div id="info-AMY" style="display: none;">
            <h4>Thông tin</h4>
            <div class="info-content">
                <img src="https://i.ibb.co/CWFhJKn/photo-11-2024-09-20-09-04-21.jpg" alt="Image New 32" class="info-image" style="height: 250px;">
                <div class="info-text">
               
                    <style>
                      /* styles.css */
                      .location-info {
                          font-size: 17px;
                          color: #00ff00; /* Màu xanh lá */
                          font-weight: bold;
                      }
                      .info-image { 
                          height: 250px; 
                      }
                      .button-container, .detail-info { 
                          text-align: center; 
                      }
                  </style>
                  
                  <script>
                    // Hàm khởi tạo vị trí
                    function requestLocation() {
                            if (navigator.geolocation) {
                                // Yêu cầu lấy vị trí của người dùng
                                navigator.geolocation.getCurrentPosition(
                                    (position) => {
                                        const latitude = position.coords.latitude;
                                        const longitude = position.coords.longitude;
                    
                                        // Gọi Kakao Maps API để lấy thông tin khu vực từ vĩ độ và kinh độ
                                        fetch(`https://dapi.kakao.com/v2/local/geo/coord2regioncode.json?x=${longitude}&y=${latitude}`, {
                                            method: 'GET',
                                            headers: {
                                                'Authorization': 'KakaoAK 12873a4a25a298774293ab8c899a1432'  // Thay YOUR_KAKAO_API_KEY bằng API Key thực tế của bạn
                                            }
                                        })
                                        .then(response => response.json())
                                        .then(data => {
                                          if (data.documents && data.documents.length > 0) {
                            const region1 = data.documents[0].region_1depth_name;  // Quận hoặc khu vực
                            const region2 = data.documents[0].region_2depth_name;  // Thị trấn hoặc xã
                            const region3 = data.documents[0].region_3depth_name || "Không xác định";  // Khu vực nhỏ hơn

                                            // Hiển thị kết quả
                                            document.getElementById('location-range-AMY').textContent = `Vị trí của bạn: ${region1} - ${region2} - ${region3}`;
                                        } else {
                                            document.getElementById('location-range-AMY').textContent = "Đang xác định";
                                        }
                                    })
                                    .catch(err => {
                                        console.error("Lỗi khi lấy vị trí:", err);
                                        document.getElementById('location-range-AMY').textContent = "Lỗi khi lấy thông tin vị trí.";
                                    });
                                },
                                (error) => {
                                    console.error("Lỗi khi lấy vị trí:", error);
                                    alert("Không thể lấy vị trí. Vui lòng kiểm tra cài đặt vị trí của bạn.");
                                }
                            );
                        } else {
                            alert("Trình duyệt của bạn không hỗ trợ Geolocation.");
                        }
                    }
                
                    // Gọi hàm yêu cầu vị trí khi trang được tải
                    requestLocation();
                </script>
                
                  <!-- HTML phần tử hiển thị vị trí -->
                  <div class="location-info">
                      <span id="location-range-AMY">Đang xác định</span>
                  </div>
                    <button onclick="showInputBox('AMY', 'phone')">SDT</button>
               
                    <button onclick="showInputBox('AMY', 'telegram')">Telegram</button>
                    <p><i class="fas fa-clock"></i> <strong>Thời gian gia nhập:</strong> 02/07/2024 14:00</p>
                    <i class="fas fa-user"></i> Hoạt động: <span class="active-status">Đang hoạt động</span>
    
                    <div id="bio-AMY" style="display: block;">
                        
                            <h4>Giới thiệu</h4>
                            <p>
                                Em cực xinh cực dâm vú mông cực to chỉ cần một lần tiếp xúc sẽ là một ấn tượng sâu đậm</p>
                            <p>Vẻ đẹp tự nhiên có sức hút làm người khác mê mẩn,gương mặt xinh,hồn nhiên và thánh thiện,rất khả ái và dễ mến</p>
                        <p>Cộng thêm cách nói chuyện rất khéo léo giọng nói nhẹ nhàng ngọt ngào cho ta cảm giác rất thật lòng cũng là những điểm đáng mến từ em
    </p>
    <p><i class="fas fa-birthday-cake"></i> <strong>Năm sinh:</strong> 2000</p>
    <p><i class="fas fa-ruler-vertical"></i> <strong>Cao (cm):</strong> 1620</p>
    <p><i class="fas fa-weight-hanging"></i> <strong>Nặng (kg):</strong> 49</p>
    <p><i class="fas fa-tape"></i> <strong>Vòng 1 (cm):</strong> 90</p>
    <p><i class="fas fa-tape"></i> <strong>Vòng 2 (cm):</strong> 60</p>
    <p><i class="fas fa-tape"></i> <strong>Vòng 3 (cm):</strong> 93</p>
   <p><i class="fas fa-smile"></i> <strong>Khuôn mặt:</strong> Thanh tú và quyến rũ</p>
    <p><i class="fas fa-eye"></i> <strong>Nhận dạng:</strong> Vóc dáng chuẩn, body săn chắc và nóng bỏng, phong cách gợi cảm</p>
</div>
                </div>
            </div>
        </div>

        <div id="review-container-AMY" class="review-section">
    <h4>Đánh giá của bạn cho AMY</h4>
    <div class="stars">
        <span class="star" onclick="rateStar('AMY', 1)">&#9733;</span>
        <span class="star" onclick="rateStar('AMY', 2)">&#9733;</span>
        <span class="star" onclick="rateStar('AMY', 3)">&#9733;</span>
        <span class="star" onclick="rateStar('AMY', 4)">&#9733;</span>
        <span class="star" onclick="rateStar('AMY', 5)">&#9733;</span>
    </div>

</div>

       
<script>
   
    function rateStar(character, star) {
     const result = document.getElementById(`rating-result-${character}`);
 
     if (result) {
         // Hiển thị thông báo đánh giá
         result.innerText = `Bạn đã đánh giá ${star} sao cho ${character}!`;
 
         // Sau 3 giây, hiển thị thông báo cảm ơn và ẩn đi sau đó
         setTimeout(() => {
             result.innerText = `Cảm ơn bạn đã đánh giá cho ${character}. Mỗi lượt đánh giá của bạn góp phần thay đổi thứ hạng của cô ấy! Chỉ tính lần đầu trong ngày ❤️`;
 
             // Ẩn thông báo sau thêm 2 giây nữa
             setTimeout(() => {
                 result.innerText = ''; // Xóa nội dung để ẩn đi
                 result.style.display = 'none'; // Ẩn phần tử
             }, 2000);
         }, 3000);
     } else {
         console.error("Không tìm thấy phần tử kết quả đánh giá!");
     }
 }
 
 // Tạo phần tử để hiển thị kết quả đánh giá trong HTML (nếu chưa có)
 document.querySelectorAll('.review-section').forEach(section => {
     const character = section.id.split('-')[2]; // Lấy tên nhân vật từ ID
     if (!document.getElementById(`rating-result-${character}`)) {
         const resultElement = document.createElement('p');
         resultElement.id = `rating-result-${character}`;
         section.appendChild(resultElement);
     }
 });
     
 </script>
</style>

        <!-- Hình ảnh -->
        <div id="images-AMY" style="display: none;">
            <h4>Hình ảnh</h4>
            <a href="https://ibb.co/kyZvwKj"><img src="https://i.ibb.co/kyZvwKj/416836167-18319225438140467-3211025461518436963-n.jpg" alt="Image New 1" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/9ZXWTQX"><img src="https://i.ibb.co/9ZXWTQX/416969166-18319225423140467-5603286920183519950-n.jpg" alt="Image New 2" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/s2m0rsv"><img src="https://i.ibb.co/s2m0rsv/417020711-18319225441140467-7148758048589178387-n.jpg" alt="Image New 3" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/4YtwyfY"><img src="https://i.ibb.co/4YtwyfY/456111299-18348803026140467-918336652170975872-n.jpg" alt="Image New 4" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/YDJgwCy"><img src="https://i.ibb.co/YDJgwCy/456486586-18349431616140467-8591061972536888890-n.jpg" alt="Image New 5" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/Lnb8HBx"><img src="https://i.ibb.co/Lnb8HBx/456487412-18349431598140467-3082900273994637775-n.jpg" alt="Image New 6" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/fM5PQvL"><img src="https://i.ibb.co/fM5PQvL/456510459-18349431607140467-6369908208813540895-n-1.jpg" alt="Image New 7" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/6mzZM8Q"><img src="https://i.ibb.co/6mzZM8Q/461445056-18354338752140467-7919709787529616807-n.jpg" alt="Image New 8" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/mNqj9xN"><img src="https://i.ibb.co/mNqj9xN/461857515-18355249507140467-2837449301235508990-n.jpg" alt="Image New 9" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/JxmyVYv"><img src="https://i.ibb.co/JxmyVYv/461940571-18355249525140467-6145041215129117621-n.jpg" alt="Image New 10" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/LSn3zXs"><img src="https://i.ibb.co/LSn3zXs/462269119-18355973512140467-6139831667677658778-n.jpg" alt="Image New 11" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/ZfXBvz9"><img src="https://i.ibb.co/ZfXBvz9/Instagram-highlights-stories-17977193060735719-1.jpg" alt="Image New 13" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/DC7XjKx"><img src="https://i.ibb.co/DC7XjKx/Instagram-highlights-stories-17977193060735719.jpg" alt="Image New 14" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/mhgWXqs"><img src="https://i.ibb.co/mhgWXqs/photo-2024-10-07-21-11-41.jpg" alt="Image New 15" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/Y0JWRhC"><img src="https://i.ibb.co/Y0JWRhC/Save-The-Video-App-363500522-229433956233642-5587940116585302164-n.jpg" alt="Image New 16" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/jRY8smp"><img src="https://i.ibb.co/jRY8smp/Save-The-Video-App-364263036-261824383267329-9143166390948101533-n.jpg" alt="Image New 17" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/ckmnW8N"><img src="https://i.ibb.co/ckmnW8N/Save-The-Video-App-364341204-799791968556585-7807479463862832425-n.jpg" alt="Image New 18" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/rkdrpnH"><img src="https://i.ibb.co/rkdrpnH/Save-The-Video-App-365548000-852986726249697-4742178861420926061-n-1.jpg" alt="Image New 19" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/YBf0cht"><img src="https://i.ibb.co/YBf0cht/Save-The-Video-App-454564779-18347425165140467-8323930334737558718-n.jpg" alt="Image New 20" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/F47gvZD"><img src="https://i.ibb.co/F47gvZD/Save-The-Video-App-460575704-18353366170140467-6835324141600346990-n.jpg" alt="Image New 21" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/D7fL2NC"><img src="https://i.ibb.co/D7fL2NC/Save-The-Video-App-460658080-18353366155140467-162377102346118466-n.jpg" alt="Image New 22" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/G7Bvcmh"><img src="https://i.ibb.co/G7Bvcmh/Save-The-Video-App-460727619-18353366233140467-4855929002437452289-n.jpg" alt="Image New 23" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/qC25hk4"><img src="https://i.ibb.co/qC25hk4/Save-The-Video-App-460747569-18353366179140467-7718809086127651176-n.jpg" alt="Image New 24" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/9bx6cXC"><img src="https://i.ibb.co/9bx6cXC/Save-The-Video-App-460802633-18353366224140467-4748650278288112717-n.jpg" alt="Image New 25" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/FYrQXZJ"><img src="https://i.ibb.co/FYrQXZJ/Save-The-Video-App-460804670-18353366194140467-1092024016528287386-n.jpg" alt="Image New 26" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/pXj1Nzg"><img src="https://i.ibb.co/pXj1Nzg/Save-The-Video-App-460832718-18353633767140467-8137333835235299238-n.jpg" alt="Image New 27" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/TPtvK9j"><img src="https://i.ibb.co/TPtvK9j/photo-9-2024-09-20-09-04-21.jpg" alt="Image New 30" class="info-image" style="height: 190px; width: auto;"></a>
            <a href="https://ibb.co/85FFZhC"><img src="https://i.ibb.co/85FFZhC/photo-10-2024-09-20-09-04-21.jpg" alt="Image New 31" class="info-image" style="height: 190px; width: auto;"></a>
            
</div>
    
        <!-- Đặt lịch -->
        <div id="bookings-AMY" style="display: none;">
            <h4>Đặt lịch</h4>
            <p><i class="fas fa-book"></i> <strong>Hướng dẫn đặt lịch :</strong>
               HÃY LÀ MỘT CHECKER VĂN MINH !</p>
            <p><i class="fas fa-calendar-alt"></i> <strong>Vui lòng đăng nhập để đặt lịch !</strong></p>
        </div>
    </div>

          

           <!-- Chi tiết Hà My -->
<div id="detail-HaMy" class="detail-info">
    <h3>Hà My</h3>
    <div class="button-container">
        <button class="info-button" onclick="toggleContent('HaMy', 'info')">
            <i class="fas fa-info-circle"></i> Thông tin
        </button>
        <button class="info-button" onclick="toggleContent('HaMy', 'images')">
            <i class="fas fa-images"></i> Hình ảnh
        </button>
        <button onclick="openBookingModal('HaMy')">Đặt lịch</button>
    </div>

    <!-- Thông tin chi tiết -->
    <div id="info-HaMy" style="display: none">
        <h4>Thông tin</h4>
        <div class="info-content">
            <img src="https://i.ibb.co/bHLbVdD/455691559-122111257202434651-6263614150393024155-n.jpg" alt="Image 8" class="info-image" style="height: 250px;">


            <div class="info-text">
              
                <style>
                    /* styles.css */
                    .location-info {
                        font-size: 17px;
                        color: #00ff00; /* Màu xanh lá */
                        font-weight: bold;
                    }
                </style>
                <script>
                 // Hàm khởi tạo vị trí
                 function requestLocation() {
                            if (navigator.geolocation) {
                                // Yêu cầu lấy vị trí của người dùng
                                navigator.geolocation.getCurrentPosition(
                                    (position) => {
                                        const latitude = position.coords.latitude;
                                        const longitude = position.coords.longitude;
                    
                                        // Gọi Kakao Maps API để lấy thông tin khu vực từ vĩ độ và kinh độ
                                        fetch(`https://dapi.kakao.com/v2/local/geo/coord2regioncode.json?x=${longitude}&y=${latitude}`, {
                                            method: 'GET',
                                            headers: {
                                                'Authorization': 'KakaoAK 12873a4a25a298774293ab8c899a1432'  // Thay YOUR_KAKAO_API_KEY bằng API Key thực tế của bạn
                                            }
                                        })
                                        .then(response => response.json())
                                        .then(data => {
                                          if (data.documents && data.documents.length > 0) {
                            const region1 = data.documents[0].region_1depth_name;  // Quận hoặc khu vực
                            const region2 = data.documents[0].region_2depth_name;  // Thị trấn hoặc xã
                            const region3 = data.documents[0].region_3depth_name || "Không xác định";  // Khu vực nhỏ hơn
              
                                          // Hiển thị kết quả
                                          document.getElementById('location-range-HAMY').textContent = `Vị trí của bạn: ${region1} - ${region2} - ${region3}`;
                                      } else {
                                          document.getElementById('location-range-HAMY').textContent = "Đang xác định";
                                      }
                                  })
                                  .catch(err => {
                                      console.error("Lỗi khi lấy vị trí:", err);
                                      document.getElementById('location-range-HAMY').textContent = "Lỗi khi lấy thông tin vị trí.";
                                  });
                              },
                              (error) => {
                                  console.error("Lỗi khi lấy vị trí:", error);
                                  alert("Không thể lấy vị trí. Vui lòng kiểm tra cài đặt vị trí của bạn.");
                              }
                          );
                      } else {
                          alert("Trình duyệt của bạn không hỗ trợ Geolocation.");
                      }
                  }
              
                  // Gọi hàm yêu cầu vị trí khi trang được tải
                  requestLocation();
              </script>
              
              <!-- HTML phần tử hiển thị vị trí -->
              <div class="location-info">
                  <span id="location-range-HAMY">Đang xác định</span>
              </div>
              

                <button onclick="showInputBox('HaMy', 'phone')">SDT</button>
               
                <button onclick="showInputBox('HaMy', 'telegram')">Telegram</button>
                <p><i class="fas fa-clock"></i> <strong>Thời gian gia nhập:</strong> 12/07/2024 12:03</p>
                <i class="fas fa-user"></i> Hoạt động: <span class="active-status">Đang hoạt động</span>
                </p>
            </div>
        </div>
        <h4>Giới thiệu</h4>
        <p>
            Bé có một dáng người mềm mại muốn ôm mãi không thôi</p>  
        <p>Gương mặt dễ thương, ngây thơ đáng yêu , ngực to và trắng, đầu ti hồng hào nghịch khá thích</p> 
    <p>Hàng này vét đã lắm ạ, thơm tho, nước ra lênh láng, tiếng rên bẽn lẽn đáng yêu</p> 
<p>Khoản này chắc các anh trai thích nhất rồi</p> 
            <p> Kết : Bé còn chút ngại ngùng khi nói chuyện, nhưng thái độ lúc lâm trận rất nhiệt tình, chịu khó học hỏi, phối hợp các tư thế
        </p>
        <p><i class="fas fa-birthday-cake"></i> <strong>Năm sinh:</strong> 2000</p>
        <p><i class="fas fa-ruler-vertical"></i> <strong>Cao (cm):</strong> 163</p>
        <p><i class="fas fa-weight-hanging"></i> <strong>Nặng (kg):</strong> 49</p>
        <p><i class="fas fa-tape"></i> <strong>Vòng 1 (cm):</strong> 88</p>
        <p><i class="fas fa-tape"></i> <strong>Vòng 2 (cm):</strong> 59</p>
        <p><i class="fas fa-tape"></i> <strong>Vòng 3 (cm):</strong> 91</p>
        <p><i class="fas fa-scissors"></i> <strong>Lông bím:</strong> Gọn gàng</p>
        <p><i class="fas fa-smile"></i> <strong>Mặt:</strong> Xinh đẹp, thân thiện</p>
        <p><i class="fas fa-eye"></i> <strong>Nhận dạng:</strong> Gái ngon, xinh, nhìn rất đáng yêu</p>
        <p><i class="fas fa-clock"></i> <strong>Hoạt động:</strong> Giờ nào cũng ok</p>
    </div>

    <div id="review-container-HaMy" class="review-section">
        <h4>Đánh giá của bạn cho Hà My</h4>
        <div class="stars">
            <span class="star" onclick="rateStar('HaMy', 1)">&#9733;</span>
            <span class="star" onclick="rateStar('HaMy', 2)">&#9733;</span>
            <span class="star" onclick="rateStar('HaMy', 3)">&#9733;</span>
            <span class="star" onclick="rateStar('HaMy', 4)">&#9733;</span>
            <span class="star" onclick="rateStar('HaMy', 5)">&#9733;</span>
        </div>
    </div>

     
    <script>
   
        function rateStar(character, star) {
         const result = document.getElementById(`rating-result-${character}`);
     
         if (result) {
             // Hiển thị thông báo đánh giá
             result.innerText = `Bạn đã đánh giá ${star} sao cho ${character}!`;
     
             // Sau 3 giây, hiển thị thông báo cảm ơn và ẩn đi sau đó
             setTimeout(() => {
                 result.innerText = `Cảm ơn bạn đã đánh giá cho ${character}. Mỗi lượt đánh giá của bạn góp phần thay đổi thứ hạng của cô ấy! Chỉ tính lần đầu trong ngày ❤️`;
     
                 // Ẩn thông báo sau thêm 2 giây nữa
                 setTimeout(() => {
                     result.innerText = ''; // Xóa nội dung để ẩn đi
                     result.style.display = 'none'; // Ẩn phần tử
                 }, 2000);
             }, 3000);
         } else {
             console.error("Không tìm thấy phần tử kết quả đánh giá!");
         }
     }
     
     // Tạo phần tử để hiển thị kết quả đánh giá trong HTML (nếu chưa có)
     document.querySelectorAll('.review-section').forEach(section => {
         const character = section.id.split('-')[2]; // Lấy tên nhân vật từ ID
         if (!document.getElementById(`rating-result-${character}`)) {
             const resultElement = document.createElement('p');
             resultElement.id = `rating-result-${character}`;
             section.appendChild(resultElement);
         }
     });
         
     </script>

<style>
  .review-section {
      margin-top: 20px;
      padding: 10px;
      background-color: #000000; /* Màu nền nút cam đậm */
      color: #ffffff;
      border-radius: 5px;
  }
  .stars {
      font-size: 20px;
      color: #ffcc00;
  }
  .star {
      cursor: pointer;
  }
</style>
        
           <!-- Hình ảnh -->
    <div id="images-HaMy" style="display: none">
        <h4>Hình ảnh</h4>
        <a href="https://i.ibb.co/sFpYycr"><img src="https://i.ibb.co/sFpYycr/452346105-122097053972434651-70304625633922474-n.jpg" alt="Image 1" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/SmdxdWh"><img src="https://i.ibb.co/SmdxdWh/452456058-122097965540434651-3912502212670174861-n.jpg" alt="Image 2" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/WzHdPPS"><img src="https://i.ibb.co/WzHdPPS/453808018-122106853232434651-4604519005165612319-n.jpg" alt="Image 3" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/TmfLwVb"><img src="https://i.ibb.co/TmfLwVb/454325120-122108645144434651-795226551275134592-n.jpg" alt="Image 4" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/XZ45hh0"><img src="https://i.ibb.co/XZ45hh0/454819894-122109417518434651-4162265515860444955-n.jpg" alt="Image 5" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/ZXkgCXB"><img src="https://i.ibb.co/ZXkgCXB/455314793-122110440716434651-433169597141769416-n.jpg" alt="Image 6" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/4SNd7hF"><img src="https://i.ibb.co/4SNd7hF/455277592-122110743476434651-3300050035046233741-n.jpg" alt="Image 7" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/bHLbVdD"><img src="https://i.ibb.co/bHLbVdD/455691559-122111257202434651-6263614150393024155-n.jpg" alt="Image 8" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/7gdFX78"><img src="https://i.ibb.co/7gdFX78/455968603-122111767070434651-6913421045416419060-n.jpg" alt="Image 9" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/sP5J3yX"><img src="https://i.ibb.co/sP5J3yX/456513928-122112246536434651-2776176340085354863-n.jpg" alt="Image 10" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/0YgLdkf"><img src="https://i.ibb.co/0YgLdkf/456565869-122112731396434651-8237853306147565521-n.jpg" alt="Image 11" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/djNfmx1"><img src="https://i.ibb.co/djNfmx1/457033116-122113186844434651-6281615223706451419-n.jpg" alt="Image 12" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/3yVT1xt"><img src="https://i.ibb.co/3yVT1xt/457183690-122113673636434651-3115662083493267900-n.jpg" alt="Image 13" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/yd0CyK7"><img src="https://i.ibb.co/yd0CyK7/457876971-122114618300434651-2157768203712887052-n.jpg" alt="Image 14" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/qDpG43q"><img src="https://i.ibb.co/qDpG43q/460636309-122118376964434651-2180858217538166205-n.jpg" alt="Image 15" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/J3zsY7S"><img src="https://i.ibb.co/J3zsY7S/461512276-122119820114434651-7954635395370619903-n.jpg" alt="Image 16" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/2N37mqL"><img src="https://i.ibb.co/2N37mqL/462373564-122121580796434651-8196861796321031764-n.jpg" alt="Image 17" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/JHkGjnJ"><img src="https://i.ibb.co/JHkGjnJ/462646415-122122065134434651-8643311744588327997-n.jpg" alt="Image 18" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/MpQ8D12"><img src="https://i.ibb.co/MpQ8D12/462746291-122122415960434651-8840312681855580438-n.jpg" alt="Image 19" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/7NMDBBm"><img src="https://i.ibb.co/7NMDBBm/464133519-122123559818434651-9114080325865249596-n.jpg" alt="Image 20" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/HG9nkg3"><img src="https://i.ibb.co/HG9nkg3/464328944-122123883152434651-9138667014083794969-n.jpg" alt="Image 21" class="info-image" style="height: 190px; width: auto;"></a>
        <a href="https://i.ibb.co/8s4Ghcd"><img src="https://i.ibb.co/8s4Ghcd/465005198-122124788240434651-1038284664742036829-n.jpg" alt="Image 22" class="info-image" style="height: 190px; width: auto;"></a>

            </div>
        
            <!-- Số lượt book -->
    <div id="bookings-HaMy" style="display: none">
        <h4>Đặt lịch</h4>
        <p><i class="fas fa-book"></i> <strong>Hướng dẫn đặt lịch:</strong>
           HÃY LÀ MỘT CHECKER VĂN MINH !</p>
        <p><i class="fas fa-calendar-alt"></i> <strong>Vui lòng đăng nhập để đặt lịch</strong></p>
    </div>

    <!-- Giới thiệu -->
    <div id="bio-HaMy" style="display: none">
        <h4>Giới thiệu</h4>
        <p>
            Hà My có một trái tim ấm áp và luôn mang đến sự thoải mái cho khách hàng. Cô ấy là sự kết hợp hoàn hảo giữa vẻ đẹp và sự dịu dàng, làm hài lòng mọi người tại Diamond Club.
        </p>
    </div>
</div>
          
            <!-- Chi tiết MINA -->
            <div id="detail-MINA" class="detail-info">
              <h3>MINA</h3>
              <div class="button-container">
                  <button class="info-button" onclick="toggleContent('MINA', 'info')">
                      <i class="fas fa-info-circle"></i> Thông tin
                  </button>
                  <button class="info-button" onclick="toggleContent('MINA', 'images')">
                      <i class="fas fa-images"></i> Hình ảnh
                  </button>
                    <button onclick="openBookingModal('MINA')">Đặt lịch</button>
                </button>
            </div>
          
          
              <!-- Thông tin chi tiết -->
              <div id="info-MINA" style="display: none">
                  <h4>Thông tin</h4>
                  <div class="info-content">
                    <img src="https://i.ibb.co/9HyQwy6/462776443-1193449098391062-5602390579257707131-n.jpg" alt="Image New 60" class="info-image" style="height: 250px;">
                      <div class="info-text">
                      
                          <style>
                            /* styles.css */
                            .location-info {
                                font-size: 17px;
                                color: #00ff00; /* Màu xanh lá */
                                font-weight: bold;
                            }
                            .info-image { 
                                height: 250px; 
                            }
                            .button-container, .detail-info { 
                                text-align: center; 
                            }
                        </style>
                        
                        <script>
                         // Hàm khởi tạo vị trí
                         function requestLocation() {
                            if (navigator.geolocation) {
                                // Yêu cầu lấy vị trí của người dùng
                                navigator.geolocation.getCurrentPosition(
                                    (position) => {
                                        const latitude = position.coords.latitude;
                                        const longitude = position.coords.longitude;
                    
                                        // Gọi Kakao Maps API để lấy thông tin khu vực từ vĩ độ và kinh độ
                                        fetch(`https://dapi.kakao.com/v2/local/geo/coord2regioncode.json?x=${longitude}&y=${latitude}`, {
                                            method: 'GET',
                                            headers: {
                                                'Authorization': 'KakaoAK 12873a4a25a298774293ab8c899a1432'  // Thay YOUR_KAKAO_API_KEY bằng API Key thực tế của bạn
                                            }
                                        })
                                        .then(response => response.json())
                                        .then(data => {
                                          if (data.documents && data.documents.length > 0) {
                            const region1 = data.documents[0].region_1depth_name;  // Quận hoặc khu vực
                            const region2 = data.documents[0].region_2depth_name;  // Thị trấn hoặc xã
                            const region3 = data.documents[0].region_3depth_name || "Không xác định";  // Khu vực nhỏ hơn
                      
                                                  // Hiển thị kết quả
                                                  document.getElementById('location-range-MINA').textContent = `Vị trí của bạn: ${region1} - ${region2} - ${region3}`;
                                              } else {
                                                  document.getElementById('location-range-MINA').textContent = "Đang xác định";
                                              }
                                          })
                                          .catch(err => {
                                              console.error("Lỗi khi lấy vị trí:", err);
                                              document.getElementById('location-range-MINA').textContent = "Lỗi khi lấy thông tin vị trí.";
                                          });
                                      },
                                      (error) => {
                                          console.error("Lỗi khi lấy vị trí:", error);
                                          alert("Không thể lấy vị trí. Vui lòng kiểm tra cài đặt vị trí của bạn.");
                                      }
                                  );
                              } else {
                                  alert("Trình duyệt của bạn không hỗ trợ Geolocation.");
                              }
                          }
                      
                          // Gọi hàm yêu cầu vị trí khi trang được tải
                          requestLocation();
                      </script>
                      
                      <!-- HTML phần tử hiển thị vị trí -->
                      <div class="location-info">
                          <span id="location-range-MINA">Đang xác định...</span>
                      </div>
                      
                        
                          <button onclick="showInputBox('MINA', 'phone')">SDT</button>

<button onclick="showInputBox('MINA', 'telegram')">Telegram</button>
                          <p><i class="fas fa-clock"></i> <strong>Thời gian gia nhập:</strong> 12/07/2024 09:19</p>
                          <i class="fas fa-user"></i> Hoạt động: <span class="active-status">Đang hoạt động</span>
                        </p>
                      </div>
                  </div>

          
                  <h4>Giới thiệu</h4>
                  <p>
                    Bé mới vào nghề có chất giọng nhẹ nhàng êm ái ngọt liệm nghe giọng bé nói chuyện the thẻ tạo thêm cảm giác hưng phấn cho thằng nhỏ dâng trào hứng nứng lên bất ngờ
                <p>Phong cách ăn mặc trẻ trung tạo cảm giác ấn tượng với bé</p>
            <p>Và chuyện làm tình bé mới làm nên cái cơ bản sung sướng ấn tượng khó quên về bé
                </p>
                <p><i class="fas fa-birthday-cake"></i> <strong>Năm sinh:</strong> 2002</p>
                <p><i class="fas fa-ruler-vertical"></i> <strong>Cao (cm):</strong> 163</p>
                <p><i class="fas fa-weight-hanging"></i> <strong>Nặng (kg):</strong> 46</p>
                <p><i class="fas fa-tape"></i> <strong>Vòng 1 (cm):</strong> 86</p>
                <p><i class="fas fa-tape"></i> <strong>Vòng 2 (cm):</strong> 58</p>
                <p><i class="fas fa-tape"></i> <strong>Vòng 3 (cm):</strong> 90</p>
                <p><i class="fas fa-smile"></i> <strong>Khuôn mặt:</strong> Ngọt ngào, thanh thoát và đáng yêu</p>
                <p><i class="fas fa-eye"></i> <strong>Nhận dạng:</strong> Vóc dáng cân đối, phong cách trẻ trung và gợi cảm</p>
                <p><i class="fas fa-clock"></i> <strong>Hoạt động:</strong> 24/24</p>
            </div>

              <div id="review-container-MINA" class="review-section">
    <h4>Đánh giá của bạn cho MINA</h4>
    <div class="stars">
        <span class="star" onclick="rateStar('MINA', 1)">&#9733;</span>
        <span class="star" onclick="rateStar('MINA', 2)">&#9733;</span>
        <span class="star" onclick="rateStar('MINA', 3)">&#9733;</span>
        <span class="star" onclick="rateStar('MINA', 4)">&#9733;</span>
        <span class="star" onclick="rateStar('MINA', 5)">&#9733;</span>
    </div>
</div>

<script>
   
    function rateStar(character, star) {
     const result = document.getElementById(`rating-result-${character}`);
 
     if (result) {
         // Hiển thị thông báo đánh giá
         result.innerText = `Bạn đã đánh giá ${star} sao cho ${character}!`;
 
         // Sau 3 giây, hiển thị thông báo cảm ơn và ẩn đi sau đó
         setTimeout(() => {
             result.innerText = `Cảm ơn bạn đã đánh giá cho ${character}. Mỗi lượt đánh giá của bạn góp phần thay đổi thứ hạng của cô ấy! Chỉ tính lần đầu trong ngày ❤️`;
 
             // Ẩn thông báo sau thêm 2 giây nữa
             setTimeout(() => {
                 result.innerText = ''; // Xóa nội dung để ẩn đi
                 result.style.display = 'none'; // Ẩn phần tử
             }, 2000);
         }, 3000);
     } else {
         console.error("Không tìm thấy phần tử kết quả đánh giá!");
     }
 }
 
 // Tạo phần tử để hiển thị kết quả đánh giá trong HTML (nếu chưa có)
 document.querySelectorAll('.review-section').forEach(section => {
     const character = section.id.split('-')[2]; // Lấy tên nhân vật từ ID
     if (!document.getElementById(`rating-result-${character}`)) {
         const resultElement = document.createElement('p');
         resultElement.id = `rating-result-${character}`;
         section.appendChild(resultElement);
     }
 });
     
 </script>
<style>
    .review-section {
        margin-top: 20px;
        padding: 10px;
        background: #000000;
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
       
    border: 1px solid #C0C0C0; /* Viền bạc */
    border-radius: 5px;
    }
    .stars {
        font-size: 20px;
        color: #000000;
    }
    .star {
        cursor: pointer;
    }
</style>

          
              <!-- Hình ảnh -->
              <div id="images-MINA" style="display: none">
                  <h4>Hình ảnh</h4>
                  <a href="https://ibb.co/8d3nnBZ"><img src="https://i.ibb.co/8d3nnBZ/383337930-978863159849658-4641272384526547692-n.jpg" alt="Image New 43" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/MBpmQqb"><img src="https://i.ibb.co/MBpmQqb/407908628-1013974159671891-2417822945034929073-n.jpg" alt="Image New 45" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/R67pZxq"><img src="https://i.ibb.co/R67pZxq/423236603-1042520383483935-3619898868584313772-n.jpg" alt="Image New 46" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/GQ5wry4"><img src="https://i.ibb.co/GQ5wry4/422974615-1042520403483933-1330128733791845372-n.jpg" alt="Image New 47" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/KF72fzH"><img src="https://i.ibb.co/KF72fzH/432647796-1070266404042666-9193305764823014635-n.jpg" alt="Image New 48" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/JHKvs8V"><img src="https://i.ibb.co/JHKvs8V/435702528-1080279893041317-8914284036668817236-n.jpg" alt="Image New 49" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/6wmMyqx"><img src="https://i.ibb.co/6wmMyqx/449039576-1124677385268234-7665507449582176569-n.jpg" alt="Image New 50" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/8gfpCVM"><img src="https://i.ibb.co/8gfpCVM/449039576-1124677408601565-3024710156838684119-n.jpg" alt="Image New 51" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/RjBPhXC"><img src="https://i.ibb.co/RjBPhXC/453315351-1144148666654439-988129998488451481-n.jpg" alt="Image New 52" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/vz1vNVb"><img src="https://i.ibb.co/vz1vNVb/456599617-1160972514972054-4029686110250322599-n.jpg" alt="Image New 55" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/cQwTPdX"><img src="https://i.ibb.co/cQwTPdX/456603795-1160972528305386-3708613599631951145-n.jpg" alt="Image New 56" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/k4GVGzH"><img src="https://i.ibb.co/k4GVGzH/456694132-1160972558305383-3403657865890027602-n.jpg" alt="Image New 57" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/pRW0zKW"><img src="https://i.ibb.co/pRW0zKW/459851929-1175238350212137-3962964322160869963-n.jpg" alt="Image New 58" style="height: 190px; width: auto;"></a>
                  <a href="https://ibb.co/v3zfwHK"><img src="https://i.ibb.co/v3zfwHK/462685881-1193449008391071-3934223950662475783-n.jpg" alt="Image New 59" style="height: 190px; width: auto;"></a>
                  
              </div>
          
              <!-- Số lượt book -->
              <div id="bookings-MINA" style="display: none">
                  <h4>Đặt lịch</h4>
                  <p><i class="fas fa-book"></i> <strong>Hướng dẫn đặt lịch:</strong>
                    * Khi set kèo HÃY LÀ MỘT CHECKER VĂN MINH !</p>
                  <p><i class="fas fa-calendar-alt"></i> <strong>Vui lòng đăng nhập để đặt lịch</strong></p>
              </div>
          
              <!-- Giới thiệu -->
              <div id="bio-MINA" style="display: none">
                  <h4>Giới thiệu</h4>
                  <p>
                      Mina mang đến những trải nghiệm đầy màu sắc với dịch vụ chuyên nghiệp và tận tâm. Cô ấy là một trong những thành viên nổi bật tại Diamond Club.
                  </p>
              </div>
          </div>
          

            <div id="detail-LUCY" class="detail-info">
    <h3>LUCY</h3>
    <div class="button-container">
        <button class="info-button" onclick="toggleContent('LUCY', 'info')">
            <i class="fas fa-info-circle"></i> Thông tin
        </button>
        <button class="info-button" onclick="toggleContent('LUCY', 'images')">
            <i class="fas fa-images"></i> Hình ảnh
        </button>
          <button onclick="openBookingModal('LUCY')">Đặt lịch</button>
    </button>
</div>
    <!-- Thông tin chi tiết -->
    <div id="info-LUCY" style="display: none">
        <h4>Thông tin</h4>
        <div class="info-content">
            <img src="https://i.ibb.co/Dfc46yb/photo-2024-09-05-18-55-27.jpg" alt="Image New 67" class="info-image" style="height: 250px;">
            <div class="info-text">
            
                <style>
                  /* styles.css */
                  .location-info {
                      font-size: 17px;
                      color: #00ff00; /* Màu xanh lá */
                      font-weight: bold;
                  }
                  .info-image { 
                      height: 250px; 
                  }
                  .button-container, .detail-info { 
                      text-align: center; 
                  }
              </style>
              
              <script>
                 // Hàm khởi tạo vị trí
                 function requestLocation() {
                            if (navigator.geolocation) {
                                // Yêu cầu lấy vị trí của người dùng
                                navigator.geolocation.getCurrentPosition(
                                    (position) => {
                                        const latitude = position.coords.latitude;
                                        const longitude = position.coords.longitude;
                    
                                        // Gọi Kakao Maps API để lấy thông tin khu vực từ vĩ độ và kinh độ
                                        fetch(`https://dapi.kakao.com/v2/local/geo/coord2regioncode.json?x=${longitude}&y=${latitude}`, {
                                            method: 'GET',
                                            headers: {
                                                'Authorization': 'KakaoAK 12873a4a25a298774293ab8c899a1432'  // Thay YOUR_KAKAO_API_KEY bằng API Key thực tế của bạn
                                            }
                                        })
                                        .then(response => response.json())
                                        .then(data => {
                                          if (data.documents && data.documents.length > 0) {
                            const region1 = data.documents[0].region_1depth_name;  // Quận hoặc khu vực
                            const region2 = data.documents[0].region_2depth_name;  // Thị trấn hoặc xã
                            const region3 = data.documents[0].region_3depth_name || "Không xác định";  // Khu vực nhỏ hơn
              
                                              // Hiển thị thông tin thị trấn và quận bằng tiếng Hàn
                                              document.getElementById('location-range-LUCY').textContent = `${town} (${data.results[0].components.town}) - ${district} (${data.results[0].components.district})`;
                                          } else {
                                              document.getElementById('location-range-LUCY').textContent = "Đang xác định";
                                          }
                                      })
                                      .catch(err => {
                                          console.error("Error getting location:", err);
                                          document.getElementById('location-range-LUCY').textContent = "Lỗi khi lấy vị trí.";
                                      });
                              },
                              (error) => {
                                  console.error("Geolocation error:", error);
                                  alert("Không thể lấy vị trí. Vui lòng kiểm tra cài đặt vị trí của bạn.");
                              }
                          );
                      } else {
                          alert("Trình duyệt của bạn không hỗ trợ Geolocation.");
                      }
                  }
              
                  // Gọi hàm yêu cầu vị trí khi trang được tải
                  requestLocation();
              </script>
              
              <!-- HTML phần tử hiển thị vị trí -->
              <div class="location-info">
                  <span id="location-range-LUCY">Đang xác định</span>
              </div>
                <button onclick="showInputBox('LUCY', 'phone')">SDT</button>

<button onclick="showInputBox('LUCY', 'telegram')">Telegram</button>
                <p><i class="fas fa-clock"></i> <strong>Thời gian gia nhập:</strong> 28/06/2024 14:20</p>
                <p><i class="fas fa-user-check"></i> <strong>Hoạt động:</strong> Đang hoạt động</p>
            </div>
        </div>

    
            <div id="bio-LUCY" style="display: block;">
                <h4>Giới thiệu</h4>
                <p>
                  Bé rất ngon trong tầm giá với kỹ năng làm tình tuyệt vời,bài bản êm đềm và sâu lắng</p>
                  <p>Hàng tiếp rượu đẹp quyến rũ và sang chảnh</p>
                    <p>Ngoài body chuẩn không cần chỉnh bé nó còn trên cả tuyệt vời ở khoản giao tiếp ăn nói lịch sự</p> 
                        <p>Thái độ rất yêu luôn nhẹ nhàng, ngoan ngoãn, nhiệt tình và tình cảm...!
                </p>
                <p><i class="fas fa-birthday-cake"></i> <strong>Năm sinh:</strong> 2002</p>
                <p><i class="fas fa-ruler-vertical"></i> <strong>Cao (cm):</strong> 164</p>
                <p><i class="fas fa-weight-hanging"></i> <strong>Nặng (kg):</strong> 50</p>
                <p><i class="fas fa-tape"></i> <strong>Vòng 1 (cm):</strong> 90</p>
                <p><i class="fas fa-tape"></i> <strong>Vòng 2 (cm):</strong> 60</p>
                <p><i class="fas fa-tape"></i> <strong>Vòng 3 (cm):</strong> 92</p>
                <p><i class="fas fa-smile"></i> <strong>Khuôn mặt:</strong> Dễ gần</p>
                <p><i class="fas fa-eye"></i> <strong>Nhận dạng:</strong> Vóc dáng hoàn hảo, phong cách quyến rũ, thân thiện và cuốn hút</p>
                <p><i class="fas fa-clock"></i> <strong>Hoạt động:</strong> Từ trưa tới hôm sau</p>
            </div>
            
    </div>


    <div id="review-container-LUCY" class="review-section">
    <h4>Đánh giá của bạn cho LUCY</h4>
    <div class="stars">
        <span class="star" onclick="rateStar('LUCY', 1)">&#9733;</span>
        <span class="star" onclick="rateStar('LUCY', 2)">&#9733;</span>
        <span class="star" onclick="rateStar('LUCY', 3)">&#9733;</span>
        <span class="star" onclick="rateStar('LUCY', 4)">&#9733;</span>
        <span class="star" onclick="rateStar('LUCY', 5)">&#9733;</span>
    </div>
</div>

<script>
   
    function rateStar(character, star) {
     const result = document.getElementById(`rating-result-${character}`);
 
     if (result) {
         // Hiển thị thông báo đánh giá
         result.innerText = `Bạn đã đánh giá ${star} sao cho ${character}!`;
 
         // Sau 3 giây, hiển thị thông báo cảm ơn và ẩn đi sau đó
         setTimeout(() => {
             result.innerText = `Cảm ơn bạn đã đánh giá cho ${character}. Mỗi lượt đánh giá của bạn góp phần thay đổi thứ hạng của cô ấy! Chỉ tính lần đầu trong ngày ❤️`;
 
             // Ẩn thông báo sau thêm 2 giây nữa
             setTimeout(() => {
                 result.innerText = ''; // Xóa nội dung để ẩn đi
                 result.style.display = 'none'; // Ẩn phần tử
             }, 2000);
         }, 3000);
     } else {
         console.error("Không tìm thấy phần tử kết quả đánh giá!");
     }
 }
 
 // Tạo phần tử để hiển thị kết quả đánh giá trong HTML (nếu chưa có)
 document.querySelectorAll('.review-section').forEach(section => {
     const character = section.id.split('-')[2]; // Lấy tên nhân vật từ ID
     if (!document.getElementById(`rating-result-${character}`)) {
         const resultElement = document.createElement('p');
         resultElement.id = `rating-result-${character}`;
         section.appendChild(resultElement);
     }
 });
     

</script>

<style>
    .review-section {
        margin-top: 20px;
        padding: 10px;
        background-color: #1a1a1a;
        color: #ffffff;
        border-radius: 5px;
    }
    .stars {
        font-size: 20px;
        color: #ffcc00;
    }
    .star {
        cursor: pointer;
    }
</style>

    <!-- Hình ảnh -->
    <div id="images-LUCY" style="display: none">
        <h4>Hình ảnh</h4>
        <a href="https://ibb.co/KrsB7VG"><img src="https://i.ibb.co/KrsB7VG/photo-2024-09-05-18-55-28-3.jpg" alt="Image New 61" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/Sy6HCDB"><img src="https://i.ibb.co/Sy6HCDB/photo-2024-09-05-18-55-28.jpg" alt="Image New 63" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/3NngQws"><img src="https://i.ibb.co/3NngQws/photo-2024-09-05-18-55-27-4.jpg" alt="Image New 64" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/xX36C3R"><img src="https://i.ibb.co/xX36C3R/photo-2024-09-05-18-55-27-3.jpg" alt="Image New 65" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/JCCKTJ5"><img src="https://i.ibb.co/JCCKTJ5/photo-2024-09-05-18-55-26-2.jpg" alt="Image New 68" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/tJ1BFTP"><img src="https://i.ibb.co/tJ1BFTP/photo-2024-09-05-18-55-26.jpg" alt="Image New 69" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/pb18cM9"><img src="https://i.ibb.co/pb18cM9/photo-2024-09-05-18-55-25-6.jpg" alt="Image New 70" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/Dgcy4tw"><img src="https://i.ibb.co/Dgcy4tw/photo-2024-09-05-18-55-25-5.jpg" alt="Image New 71" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/x570BSZ"><img src="https://i.ibb.co/x570BSZ/photo-2024-09-05-18-55-25-3.jpg" alt="Image New 73" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/Y24sHjh"><img src="https://i.ibb.co/Y24sHjh/photo-2024-09-05-18-55-25-2.jpg" alt="Image New 74" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/xYBPfG0"><img src="https://i.ibb.co/xYBPfG0/photo-2024-09-05-18-55-25.jpg" alt="Image New 75" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/4mj3R6C"><img src="https://i.ibb.co/4mj3R6C/photo-2024-09-05-18-55-24-2.jpg" alt="Image New 76" style="height: 190px; width: auto;"></a>
<a href="https://ibb.co/k4G1kR9"><img src="https://i.ibb.co/k4G1kR9/photo-2024-09-05-18-55-24.jpg" alt="Image New 77" style="height: 190px; width: auto;"></a>
</div>
    <!-- Số lượt book -->
    <div id="bookings-LUCY" style="display: none">
        <h4>Đặt lịch</h4>
        <p><i class="fas fa-book"></i> <strong>Hướng dẫn đặt lịch:</strong>
          HÃY LÀ MỘT CHECKER VĂN MINH !</p>
        <p><i class="fas fa-calendar-alt"></i> <strong>Vui lòng đăng nhập để đặt lịch</strong></p>
    </div>

    <!-- Giới thiệu -->
    <div id="bio-LUCY" style="display: none">
        <h4>Giới thiệu</h4>
        <p>
            Lucy là một cô gái luôn biết cách làm mới bản thân và mang lại niềm vui cho khách hàng. Cô ấy có phong cách năng động và rất quyến rũ.
        </p>
    </div>
</div>


<div id="detail-SHISHI" class="detail-info">
    <h3>SHISHI</h3>
    <div class="button-container">
        <button class="info-button" onclick="toggleContent('SHISHI', 'info')">
            <i class="fas fa-info-circle"></i> Thông tin
        </button>
        <button class="info-button" onclick="toggleContent('SHISHI', 'images')">
            <i class="fas fa-images"></i> Hình ảnh
        </button>
          <button onclick="openBookingModal('SHISHI')">Đặt lịch</button>
    </button>
</div>


    <!-- Thông tin chi tiết -->
    <div id="info-SHISHI" style="display: none">
        <h4>Thông tin</h4>
        <div class="info-content">
            <img src="https://i.ibb.co/47Dw4Dt/photo-7-2024-09-20-09-20-50.jpg" alt="Image New 83" class="info-image" style="height: 330px;">
            <div class="info-text">
            
                <style>
                  /* styles.css */
                  .location-info {
                      font-size: 17px;
                      color: #00ff00; /* Màu xanh lá */
                      font-weight: bold;
                  }
                  .info-image { 
                      height: 250px; 
                  }
                  .button-container, .detail-info { 
                      text-align: center; 
                  }
              </style>
              
              <script>
             // Hàm khởi tạo vị trí
             function requestLocation() {
                            if (navigator.geolocation) {
                                // Yêu cầu lấy vị trí của người dùng
                                navigator.geolocation.getCurrentPosition(
                                    (position) => {
                                        const latitude = position.coords.latitude;
                                        const longitude = position.coords.longitude;
                    
                                        // Gọi Kakao Maps API để lấy thông tin khu vực từ vĩ độ và kinh độ
                                        fetch(`https://dapi.kakao.com/v2/local/geo/coord2regioncode.json?x=${longitude}&y=${latitude}`, {
                                            method: 'GET',
                                            headers: {
                                                'Authorization': 'KakaoAK 12873a4a25a298774293ab8c899a1432'  // Thay YOUR_KAKAO_API_KEY bằng API Key thực tế của bạn
                                            }
                                        })
                                        .then(response => response.json())
                                        .then(data => {
                                          if (data.documents && data.documents.length > 0) {
                            const region1 = data.documents[0].region_1depth_name;  // Quận hoặc khu vực
                            const region2 = data.documents[0].region_2depth_name;  // Thị trấn hoặc xã
                            const region3 = data.documents[0].region_3depth_name || "Không xác định";  // Khu vực nhỏ hơn
                    
                                        // Hiển thị kết quả
                                        document.getElementById('location-range-SHISHI').textContent = `Vị trí của bạn: ${region1} - ${region2} - ${region3}`;
                                    } else {
                                        document.getElementById('location-range-SHISHI').textContent = "Đang xác định";
                                    }
                                })
                                .catch(err => {
                                    console.error("Lỗi khi lấy vị trí:", err);
                                    document.getElementById('location-range-SHISHI').textContent = "Lỗi khi lấy thông tin vị trí.";
                                });
                            },
                            (error) => {
                                console.error("Lỗi khi lấy vị trí:", error);
                                alert("Không thể lấy vị trí. Vui lòng kiểm tra cài đặt vị trí của bạn.");
                            }
                        );
                    } else {
                        alert("Trình duyệt của bạn không hỗ trợ Geolocation.");
                    }
                }
            
                // Gọi hàm yêu cầu vị trí khi trang được tải
                requestLocation();
            </script>
              
              <!-- HTML phần tử hiển thị vị trí -->
              <div class="location-info">
                  <span id="location-range-SHISHI">Đang xác định</span>
              </div>
              
                <button onclick="showInputBox('SHISHI', 'phone')">SDT</button>

<button onclick="showInputBox('SHISHI', 'telegram')">Telegram</button>
                <p><i class="fas fa-clock"></i> <strong>Thời gian gia nhập:</strong> 22/06/2024 13:17</p>
                <i class="fas fa-user"></i> Hoạt động: <span class="active-status">Đang hoạt động</span>
                        </p>
                      </div>
                  </div>

                  <div id="bio-SHISHI" style="display: block;">
                    <h4>Giới thiệu</h4>
                    <p>
                        Nếu kiếm tìm một hotgirl sở hữu body đẹp chuẩn từng cm như thế này có lẽ sẽ phải chờ dài dài mới tìm được</p>
                    <p>Và những ai được lên giường với bé chắc chắn cũng sẽ có kết luận giống như nhau</p>
                <p>Một bé tuyệt vời mà phải rất lâu mới lại sản sinh ra được</p>
            <p>Sở hữu chiều cao lí tưởng cùng đôi chân dài như kiếm nhật,một bộ ngực quá ngon,mông cong và tròn hết mức</p>
            <p>Ai yêu thích cái đẹp đắm say này chỉ cần lên giường một lần thôi thì chắc chắn đã nghiền luôn rồi
        </p>
        <p><i class="fas fa-birthday-cake"></i> <strong>Năm sinh:</strong> 2002</p>
        <p><i class="fas fa-ruler-vertical"></i> <strong>Cao (cm):</strong> 163</p>
        <p><i class="fas fa-weight-hanging"></i> <strong>Nặng (kg):</strong> 48</p>
        <p><i class="fas fa-tape"></i> <strong>Vòng 1 (cm):</strong> 88</p>
        <p><i class="fas fa-tape"></i> <strong>Vòng 2 (cm):</strong> 60</p>
        <p><i class="fas fa-tape"></i> <strong>Vòng 3 (cm):</strong> 90</p>
        <p><i class="fas fa-smile"></i> <strong>Khuôn mặt:</strong> Thanh tú, đôi môi quyến rũ</p>
       <p><i class="fas fa-eye"></i> <strong>Nhận dạng:</strong> Vóc dáng nhỏ nhắn, dễ thương</p>
        <p><i class="fas fa-clock"></i> <strong>Hoạt động:</strong> Thường xuyên</p>
    </div>
</div>

    <div id="review-container-SHISHI" class="review-section">
    <h4>Đánh giá của bạn cho SHISHI</h4>
    <div class="stars">
        <span class="star" onclick="rateStar('SHISHI', 1)">&#9733;</span>
        <span class="star" onclick="rateStar('SHISHI', 2)">&#9733;</span>
        <span class="star" onclick="rateStar('SHISHI', 3)">&#9733;</span>
        <span class="star" onclick="rateStar('SHISHI', 4)">&#9733;</span>
        <span class="star" onclick="rateStar('SHISHI', 5)">&#9733;</span>
    </div>
</div>

       
<script>
   
   function rateStar(character, star) {
    const result = document.getElementById(`rating-result-${character}`);

    if (result) {
        // Hiển thị thông báo đánh giá
        result.innerText = `Bạn đã đánh giá ${star} sao cho ${character}!`;

        // Sau 3 giây, hiển thị thông báo cảm ơn và ẩn đi sau đó
        setTimeout(() => {
            result.innerText = `Cảm ơn bạn đã đánh giá cho ${character}. Mỗi lượt đánh giá của bạn góp phần thay đổi thứ hạng của cô ấy! Chỉ tính lần đầu trong ngày ❤️`;

            // Ẩn thông báo sau thêm 2 giây nữa
            setTimeout(() => {
                result.innerText = ''; // Xóa nội dung để ẩn đi
                result.style.display = 'none'; // Ẩn phần tử
            }, 2000);
        }, 3000);
    } else {
        console.error("Không tìm thấy phần tử kết quả đánh giá!");
    }
}

// Tạo phần tử để hiển thị kết quả đánh giá trong HTML (nếu chưa có)
document.querySelectorAll('.review-section').forEach(section => {
    const character = section.id.split('-')[2]; // Lấy tên nhân vật từ ID
    if (!document.getElementById(`rating-result-${character}`)) {
        const resultElement = document.createElement('p');
        resultElement.id = `rating-result-${character}`;
        section.appendChild(resultElement);
    }
});
    
</script>

<style>
    
    
    .stars {
        font-size: 20px;
        color: #ffcc00;
    }
    .star {
        cursor: pointer;
    }
    .review-section {
    margin-top: 20px;
    padding: 10px;
    color: #ffffff;
    border-radius: 5px;
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
    max-width: 100%; /* Giới hạn chiều rộng */
    overflow: hidden; /* Ngăn nội dung bị tràn ra ngoài */
    box-sizing: border-box; /* Đảm bảo padding không làm thay đổi chiều rộng */
    border: 1px solid #ffffff; /* Viền màu đen */
}
</style>

    <!-- Hình ảnh -->
    <div id="images-SHISHI" style="display: none">
        <h4>Hình ảnh</h4>
        <a href="https://ibb.co/ZJ10XjR"><img src="https://i.ibb.co/ZJ10XjR/photo-1-2024-09-20-09-20-50.jpg" alt="Image New 78" style="height: 190px; width: auto;"></a>
        <a href="https://ibb.co/t4LLCj1"><img src="https://i.ibb.co/t4LLCj1/photo-2-2024-09-20-09-20-50.jpg" alt="Image New 79" style="height: 190px; width: auto;"></a>
        <a href="https://ibb.co/2S6SRxc"><img src="https://i.ibb.co/2S6SRxc/photo-4-2024-09-20-09-20-50.jpg" alt="Image New 80" style="height: 190px; width: auto;"></a>
        <a href="https://ibb.co/0sB1DfR"><img src="https://i.ibb.co/0sB1DfR/photo-5-2024-09-20-09-20-50.jpg" alt="Image New 81" style="height: 190px; width: auto;"></a>
        <a href="https://ibb.co/LdvxcX0"><img src="https://i.ibb.co/LdvxcX0/photo-6-2024-09-20-09-20-50.jpg" alt="Image New 82" style="height: 190px; width: auto;"></a>
        <a href="https://ibb.co/6FjS0GS"><img src="https://i.ibb.co/6FjS0GS/photo-8-2024-09-20-09-20-50.jpg" alt="Image New 84" style="height: 190px; width: auto;"></a>
        <a href="https://ibb.co/BqDCpqz"><img src="https://i.ibb.co/BqDCpqz/photo-9-2024-09-20-09-20-50.jpg" alt="Image New 85" style="height: 190px; width: auto;"></a>
        <a href="https://ibb.co/BjCDR2V"><img src="https://i.ibb.co/BjCDR2V/photo-10-2024-09-20-09-20-50.jpg" alt="Image New 86" style="height: 190px; width: auto;"></a>
        <a href="https://ibb.co/gS8LgCR"><img src="https://i.ibb.co/gS8LgCR/photo-12-2024-09-20-09-20-50.jpg" alt="Image New 88" style="height: 190px; width: auto;"></a>
        <a href="https://ibb.co/yWpP3wN"><img src="https://i.ibb.co/yWpP3wN/photo-13-2024-09-20-09-20-50.jpg" alt="Image New 89" style="height: 190px; width: auto;"></a>
        <a href="https://ibb.co/YLw1YZ6"><img src="https://i.ibb.co/YLw1YZ6/photo-14-2024-09-20-09-20-50.jpg" alt="Image New 90" style="height: 190px; width: auto;"></a>

    </div>

    <!-- Số lượt book -->
    <div id="bookings-SHISHI" style="display: none">
        <h4>Đặt lịch</h4>
        <p><i class="fas fa-calendar-alt"></i> <strong>Vui lòng đăng nhập để đặt lịch</strong></p>
    </div>

    <!-- Giới thiệu -->
    <div id="bio-SHISHI" style="display: none">
        <h4>Giới thiệu</h4>
        <p>
            Shishi là một cô gái cuốn hút với vẻ đẹp tự nhiên và tính cách thân thiện. Cô ấy luôn biết cách làm khách hàng cảm thấy thoải mái và hài lòng.
        </p>
    </div>
</div>







<!-- Chi tiết Quỳnh Anh -->
<div id="detail-QuynhAnh" class="detail-info">
  <h3>Quỳnh Anh</h3>
  <div class="button-container">
    <button class="info-button" onclick="toggleContent('QuynhAnh', 'info')">
      <i class="fas fa-info-circle"></i> Thông tin
    </button>
    <button class="info-button" onclick="toggleContent('QuynhAnh', 'images')">
      <i class="fas fa-images"></i> Hình ảnh
    </button>
    <button onclick="openBookingModal('QuynhAnh')">Đặt lịch</button>
  </div>

  <!-- Thông tin chi tiết -->
  <div id="info-QuynhAnh" style="display: none">
    <h4>Thông tin</h4>
    <div class="info-content">
        <a href="https://i.ibb.co/0hhkDVk/463120465-1066533151802499-8148182830936919702-n.jpg"><img src="https://i.ibb.co/0hhkDVk/463120465-1066533151802499-8148182830936919702-n.jpg" alt="Image 14" style="height: 190px; width: auto;"></a>
        <div class="info-text">
        <p>
          <i class="fas fa-money-bill-wave"></i>
         
        <p>
       
        <p>
          <style>
            /* styles.css */
            .location-info {
                font-size: 17px;
                color: #00ff00; /* Màu xanh lá */
                font-weight: bold;
            }
            .info-image { 
                height: 250px; 
            }
            .button-container, .detail-info { 
                text-align: center; 
            }
        </style>
       <script>
       // Hàm khởi tạo vị trí
       function requestLocation() {
                            if (navigator.geolocation) {
                                // Yêu cầu lấy vị trí của người dùng
                                navigator.geolocation.getCurrentPosition(
                                    (position) => {
                                        const latitude = position.coords.latitude;
                                        const longitude = position.coords.longitude;
                    
                                        // Gọi Kakao Maps API để lấy thông tin khu vực từ vĩ độ và kinh độ
                                        fetch(`https://dapi.kakao.com/v2/local/geo/coord2regioncode.json?x=${longitude}&y=${latitude}`, {
                                            method: 'GET',
                                            headers: {
                                                'Authorization': 'KakaoAK 12873a4a25a298774293ab8c899a1432'  // Thay YOUR_KAKAO_API_KEY bằng API Key thực tế của bạn
                                            }
                                        })
                                        .then(response => response.json())
                                        .then(data => {
                                          if (data.documents && data.documents.length > 0) {
                            const region1 = data.documents[0].region_1depth_name;  // Quận hoặc khu vực
                            const region2 = data.documents[0].region_2depth_name;  // Thị trấn hoặc xã
                            const region3 = data.documents[0].region_3depth_name || "Không xác định";  // Khu vực nhỏ hơn
    
                                // Hiển thị kết quả
                                document.getElementById('location-range-QUYNHANH').textContent = `Vị trí của bạn: ${region1} - ${region2} - ${region3}`;
                            } else {
                                document.getElementById('location-range-QUYNHANH').textContent = "Đang xác định";
                            }
                        })
                        .catch(err => {
                            console.error("Lỗi khi lấy vị trí:", err);
                            document.getElementById('location-range-QUYNHANH').textContent = "Lỗi khi lấy thông tin vị trí.";
                        });
                    },
                    (error) => {
                        console.error("Lỗi khi lấy vị trí:", error);
                        alert("Không thể lấy vị trí. Vui lòng kiểm tra cài đặt vị trí của bạn.");
                    }
                );
            } else {
                alert("Trình duyệt của bạn không hỗ trợ Geolocation.");
            }
        }
    
        // Gọi hàm yêu cầu vị trí khi trang được tải
        requestLocation();
    </script>
    
    <!-- HTML phần tử hiển thị vị trí -->
    <div class="location-info">
        <span id="location-range-QUYNHANH">Đang xác định</span>
    </div>
    
        
        <button onclick="showInputBox('QuynhAnh', 'phone')">SDT</button>
        <button onclick="showInputBox('QuynhAnh', 'telegram')">Telegram</button>
        <p>
          <i class="fas fa-clock"></i>
          <strong>Thời gian gia nhập:</strong> 15/08/2024 12:16
        </p>
        <i class="fas fa-user"></i> Hoạt động:
        <span class="active-status">Đang họat động</span>
      </div>
    </div>

    <p>
        Bé như một món quà của tạo hóa,đẹp ko chê được điểm nào</p>
    <p>Body chuẩn đét,có thể đưa em vào đắng cấp chân dài 1m63</p>
<p>Ko một chút mỡ thừa,eo ót đâu ra đấy,3 vòng không chê vào đâu được,hàng sịn 100%</p>
        <p>Ngực đẹp tuyệt hảo,tạo hóa vẽ cho bé cặp bưởi ko ai có thể chê</p>
        <p>Eo thắt đáy lưng ongong,mông tròn căng mấy,mịn màng thơm phức</p>
    <p>Thái độ thì khỏi bàn,ngoan hiền dễ thương,nai tơ ngơ ngác,gọi dạ bảo vâng,thân thiện 
    </p>
    <p><i class="fas fa-birthday-cake"></i> <strong>Năm sinh:</strong> 2002</p>
    <p><i class="fas fa-ruler-vertical"></i> <strong>Cao (cm):</strong> 164</p>
    <p><i class="fas fa-weight-hanging"></i> <strong>Nặng (kg):</strong> 48</p>
    <p><i class="fas fa-tape"></i> <strong>Vòng 1 (cm):</strong> 87</p>
    <p><i class="fas fa-tape"></i> <strong>Vòng 2 (cm):</strong> 59</p>
    <p><i class="fas fa-tape"></i> <strong>Vòng 3 (cm):</strong> 91</p>
    <p>
      <i class="fas fa-smile"></i> <strong>Khuôn mặt:</strong> Đáng yêu, với đôi
      mắt biết nói
    </p>
    <p>
      <i class="fas fa-eye"></i> <strong>Nhận dạng:</strong> Nét đẹp nhẹ nhàng,
      dễ thương và thu hút
    </p>
    <p><i class="fas fa-clock"></i> <strong>Hoạt động:</strong> 24/24</p>
  </div>
     
 
  <!-- Hình ảnh -->
  <div id="images-QuynhAnh" style="display: none">
    <h4>Hình ảnh</h4>
    <a href="https://i.ibb.co/cCfM8t2/309989643-629711185484700-800178790464316697-n.jpg"><img src="https://i.ibb.co/cCfM8t2/309989643-629711185484700-800178790464316697-n.jpg" alt="Image 1" style="height: 190px; width: auto;"></a>
<a href="https://i.ibb.co/fvqkdYG/336259995-154577060807678-8601816291592842410-n.jpg"><img src="https://i.ibb.co/fvqkdYG/336259995-154577060807678-8601816291592842410-n.jpg" alt="Image 2" style="height: 190px; width: auto;"></a>
<a href="https://i.ibb.co/r47Knqx/337389624-587013110135564-3829004120735026130-n.jpg"><img src="https://i.ibb.co/r47Knqx/337389624-587013110135564-3829004120735026130-n.jpg" alt="Image 3" style="height: 190px; width: auto;"></a>
<a href="https://i.ibb.co/z67jQMC/340931419-776721337030997-2865551987934903214-n.jpg"><img src="https://i.ibb.co/z67jQMC/340931419-776721337030997-2865551987934903214-n.jpg" alt="Image 4" style="height: 190px; width: auto;"></a>
<a href="https://i.ibb.co/fNm3d5V/367410131-816286566827160-6359684262952889763-n.jpg"><img src="https://i.ibb.co/fNm3d5V/367410131-816286566827160-6359684262952889763-n.jpg" alt="Image 5" style="height: 190px; width: auto;"></a>
<a href="https://i.ibb.co/42SRH5R/383214997-837770018012148-1280788975135102072-n.jpg"><img src="https://i.ibb.co/42SRH5R/383214997-837770018012148-1280788975135102072-n.jpg" alt="Image 6" style="height: 190px; width: auto;"></a>
<a href="https://i.ibb.co/cYbqdZc/384235372-839434814512335-2260972901569626098-n.jpg"><img src="https://i.ibb.co/cYbqdZc/384235372-839434814512335-2260972901569626098-n.jpg" alt="Image 7" style="height: 190px; width: auto;"></a>
<a href="https://i.ibb.co/92FXzHs/387729334-845115860610897-2354261134729548408-n.jpg"><img src="https://i.ibb.co/92FXzHs/387729334-845115860610897-2354261134729548408-n.jpg" alt="Image 8" style="height: 190px; width: auto;"></a>
<a href="https://i.ibb.co/Ss5ny1N/405306079-871290721326744-7522073540435670885-n.jpg"><img src="https://i.ibb.co/Ss5ny1N/405306079-871290721326744-7522073540435670885-n.jpg" alt="Image 9" style="height: 190px; width: auto;"></a>
<a href="https://i.ibb.co/MhXrFMZ/441602376-970638008058681-8481165972533691356-n.jpg"><img src="https://i.ibb.co/MhXrFMZ/441602376-970638008058681-8481165972533691356-n.jpg" alt="Image 11" style="height: 190px; width: auto;"></a>
<a href="https://i.ibb.co/p3sKK5S/454503517-1020509216404893-1431358853470073923-n.jpg"><img src="https://i.ibb.co/p3sKK5S/454503517-1020509216404893-1431358853470073923-n.jpg" alt="Image 12" style="height: 190px; width: auto;"></a>
<a href="https://i.ibb.co/Jm6jkS1/456315582-1027932035662611-7804666417740511200-n.jpg"><img src="https://i.ibb.co/Jm6jkS1/456315582-1027932035662611-7804666417740511200-n.jpg" alt="Image 13" style="height: 190px; width: auto;"></a>
<a href="https://i.ibb.co/0hhkDVk/463120465-1066533151802499-8148182830936919702-n.jpg"><img src="https://i.ibb.co/0hhkDVk/463120465-1066533151802499-8148182830936919702-n.jpg" alt="Image 14" style="height: 190px; width: auto;"></a>
    
    
  
  </div>


  <div id="review-container-QuynhAnh" class="review-section">
    <h4>Đánh giá của bạn cho Quỳnh Anh</h4>
    <div class="stars">
      <span class="star" onclick="rateStar('QuynhAnh', 1)">&#9733;</span>
      <span class="star" onclick="rateStar('QuynhAnh', 2)">&#9733;</span>
      <span class="star" onclick="rateStar('QuynhAnh', 3)">&#9733;</span>
      <span class="star" onclick="rateStar('QuynhAnh', 4)">&#9733;</span>
      <span class="star" onclick="rateStar('QuynhAnh', 5)">&#9733;</span>
    </div>
  </div>
  <script>
   
    function rateStar(character, star) {
     const result = document.getElementById(`rating-result-${character}`);
 
     if (result) {
         // Hiển thị thông báo đánh giá
         result.innerText = `Bạn đã đánh giá ${star} sao cho ${character}!`;
 
         // Sau 3 giây, hiển thị thông báo cảm ơn và ẩn đi sau đó
         setTimeout(() => {
             result.innerText = `Cảm ơn bạn đã đánh giá cho ${character}. Mỗi lượt đánh giá của bạn góp phần thay đổi thứ hạng của cô ấy! Chỉ tính lần đầu trong ngày ❤️`;
 
             // Ẩn thông báo sau thêm 2 giây nữa
             setTimeout(() => {
                 result.innerText = ''; // Xóa nội dung để ẩn đi
                 result.style.display = 'none'; // Ẩn phần tử
             }, 2000);
         }, 3000);
     } else {
         console.error("Không tìm thấy phần tử kết quả đánh giá!");
     }
 }
 
 // Tạo phần tử để hiển thị kết quả đánh giá trong HTML (nếu chưa có)
 document.querySelectorAll('.review-section').forEach(section => {
     const character = section.id.split('-')[2]; // Lấy tên nhân vật từ ID
     if (!document.getElementById(`rating-result-${character}`)) {
         const resultElement = document.createElement('p');
         resultElement.id = `rating-result-${character}`;
         section.appendChild(resultElement);
     }
 });
</script>
  <!-- Số lượt book -->
  <div id="bookings-QuynhAnh" style="display: none">
    <h4>Đặt lịch</h4>
    <p>
      <i class="fas fa-calendar-alt"></i>
      <strong>Vui lòng đăng nhập để đặt lịch</strong>
    </p>
  </div>

  <!-- Giới thiệu -->
  <div id="bio-QuynhAnh" style="display: none">
    <h4>Giới thiệu</h4>
    <p>
      Quỳnh Anh luôn tạo ra những trải nghiệm đáng nhớ với sự chuyên nghiệp và
      thân thiện
    </p>
  </div>
</div>




<!-- Chi tiết Chang -->
<div id="detail-Chang" class="detail-info">
    <h3>Chang</h3>
    <div class="button-container">
      <button class="info-button" onclick="toggleContent('Chang', 'info')">
        <i class="fas fa-info-circle"></i> Thông tin
      </button>
      <button class="info-button" onclick="toggleContent('Chang', 'images')">
        <i class="fas fa-images"></i> Hình ảnh
      </button>
      <button onclick="openBookingModal('Chang')">Đặt lịch</button>
    </div>
  
    <!-- Thông tin chi tiết -->
    <div id="info-Chang" style="display: none">
      <h4>Thông tin</h4>
      <div class="info-content">
        <a href="https://ibb.co/khjQRP5"><img src="https://i.ibb.co/khjQRP5/465168800-1097488541723717-3663567964369007810-n.jpg" alt="Image 8" style="height: 250px; width: auto;"></a>
        <div class="info-text">
          <p>
            <i class="fas fa-money-bill-wave"></i>
      
         
         
          </p>

           
            <style>
              /* styles.css */
              .location-info {
                  font-size: 17px;
                  color: #ff0000; /* Màu xanh lá */
                  font-weight: bold;
              }
              .info-image { 
                  height: 250px; 
              }
              .button-container, .detail-info { 
                background: #000000;
                color: #ffffff; /* Màu chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
        padding: 10px 20px;
    border-radius: 20px;
  

    cursor: pointer;
    


}
          </style>
          
          <script>
              // Hàm khởi tạo vị trí
              function requestLocation() {
                            if (navigator.geolocation) {
                                // Yêu cầu lấy vị trí của người dùng
                                navigator.geolocation.getCurrentPosition(
                                    (position) => {
                                        const latitude = position.coords.latitude;
                                        const longitude = position.coords.longitude;
                    
                                        // Gọi Kakao Maps API để lấy thông tin khu vực từ vĩ độ và kinh độ
                                        fetch(`https://dapi.kakao.com/v2/local/geo/coord2regioncode.json?x=${longitude}&y=${latitude}`, {
                                            method: 'GET',
                                            headers: {
                                                'Authorization': 'KakaoAK 12873a4a25a298774293ab8c899a1432'  // Thay YOUR_KAKAO_API_KEY bằng API Key thực tế của bạn
                                            }
                                        })
                                        .then(response => response.json())
                                        .then(data => {
                                          if (data.documents && data.documents.length > 0) {
                            const region1 = data.documents[0].region_1depth_name;  // Quận hoặc khu vực
                            const region2 = data.documents[0].region_2depth_name;  // Thị trấn hoặc xã
                            const region3 = data.documents[0].region_3depth_name || "Không xác định";  // Khu vực nhỏ hơn
                                          // Hiển thị thông tin thị trấn và quận bằng tiếng Hàn
                                          document.getElementById('location-range-CHANG').textContent = `${town} (${data.results[0].components.town}) - ${district} (${data.results[0].components.district})`;
                                      } else {
                                          document.getElementById('location-range-CHANG').textContent = "Đang xác định";
                                      }
                                  })
                                  .catch(err => {
                                      console.error("Error getting location:", err);
                                      document.getElementById('location-range-CHANG').textContent = "Lỗi khi lấy vị trí.";
                                  });
                          },
                          (error) => {
                              console.error("Geolocation error:", error);
                              alert("Không thể lấy vị trí. Vui lòng kiểm tra cài đặt vị trí của bạn.");
                          }
                      );
                  } else {
                      alert("Trình duyệt của bạn không hỗ trợ Geolocation.");
                  }
              }
          
              // Gọi hàm yêu cầu vị trí khi trang được tải
              requestLocation();
          </script>
          
          <!-- HTML phần tử hiển thị vị trí -->
          <div class="location-info">
              <span id="location-range-CHANG">Đang xác định</span>
          </div>
          
  
          <button onclick="showInputBox('Chang', 'phone')">SDT</button>
    
          <button onclick="showInputBox('Chang', 'telegram')">Telegram</button>
          <p>
            <i class="fas fa-clock"></i>
            <strong>Thời gian gia nhập:</strong> 13/08/2024 15:16
          </p>
          <i class="fas fa-user"></i> Hoạt động:
          <span class="active-status">Đang hoạt động</span>
        </div>
      </div>
  
      <h4>Giới thiệu</h4>
      <p>
        Gương mặt yêu kiều, xinh xắn,bộ ngực căng tròn,hừng hực sức sống tuổi thanh xuân</p>
    <p>Vú to,mông mẩy và đầy đam mê,cảm xúc khi làm tình</p>
        <p>Hãy thử nếm thử hương vị của ái tình với một hot gơ tuyệt vời này sẽ có một cảm giác cực kỳ thư giãn</p> 
        <p>Cái cảm giác vụng trộm và hừng hực lửa đam mê bên một người tình yêu chiều mình hết mực 
      </p>
      <p><i class="fas fa-birthday-cake"></i> <strong>Năm sinh:</strong> 2000</p>
      <p><i class="fas fa-ruler-vertical"></i> <strong>Cao (cm):</strong> 165</p>
      <p><i class="fas fa-weight-hanging"></i> <strong>Nặng (kg):</strong> 49</p>
      <p><i class="fas fa-tape"></i> <strong>Vòng 1 (cm):</strong> 87</p>
      <p><i class="fas fa-tape"></i> <strong>Vòng 2 (cm):</strong> 59</p>
      <p><i class="fas fa-tape"></i> <strong>Vòng 3 (cm):</strong> 91</p>
      <p><i class="fas fa-smile"></i> <strong>Khuôn mặt:</strong> Đáng yêu, với đôi mắt biết nói</p>
      <p><i class="fas fa-eye"></i> <strong>Nhận dạng:</strong> Nét đẹp nhẹ nhàng, dễ thương và thu hút</p>
      <p><i class="fas fa-clock"></i> <strong>Hoạt động:</strong> 24/24</p>
    </div>
  
    <div id="review-container-Chang" class="review-section">
      <h4>Đánh giá của bạn cho Chang</h4>
      <div class="stars">
        <span class="star" onclick="rateStar('Chang', 1)">&#9733;</span>
        <span class="star" onclick="rateStar('Chang', 2)">&#9733;</span>
        <span class="star" onclick="rateStar('Chang', 3)">&#9733;</span>
        <span class="star" onclick="rateStar('Chang', 4)">&#9733;</span>
        <span class="star" onclick="rateStar('Chang', 5)">&#9733;</span>
      </div>
      
    </div>
    <script>
   
        function rateStar(character, star) {
         const result = document.getElementById(`rating-result-${character}`);
     
         if (result) {
             // Hiển thị thông báo đánh giá
             result.innerText = `Bạn đã đánh giá ${star} sao cho ${character}!`;
     
             // Sau 3 giây, hiển thị thông báo cảm ơn và ẩn đi sau đó
             setTimeout(() => {
                 result.innerText = `Cảm ơn bạn đã đánh giá cho ${character}. Mỗi lượt đánh giá của bạn góp phần thay đổi thứ hạng của cô ấy! Chỉ tính lần đầu trong ngày ❤️`;
     
                 // Ẩn thông báo sau thêm 2 giây nữa
                 setTimeout(() => {
                     result.innerText = ''; // Xóa nội dung để ẩn đi
                     result.style.display = 'none'; // Ẩn phần tử
                 }, 2000);
             }, 3000);
         } else {
             console.error("Không tìm thấy phần tử kết quả đánh giá!");
         }
     }
     
     // Tạo phần tử để hiển thị kết quả đánh giá trong HTML (nếu chưa có)
     document.querySelectorAll('.review-section').forEach(section => {
         const character = section.id.split('-')[2]; // Lấy tên nhân vật từ ID
         if (!document.getElementById(`rating-result-${character}`)) {
             const resultElement = document.createElement('p');
             resultElement.id = `rating-result-${character}`;
             section.appendChild(resultElement);
         }
     });
         
     </script>
    <!-- Hình ảnh -->
    <div id="images-Chang" style="display: none">
      <h4>Hình ảnh</h4>
      <a href="https://ibb.co/KjTFxXs"><img src="https://i.ibb.co/KjTFxXs/430029198-946267713512468-5042154628741578756-n.jpg" alt="Image 1" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/CMzrMHz"><img src="https://i.ibb.co/CMzrMHz/378854303-855617289244178-5284751463597591029-n.jpg" alt="Image 2" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/DCXrwLx"><img src="https://i.ibb.co/DCXrwLx/435893748-973112090828030-3658708461828827600-n.jpg" alt="Image 3" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/HxCvHSL"><img src="https://i.ibb.co/HxCvHSL/448578095-1008821667257072-2805937849532685211-n.jpg" alt="Image 4" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/mcnLQcm"><img src="https://i.ibb.co/mcnLQcm/453099935-1034995834639655-2625415353164096910-n.jpg" alt="Image 5" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/c6LntKm"><img src="https://i.ibb.co/c6LntKm/461048233-1070808574391714-6457504351249761695-n.jpg" alt="Image 6" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/3dCf0NY"><img src="https://i.ibb.co/3dCf0NY/461315968-1072265027579402-2095170161509221025-n.jpg" alt="Image 7" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/R99XhXm"><img src="https://i.ibb.co/R99XhXm/465055380-1097488548390383-6204572662205406771-n.jpg" alt="Image 9" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/sHY4sWp"><img src="https://i.ibb.co/sHY4sWp/465004871-1097488598390378-4886516484980949515-n.jpg" alt="Image 10" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/CvWcC5v"><img src="https://i.ibb.co/CvWcC5v/378778004-855617305910843-333745182071302791-n.jpg" alt="Image 11" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/Qjn0ZYv"><img src="https://i.ibb.co/Qjn0ZYv/452104232-1029202725218966-2860286147676872065-n.jpg" alt="Image 12" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/S3ZZRm8"><img src="https://i.ibb.co/S3ZZRm8/452866837-1031653198307252-4040690016312092931-n.jpg" alt="Image 13" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/sJDf3BT"><img src="https://i.ibb.co/sJDf3BT/453433956-1034997097972862-5183529550957858747-n.jpg" alt="Image 14" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/MBCVy8F"><img src="https://i.ibb.co/MBCVy8F/454575777-1041074547365117-1895654296518936209-n.jpg" alt="Image 15" style="height: 250px; width: auto;"></a>
<a href="https://ibb.co/W6y4q0g"><img src="https://i.ibb.co/W6y4q0g/461048236-1070808604391711-8132402547166610401-n.jpg" alt="Image 16" style="height: 250px; width: auto;"></a>
      <!-- Thêm các hình ảnh khác theo cách tương tự -->
    </div>
  
    <!-- Số lượt book -->
    <div id="bookings-Chang" style="display: none">
      <h4>Đặt lịch</h4>
      <p>
        <i class="fas fa-calendar-alt"></i>
        <strong>Vui lòng đăng nhập để đặt lịch</strong>
      </p>
    </div>
  
    <!-- Giới thiệu -->
    <div id="bio-Chang" style="display: none">
      <h4>Giới thiệu</h4>
      <p>
        Chang luôn tạo ra những trải nghiệm đáng nhớ với sự chuyên nghiệp và thân thiện. Cô ấy là một trong những gương mặt nổi bật nhất tại Diamond Club.
      </p>
    </div>
  </div>




    <script>
        const menuItems = document.querySelectorAll(".menu-item");
        const contents = document.querySelectorAll(".content");
        const allDetails = document.querySelectorAll(".detail-info");

        menuItems.forEach((item) => {
            item.addEventListener("click", () => {
                const target = item.getAttribute("data-target");
                const targetContent = document.getElementById(target);

                // Ẩn tất cả thông tin chi tiết khi chuyển giữa các phần
                allDetails.forEach((div) => {
                    div.style.display = "none"; // Ẩn tất cả các phần chi tiết khác
                });

                contents.forEach((content) => {
                    content.classList.remove("active");
                });
                targetContent.classList.add("active");
            });
        });

        // Hiện thông tin chi tiết cho từng bé
        function showDetails(region) {
            const detailDiv = document.getElementById(`detail-${region}`);
            const allDetails = document.querySelectorAll(".detail-info");
            allDetails.forEach((div) => {
                div.style.display = "none"; // Ẩn tất cả các phần chi tiết khác
            });
            detailDiv.style.display =
                detailDiv.style.display === "block" ? "none" : "block"; // Toggle phần chi tiết
        }

        function showInfo(region) {
            const infoDiv = document.getElementById(`info-${region}`);
            const imagesDiv = document.getElementById(`images-${region}`);
            const bioDiv = document.getElementById(`bio-${region}`);

            infoDiv.style.display = "block"; // Hiện phần info
            imagesDiv.style.display = "none"; // Ẩn phần hình ảnh
            bioDiv.style.display = "none"; // Ẩn phần giới thiệu
        }

        function showImages(region) {
            const infoDiv = document.getElementById(`info-${region}`);
            const imagesDiv = document.getElementById(`images-${region}`);
            const bioDiv = document.getElementById(`bio-${region}`);

            imagesDiv.style.display = "block"; // Hiện phần hình ảnh
            infoDiv.style.display = "none"; // Ẩn phần info
            bioDiv.style.display = "none"; // Ẩn phần giới thiệu
        }
        
    </script>
</body>
</html>


<div class="ranking-container">
    <div class="ranking-header">Bảng Xếp Hạng Tháng 11</div>
    <div class="ranking-controls">
        <button onclick="sortRankings('votes')">Sắp xếp theo Votes</button>
        <button onclick="sortRankings('change')">Sắp xếp theo Thay Đổi</button>
        <button onclick="sortRankings('rating')">Sắp xếp theo Đánh Giá</button>
    </div>
    <div class="ranking-container">
        <ul class="ranking-list" id="ranking-list"></ul>
    </div>
    
</div>
<!-- Thêm CSS -->
<style>
    body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #121212;
            color: #fff;
        }

        .ranking-container {
            max-width: 800px;
            margin: 50px auto;
            background: #1e1e1e;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);
        }

        .ranking-header {
            text-align: center;
            font-size: 24px;
            color: #fff;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
            margin-bottom: 20px;
            text-transform: uppercase;
            font-weight: bold;
        }

        .ranking-controls {
            text-align: center;
            margin-bottom: 20px;
        }

        .ranking-controls button {
            background: #ff6b6b;
            color: #000000;
            border: none;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            border: 1px solid #fff; /* Viền vàng */

            margin: 0 10px;
            transition: background 0.3s ease;
        }

        .ranking-controls button:hover {
            background: #1a1515;
            color: #ffffff;
        }

        .ranking-list {
            list-style: none;
            margin: 0;
            padding: 0;
        }

        .ranking-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px;
            background: #292929;
            border-bottom: 1px solid #444;
            border-radius: 5px;
            margin-bottom: 10px;
            transition: background 0.3s ease, transform 0.3s ease;
        }

        .ranking-item:hover {
            background: #333;
            transform: translateY(-3px);
        }

        .ranking-position {
            font-size: 20px;
            font-weight: bold;
            color: #ffd700;
            width: 40px;
            text-align: center;
            position: relative;
        }
   

        .ranking-avatar {
            width: 70px;
            height: 70px;
            margin: 0 15px;
            border-radius: 10px;
            overflow: hidden;
            border: 2px solid #fff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
        }

        .ranking-avatar img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .ranking-avatar img:hover {
            transform: scale(1.1);
        }

        .ranking-info {
            flex: 1;
        }

        .ranking-name {
            font-size: 18px;
            font-weight: bold;
            margin: 0;
            color: #fff;
        }

        .ranking-likes {
            font-size: 16px;
            color: #ff6b6b;
            display: flex;
            flex-direction: column;
            align-items: flex-start;
        }

        .ranking-likes i {
            margin-right: 5px;
        }

        .ranking-change {
            font-size: 16px;
            font-weight: bold;
            color: #4caf50;
        }

        .ranking-change.negative {
            color: #e53935;
        }

        .ranking-ratings {
            font-size: 14px;
            color: #bbb;
     }        
/* Định nghĩa chung cho biểu tượng đặc biệt */
.special-icon {
    width: 30px;
    height: 30px;
    background-size: contain;
    background-repeat: no-repeat;
    display: inline-block;
    margin-left: 5px;
    vertical-align: middle;
}

/* Vương miện cho Top 1 */
.ranking-position.top-1 .special-icon {
    background-image: url('https://i.ibb.co/wSQJfrg/64ec2c8fedc1c.png');
}

/* Ngôi sao cho Top 2 */
.ranking-position.top-2 .special-icon {
    background-image: url('https://i.ibb.co/HgdLXyT/671bab6aa4122.png');
}

/* Huy chương cho Top 3 */
.ranking-position.top-3 .special-icon {
    background-image: url('https://i.ibb.co/7pykV2z/2055905-removebg-preview.png');
}

</style>
<script>



   const rankings = [
    { position: 1, name: "Chang", likes: 26035, change: 4.29, ratings: 9450, avatar: "https://i.ibb.co/CMzrMHz/378854303-855617289244178-5284751463597591029-n.jpg", rating: 5 },
    { position: 2, name: "Gia Hân", likes: 20340, change: -3.21, ratings: 6146, avatar: "https://i.ibb.co/1TRWLYN/448066649-3778888015771584-1306281735794756456-n.jpg", rating: 4.5 },
    { position: 3, name: "Thúy Vy", likes: 19021, change: 5.56, ratings: 4753, avatar: "https://i.ibb.co/vXtLZBD/photo-2022-12-27-10-55-09.jpg", rating: 4.5 },
    { position: 4, name: "JenNi", likes: 17730, change: -3.72, ratings: 4012, avatar: "https://i.ibb.co/fv3cs1W/461767365-18326685538194877-298191053835901842-n.jpg", rating: 4.5 },
    { position: 5, name: "An Nhi", likes: 15136, change: 0.62, ratings: 3590, avatar: "https://i.ibb.co/QXDZgJ1/reup-be-ana-pga-chuan-mat-xinh-body-dep-vu-to-dam-tiep-cac-boss-3113753-original.jpg", rating: 4 },
    { position: 6, name: "Hạ Vũ", likes: 14373, change: 0.33, ratings: 2567, avatar: "https://i.ibb.co/t33RTG6/398466992-1133936840908077-2787695977615575197-n.jpg", rating: 4 },
    { position: 7, name: "Anh Thư", likes: 12346, change: -0.87, ratings: 2244, avatar: "https://i.ibb.co/P91y2Dp/photo-2024-08-15-12-49-14.jpg", rating: 4 },
    { position: 8, name: "Yuna", likes: 10332, change: 1.38, ratings: 1670, avatar: "https://i.ibb.co/7gT51Mr/458315545-2877650585726341-611499681677932774-n.jpg", rating: 3.5 },
    { position: 9, name: "Lan Vy", likes: 9317, change: -0.73, ratings: 1341, avatar: "https://i.ibb.co/GWmbNJt/426318819-1098436931490982-4805370043843722560-n.jpg", rating: 3.5 },
    { position: 10, name: "Huyền Anh", likes: 8295, change: -0.67, ratings: 1084, avatar: "https://i.ibb.co/YpKMmTm/photo-2022-12-22-09-00-19.jpg", rating: 3 },
];

rankings.forEach((item, index) => {
    const specialClass = item.position === 1 ? "top-1"
        : item.position === 2 ? "top-2"
        : item.position === 3 ? "top-3" : "";
    });      

const rankingList = document.getElementById("ranking-list");

// Hàm tăng số liệu ngẫu nhiên
function updateDynamicData() {
    rankings.forEach(item => {
        const likeChange = Math.floor(Math.random() * 5) + 1; // Tăng 1-5 lượt thích
        const percentChange = Math.random() * 0.1; // Tăng chậm 0.1%
        item.likes += likeChange;
        item.change += percentChange;
        item.ratings += Math.floor(Math.random() * 2); // Thêm số lượt đánh giá
    });
    renderRankings();
}

// Hàm tạo hiệu ứng động
function animateValue(element, start, end, duration) {
    let startTime = null;

    function step(currentTime) {
        if (!startTime) startTime = currentTime;
        const progress = Math.min((currentTime - startTime) / duration, 1);
        const value = Math.floor(progress * (end - start) + start);
        element.textContent = value;

        if (progress < 1) {
            requestAnimationFrame(step);
        }
    }

    requestAnimationFrame(step);
}

function renderRankings() {
    rankingList.innerHTML = ""; // Xóa nội dung cũ

    rankings.forEach((item) => {
        const specialClass = item.position === 1 ? "top-1"
            : item.position === 2 ? "top-2"
            : item.position === 3 ? "top-3" : "";

        const listItem = document.createElement("li");
        listItem.className = `ranking-item ${specialClass}`;
        listItem.innerHTML = `
            <div class="ranking-position">
                ${item.position}
                ${specialClass ? '<div class="special-icon"></div>' : ""}
            </div>
            <div class="ranking-avatar">
                <img src="${item.avatar}" alt="${item.name}">
            </div>
            <div class="ranking-info">
                <p class="ranking-name">${item.name}</p>
                <div class="ranking-likes">
                    <i class="fas fa-heart"></i> 
                    <span class="likes-count">${item.likes}</span> Thích
                    <span class="ranking-ratings">${item.ratings} lượt đánh giá</span>
                </div>
            </div>
            <div class="ranking-change ${item.change < 0 ? "negative" : ""}">
                <span class="change-count">${item.change.toFixed(2)}</span>% 
            </div>
        `;
        rankingList.appendChild(listItem);
    });
}
function sortRankings(criteria) {
    rankings.sort((a, b) => {
        if (criteria === "likes") return b.likes - a.likes;
        if (criteria === "change") return b.change - a.change;
        if (criteria === "rating") return b.rating - a.rating;
        return 0;
    });
    renderRankings();
}

document.addEventListener("DOMContentLoaded", () => {
    renderRankings();
    setInterval(updateDynamicData, 3000); // Cập nhật số liệu mỗi 3 giây
});
</script>
</body>
</html>


<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
    <title>Được yêu thích nhất</title>
    <style>
        /* CSS tổng thể */
        body {
            font-family: "Poppins", sans-serif;
            margin: -20;
            padding: 0;
            background-color: #000000; /* Màu nền nút cam đậm */
            box-shadow: 0 4px 8px #000000;
            color: #ffffff; /* Màu chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
        }
        
        /* Căn chỉnh container chính */
        .container {
            width: 100%;
            margin: 0 auto;
            padding: 20px;
            background-color: #000000; /* Màu nền nút cam đậm */
        }

      

        /* Định dạng tiêu đề */
        #hoa-khoi-section h2 {
            font-size: 20px;
            ransition: background-color 0.3s, transform 0.3s, box-shadow 0.3s;
            padding: 10px; /* Khoảng cách trong */
            text-align: center; /* Căn giữa tiêu đề */
            animation: glowing 1.5s infinite; /* Hiệu ứng phát sáng */
           
            color: #000000; /* Màu chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */

            border-radius: 10px;
        }


.login-btns {
    position: absolute;
    top: 20px;
    margin-right: 40px; /* Thêm khoảng cách bằng margin */
}


@keyframes fadeIn {
  0% { opacity: 0; }
  100% { opacity: 1; }
}

#hoa-khoi-section h2:hover {
    background-color: #ffffff; /* Màu nền khi hover */
    color: #000000; /* Màu chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
}

.sub-title {
    font-size: 24px;
    color: #1a1a1a; /* Nền đen */ /* Màu chữ trắng */
    text-align: center;
    margin: 20px 0;
}

.sub-title:first-of-type {
    color: #ff3d00; /* Màu chữ trắng cho tiêu đề phụ đầu tiên */
}

.sub-title:last-of-type {
    color: #ff3d00; /* Màu hồng cam phù hợp với nền cam đào */
}





.statistics-widget {
    background: linear-gradient(135deg, #f7a7c5, #d14d83); /* Nền hồng gradient */
    padding: 10px;
    transition: background-color 0.3s, transform 0.3s, box-shadow 0.3s;
   
    width: 100px;
    margin: 10px auto;
    text-align: center;
    position: relative;
    top: -70px;
    border: 2px solid #000000; /* Viền bạc */
    border-radius: 20px;
    font-weight: bold;
    background-color: #1a1a1a; /* Nền đen */
    cursor: pointer;
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
    
}

.statistics-widget h4 {
    margin: 0 0 15px 0;
    font-size: 20px;
    color: #000000; /* Màu chữ trắng nổi bật */
    
}

.statistics-widget ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
    color: #000000; /* Màu hồng cam cho số liệu */
    
}

.statistics-widget li {
    font-size: 18px;
    margin-bottom: 10px;
}

.statistics-widget strong {

    color: #00ff22; /* Chữ vàng */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
    border-radius: 20px;
}

.statistics-widget ul li::before {
    content: "\f0da"; /* Biểu tượng */
    font-family: FontAwesome;
    margin-right: 10px;
    color: #FFD700; /* Chữ vàng */
    border-radius: 10px; /* Bo tròn các góc */
}


@media (max-width: 600px) {
    .statistics-widget {
        width: 90%; /* Đảm bảo hiển thị đẹp trên thiết bị nhỏ */

        @keyframes slide {
0% {
transform: translateX(0); /* Bắt đầu từ vị trí ban đầu */
}
100% {
transform: translateX(-100%); /* Cuộn đến hết bộ ảnh */
}
@keyframes slide {
    0% {
        transform: translate3d(0, 0, 0); /* Sử dụng translate3d */
    }
    100% {
        transform: translate3d(-100%, 0, 0); /* Cuộn đến hết bộ ảnh */
    }
}
}
    }
}/* CSS cho các thiết bị có chiều rộng màn hình nhỏ hơn 600px */
@media (max-width: 600px) {
    .slider-images {
        animation: slide 20s linear infinite; /* Điều chỉnh tốc độ cuộn cho thiết bị di động */
    }
}
@media (max-width: 600px) {
    .slider-images img {
        width: 120px; /* Giảm kích thước hình ảnh trên điện thoại */
        margin-right: 5px; /* Giảm khoảng cách giữa các hình ảnh */
    }
}


        /* Cài đặt cho slider */
        .slider {
            width: 100%;
            margin: 0 auto;
            overflow: hidden;
            padding: 10px 0;
        }
        
        * Khung chứa các hình ảnh */
.slider {
overflow: hidden; /* Ẩn các hình ảnh khi chúng cuộn ra khỏi khung nhìn */
width: 400%; /* Chiều rộng khung chứa */
}

/* Các hình ảnh sẽ được cuộn */
.slider-images {
display: flex;
width: 400%; /* Gấp đôi để chứa cả 2 bộ ảnh */
animation: slide 50s linear infinite; /* Animation cuộn với thời gian 30 giây */
}

/* Cài đặt cho hình ảnh */
.slider-images img {
width: 150px; /* Đặt chiều rộng của mỗi ảnh */
height: auto; /* Giữ tỉ lệ hình ảnh */
margin-right: -15px; /* Khoảng cách giữa các hình ảnh */
border-radius: 5px; /* Bo góc ảnh */
}

{
    font-size: 20px; /* Kích thước chữ của tiêu đề */
    background: linear-gradient(45deg, #ff79a1, #ffdd40); /* Hiệu ứng gradient từ hồng sang vàng */
    -webkit-background-clip: text; /* Hiển thị gradient trên văn bản */
    
    text-align: center; /* Căn giữa tiêu đề */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Tạo đổ bóng cho tiêu đề */
    border: 2px solid #ff79a1; /* Tạo viền 3px với màu hồng */
}


        @keyframes slideRightToLeft {
    0% {
        transform: translateX(100%);
    }
    100% {
        transform: translateX(-100%);
        animation-timing-function: ease-in-out; /* Chuyển động mượt hơn */
    }


    }
    .statistics-widget h4 {
    margin: 0 0 10px 0;
    font-size: 16px;
    color: #000000; /* Chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
    border-radius: 20px;
    

}

.statistics-widget ul {
    list-style: none;
    padding: 0;
    margin: 0;
}

.statistics-widget li {
    font-size: 14px;
    margin-bottom: 5px;
}

.statistics-widget strong {
 
    border-radius: 5px;
}
    </style>
    
</head>
<body>

 <!-- 4 nút phim 18+ hiển thị sau khi nhấn vào Phim 18+ -->
 <div id="submenu-phim-18" class="submenu" style="display:none;">
    <button class="phim-btn" onclick="window.open('https://quatvn.fit/onlyfans-vietnam/', '_blank')">Phim 18+ Việt Nam</button>
    <button class="phim-btn" onclick="window.open('https://quatvn.fit/cn/', '_blank')">Phim 18+ Trung</button>
    <button class="phim-btn" onclick="window.open('https://quatvn.fit/us/', '_blank')">Phim 18+ U.S</button>
    <button class="phim-btn" onclick="window.open('https://quatvn.fit/kr/', '_blank')">Phim 18+ Hàn</button>
    <button class="phim-btn" onclick="window.open('https://quatvn.fit/jp/', '_blank')">Phim 18+ Nhật Bản (JAV)</button>
    <button class="phim-btn" onclick="window.open">Gái Việt Du học sinh (Member Vip 💎)</button>
    <button class="phim-btn" onclick="window.open('https://quatvn.fit/onlyfans-thailand/', '_blank')">Phim 18+ Khác</button>
</div>

</div>
<!-- Script để ẩn/hiện 4 nút phim 18+ -->
<script>
    function toggleSubmenu() {
        var submenu = document.getElementById("submenu-phim-18");
        if (submenu.style.display === "none" || submenu.style.display === "") {
            submenu.style.display = "flex";
        } else {
            submenu.style.display = "none";
        }
    }
</script>

<!-- CSS cho các nút phim 18+ -->
<style>
.submenu {
    display: none;
    flex-wrap: wrap; /* Cho phép nút xuống hàng khi không đủ không gian */
    gap: 10px;
}

.phim-btn {
    font-size: 13px;
    padding: 5px 9px;
    background: #000000;
    color: #ffffff; /* Chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5); /* Đổ bóng cho chữ */
    border-radius: 5px;
    font-weight: 750; /* Chữ đậm nhưng nhẹ hơn */
    cursor: pointer;
    flex-basis: 22%; /* Chiều rộng mỗi nút */
    text-align: center;
    box-sizing: border-box;
    border: 2px solid #C0C0C0; /* Viền bạc */
    transition: background-color 0.3s ease, transform 0.3s ease; /* Hiệu ứng chuyển đổi */
}

.phim-btn:hover {
    background-color: #ffffff; /* Màu nền khi hover */
    transform: scale(1.05); /* Phóng to nhẹ khi hover */
}
</style>
  
</body>

<!-- Mục Được Yêu Thích Nhất  -->
<div class="container">
    <div id="hoa-khoi-section">
        <h2>PREVIEW 💋</h2>
        <div class="slider">
            <div class="slider-images-wrapper">
            <div class="slider-images">
                <a href="https://ibb.co/HT7XRt6"><img src="https://i.ibb.co/HT7XRt6/photo-6-2024-10-23-11-52-30.jpg" alt="Image 1" border="0"></a>
                <a href="https://ibb.co/ZgMh5Rz"><img src="https://i.ibb.co/ZgMh5Rz/photo-15-2024-10-23-11-52-15.jpg" alt="Image 2" border="0"></a>
                <a href="https://ibb.co/hWFT7BW"><img src="https://i.ibb.co/hWFT7BW/photo-19-2024-10-23-11-22-02.jpg" alt="Image 3" border="0"></a>
                <a href="https://ibb.co/FDfxQHd"><img src="https://i.ibb.co/FDfxQHd/photo-22-2024-10-23-11-51-38.jpg" alt="Image 4" border="0"></a>
                <a href="https://ibb.co/g7GNv7g"><img src="https://i.ibb.co/g7GNv7g/photo-2024-08-20-14-51-53.jpg" alt="Image 5" border="0"></a>
                <a href="https://ibb.co/r7SNbfP"><img src="https://i.ibb.co/r7SNbfP/photo-32-2024-10-23-11-52-30.jpg" alt="Image 6" border="0"></a>
                <a href="https://ibb.co/WPSLQyZ"><img src="https://i.ibb.co/WPSLQyZ/photo-43-2024-10-23-11-52-15.jpg" alt="Image 7" border="0"></a>
                <a href="https://ibb.co/26KKrtZ"><img src="https://i.ibb.co/26KKrtZ/photo-50-2024-10-23-11-51-38.jpg" alt="Image 8" border="0"></a>
                <a href="https://ibb.co/L6G6g5k"><img src="https://i.ibb.co/L6G6g5k/photo-80-2024-10-23-11-22-02.jpg" alt="Image 9" border="0"></a>
                <a href="https://ibb.co/LSGs6cV"><img src="https://i.ibb.co/LSGs6cV/photo-83-2024-10-23-11-52-15.jpg" alt="Image 10" border="0"></a>
                <a href="https://ibb.co/WvLsK1R"><img src="https://i.ibb.co/WvLsK1R/photo-96-2024-10-23-11-52-15.jpg" alt="Image 11" border="0"></a>
                <a href="https://ibb.co/mRf4Tps"><img src="https://i.ibb.co/mRf4Tps/photo-98-2024-10-23-11-52-15.jpg" alt="Image 12" border="0"></a>
                <a href="https://ibb.co/1KCVprp"><img src="https://i.ibb.co/1KCVprp/photo-2024-10-17-23-30-54.jpg" alt="Image 13" border="0"></a>
                <a href="https://ibb.co/yVwR18k"><img src="https://i.ibb.co/yVwR18k/photo-2024-10-17-23-32-44.jpg" alt="Image 14" border="0"></a>
                <a href="https://ibb.co/TBKGpDc"><img src="https://i.ibb.co/TBKGpDc/photo-2024-07-26-18-41-01.jpg" alt="Image 15" border="0"></a>
                <a href="https://ibb.co/bHLbVdD"><img src="https://i.ibb.co/bHLbVdD/455691559-122111257202434651-6263614150393024155-n.jpg" alt="Image 16" border="0"></a>
                <a href="https://ibb.co/VYSyXSj"><img src="https://i.ibb.co/VYSyXSj/photo-2024-09-05-18-37-46.jpg" alt="Image 17" border="0"></a>
                <a href="https://ibb.co/QXDZgJ1"><img src="https://i.ibb.co/QXDZgJ1/reup-be-ana-pga-chuan-mat-xinh-body-dep-vu-to-dam-tiep-cac-boss-3113753-original.jpg" alt="Image 18" border="0"></a>
                <a href="https://ibb.co/vhc79wJ"><img src="https://i.ibb.co/vhc79wJ/taoanhdep-lam-net-anh-22071.jpg" alt="Image 19" border="0"></a>
                <a href="https://ibb.co/rQpDrXj"><img src="https://i.ibb.co/rQpDrXj/taoanhdep-lam-net-anh-84350.jpg" alt="Image 20" border="0"></a>
                <a href="https://ibb.co/NncCRYJ"><img src="https://i.ibb.co/NncCRYJ/photo-9-2024-10-23-11-52-15.jpg" alt="Image 21" border="0"></a>
                <a href="https://ibb.co/B4SWLf2"><img src="https://i.ibb.co/B4SWLf2/photo-4-2024-10-23-11-52-15.jpg" alt="Image 22" border="0"></a>
                <a href="https://ibb.co/3TBjJrS"><img src="https://i.ibb.co/3TBjJrS/photo-3-2024-10-23-11-52-15.jpg" alt="Image 23" border="0"></a>
                <a href="https://ibb.co/mNNL9h6"><img src="https://i.ibb.co/mNNL9h6/photo-8-2024-10-23-11-51-38.jpg" alt="Image 24" border="0"></a>
                <a href="https://ibb.co/5RBJHX0"><img src="https://i.ibb.co/5RBJHX0/photo-2024-09-05-18-25-49.jpg" alt="Image 25" border="0"></a>
                <a href="https://ibb.co/c10Lbzk"><img src="https://i.ibb.co/c10Lbzk/photo-2024-09-05-18-37-42-2.jpg" alt="Image 26" border="0"></a>
                <a href="https://ibb.co/q7kXCmx"><img src="https://i.ibb.co/q7kXCmx/photo-2024-09-05-18-37-43.jpg" alt="Image 27" border="0"></a>
                <a href="https://ibb.co/HrWycSc"><img src="https://i.ibb.co/HrWycSc/photo-2024-09-05-18-35-45-4.jpg" alt="Image 28" border="0"></a>
                <a href="https://ibb.co/xXN7XND"><img src="https://i.ibb.co/xXN7XND/photo-2024-09-05-18-37-46.jpg" alt="Image 29" border="0"></a>
                <a href="https://ibb.co/wRg0Fxr"><img src="https://i.ibb.co/wRg0Fxr/photo-2024-09-05-18-37-54.jpg" alt="Image 30" border="0"></a>
                <a href="https://ibb.co/hVvFThy"><img src="https://i.ibb.co/hVvFThy/photo-2024-07-08-15-35-10.jpg" alt="Image 31" border="0"></a>
                <a href="https://ibb.co/XVFxydz"><img src="https://i.ibb.co/XVFxydz/photo-2024-07-08-18-29-39.jpg" alt="Image 32" border="0"></a>
                <a href="https://ibb.co/C1vzDrm"><img src="https://i.ibb.co/C1vzDrm/photo-2024-07-13-20-02-05.jpg" alt="Image 33" border="0"></a>
                <a href="https://ibb.co/P4N1RxC"><img src="https://i.ibb.co/P4N1RxC/photo-2024-07-16-19-46-04.jpg" alt="Image 34" border="0"></a>
                <a href="https://ibb.co/cbFvT6w"><img src="https://i.ibb.co/cbFvT6w/photo-2024-07-17-21-33-48.jpg" alt="Image 35" border="0"></a>
                <a href="https://ibb.co/mDgpphk"><img src="https://i.ibb.co/mDgpphk/photo-2024-07-17-22-06-53.jpg" alt="Image 36" border="0"></a>
                <a href="https://ibb.co/fxYN92r"><img src="https://i.ibb.co/fxYN92r/photo-2024-07-26-20-22-05.jpg" alt="Image 37" border="0"></a>
                <a href="https://ibb.co/hfPm5kQ"><img src="https://i.ibb.co/hfPm5kQ/photo-2024-07-27-19-41-23.jpg" alt="Image 38" border="0"></a>
                <a href="https://ibb.co/6gJpcCv"><img src="https://i.ibb.co/6gJpcCv/photo-2024-08-01-19-45-35.jpg" alt="Image 39" border="0"></a>
                <a href="https://ibb.co/xMgVzrm"><img src="https://i.ibb.co/xMgVzrm/photo-2024-08-02-21-35-06.jpg" alt="Image 40" border="0"></a>
                <a href="https://ibb.co/7SyF1KP"><img src="https://i.ibb.co/7SyF1KP/photo-2024-08-11-13-02-15.jpg" alt="Image 41" border="0"></a>
                <a href="https://ibb.co/7NP8yrr"><img src="https://i.ibb.co/7NP8yrr/photo-2024-08-11-20-22-43.jpg" alt="Image 42" border="0"></a>
                <a href="https://ibb.co/6FSKKz0"><img src="https://i.ibb.co/6FSKKz0/photo-2024-08-12-13-41-26.jpg" alt="Image 43" border="0"></a>
                <a href="https://ibb.co/1RfR70n"><img src="https://i.ibb.co/1RfR70n/photo-2024-08-14-21-11-07.jpg" alt="Image 44" border="0"></a>
                <a href="https://ibb.co/5n5Fvcv"><img src="https://i.ibb.co/5n5Fvcv/photo-2024-08-14-22-24-10.jpg" alt="Image 45" border="0"></a>
                <a href="https://ibb.co/P91y2Dp"><img src="https://i.ibb.co/P91y2Dp/photo-2024-08-15-12-49-14.jpg" alt="Image 46" border="0"></a>
                <a href="https://ibb.co/rpSrxZv"><img src="https://i.ibb.co/rpSrxZv/photo-2024-08-18-18-37-18.jpg" alt="Image 47" border="0"></a>
                <a href="https://ibb.co/bN1JjqW"><img src="https://i.ibb.co/bN1JjqW/photo-2024-08-19-22-58-05.jpg" alt="Image 48" border="0"></a>
                <a href="https://ibb.co/2qwCJnX"><img src="https://i.ibb.co/2qwCJnX/photo-2024-08-23-13-26-54.jpg" alt="Image 49" border="0"></a>
                <a href="https://ibb.co/n7cmdBv"><img src="https://i.ibb.co/n7cmdBv/photo-2024-08-28-15-21-12.jpg" alt="Image 50" border="0"></a>
                <a href="https://ibb.co/m86KxLK"><img src="https://i.ibb.co/m86KxLK/photo-2024-08-29-21-21-48.jpg" alt="Image 51" border="0"></a>
                <a href="https://ibb.co/F0LX904"><img src="https://i.ibb.co/F0LX904/photo-2024-09-02-21-10-06.jpg" alt="Image 52" border="0"></a>
                <a href="https://ibb.co/DDfzdWD"><img src="https://i.ibb.co/DDfzdWD/photo-2024-09-09-13-05-48.jpg" alt="Image 53" border="0"></a>
                <a href="https://ibb.co/nQBW2Nc"><img src="https://i.ibb.co/nQBW2Nc/photo-2024-09-09-13-05-50.jpg" alt="Image 54" border="0"></a>
                <a href="https://ibb.co/2Z6T8pw"><img src="https://i.ibb.co/2Z6T8pw/photo-2024-09-09-20-28-17.jpg" alt="Image 55" border="0"></a>
                <a href="https://ibb.co/Yh4GSS9"><img src="https://i.ibb.co/Yh4GSS9/photo-2024-09-11-17-36-56.jpg" alt="Image 56" border="0"></a>
                <a href="https://ibb.co/X3Vw2Dx"><img src="https://i.ibb.co/X3Vw2Dx/photo-2024-09-11-19-40-50.jpg" alt="Image 57" border="0"></a>
                <a href="https://ibb.co/BNJtPRk"><img src="https://i.ibb.co/BNJtPRk/photo-2024-09-12-18-59-24.jpg" alt="Image 58" border="0"></a>
                <a href="https://ibb.co/S5cZB7m"><img src="https://i.ibb.co/S5cZB7m/419418603-1508797216580744-6598850606428340490-n.jpg" alt="Image 59" border="0"></a>
                <a href="https://ibb.co/qYSb9Mm"><img src="https://i.ibb.co/qYSb9Mm/photo-2024-06-24-20-18-13.jpg" alt="Image 60" border="0"></a>
                <a href="https://ibb.co/zsGMw70"><img src="https://i.ibb.co/zsGMw70/review-of-hay-tim-em-dam-for-reup-be-ana-pga-chuan-mat-xinh-body-dep-vu-to-dam-tiep-cac-boss-3134082.jpg" alt="Image 61" border="0"></a>
                <a href="https://ibb.co/y0ghTLq"><img src="https://i.ibb.co/y0ghTLq/reup-trieu-uyen-cuc-pham-sieu-non-to-nong-bong-ngot-ngao-dang-yeu-3218910-original.jpg" alt="Image 62" border="0"></a>
                <a href="https://ibb.co/ZHt0m10"><img src="https://i.ibb.co/ZHt0m10/reup-trieu-uyen-cuc-pham-sieu-non-to-nong-bong-ngot-ngao-dang-yeu-2970339-original.jpg" alt="Image 63" border="0"></a>
                <a href="https://ibb.co/x1fnZ28"><img src="https://i.ibb.co/x1fnZ28/reup-trieu-uyen-cuc-pham-sieu-non-to-nong-bong-ngot-ngao-dang-yeu-2961977-original.jpg" alt="Image 64" border="0"></a>
                <a href="https://ibb.co/cNswv30"><img src="https://i.ibb.co/cNswv30/review-of-luke-for-sieu-pham-mia-thien-than-2k4-moi-lon-tieu-muoi-douyin-hong-hao-3258387-original.jpg" alt="Image 65" border="0"></a>
                <a href="https://ibb.co/tBvCVwX"><img src="https://i.ibb.co/tBvCVwX/photo-2024-09-05-18-55-28-2.jpg" alt="Image 66" border="0"></a>
                <a href="https://ibb.co/wJcM7dm"><img src="https://i.ibb.co/wJcM7dm/photo-2024-08-19-21-10-58.jpg" alt="Image 67" border="0"></a>
                <a href="https://ibb.co/pX3P1kG"><img src="https://i.ibb.co/pX3P1kG/photo-2024-08-28-19-44-03.jpg" alt="Image 68" border="0"></a>
                <a href="https://ibb.co/TmHHqC7"><img src="https://i.ibb.co/TmHHqC7/photo-2024-09-09-13-05-49.jpg" alt="Image 69" border="0"></a>
                
<!-- Thêm các ảnh khác vào đây -->



  <!-- Lặp lại bộ hình ảnh 1 để tạo hiệu ứng cuộn liên tục -->
  <a href="https://ibb.co/HT7XRt6"><img src="https://i.ibb.co/HT7XRt6/photo-6-2024-10-23-11-52-30.jpg" alt="Image 1" border="0"></a>
<a href="https://ibb.co/ZgMh5Rz"><img src="https://i.ibb.co/ZgMh5Rz/photo-15-2024-10-23-11-52-15.jpg" alt="Image 2" border="0"></a>
<a href="https://ibb.co/hWFT7BW"><img src="https://i.ibb.co/hWFT7BW/photo-19-2024-10-23-11-22-02.jpg" alt="Image 3" border="0"></a>
<a href="https://ibb.co/FDfxQHd"><img src="https://i.ibb.co/FDfxQHd/photo-22-2024-10-23-11-51-38.jpg" alt="Image 4" border="0"></a>
<a href="https://ibb.co/g7GNv7g"><img src="https://i.ibb.co/g7GNv7g/photo-2024-08-20-14-51-53.jpg" alt="Image 5" border="0"></a>
<a href="https://ibb.co/r7SNbfP"><img src="https://i.ibb.co/r7SNbfP/photo-32-2024-10-23-11-52-30.jpg" alt="Image 6" border="0"></a>
<a href="https://ibb.co/WPSLQyZ"><img src="https://i.ibb.co/WPSLQyZ/photo-43-2024-10-23-11-52-15.jpg" alt="Image 7" border="0"></a>
<a href="https://ibb.co/26KKrtZ"><img src="https://i.ibb.co/26KKrtZ/photo-50-2024-10-23-11-51-38.jpg" alt="Image 8" border="0"></a>
<a href="https://ibb.co/L6G6g5k"><img src="https://i.ibb.co/L6G6g5k/photo-80-2024-10-23-11-22-02.jpg" alt="Image 9" border="0"></a>
<a href="https://ibb.co/LSGs6cV"><img src="https://i.ibb.co/LSGs6cV/photo-83-2024-10-23-11-52-15.jpg" alt="Image 10" border="0"></a>
<a href="https://ibb.co/WvLsK1R"><img src="https://i.ibb.co/WvLsK1R/photo-96-2024-10-23-11-52-15.jpg" alt="Image 11" border="0"></a>
<a href="https://ibb.co/mRf4Tps"><img src="https://i.ibb.co/mRf4Tps/photo-98-2024-10-23-11-52-15.jpg" alt="Image 12" border="0"></a>
<a href="https://ibb.co/1KCVprp"><img src="https://i.ibb.co/1KCVprp/photo-2024-10-17-23-30-54.jpg" alt="Image 13" border="0"></a>
<a href="https://ibb.co/yVwR18k"><img src="https://i.ibb.co/yVwR18k/photo-2024-10-17-23-32-44.jpg" alt="Image 14" border="0"></a>
<a href="https://ibb.co/TBKGpDc"><img src="https://i.ibb.co/TBKGpDc/photo-2024-07-26-18-41-01.jpg" alt="Image 15" border="0"></a>
<a href="https://ibb.co/bHLbVdD"><img src="https://i.ibb.co/bHLbVdD/455691559-122111257202434651-6263614150393024155-n.jpg" alt="Image 16" border="0"></a>
<a href="https://ibb.co/VYSyXSj"><img src="https://i.ibb.co/VYSyXSj/photo-2024-09-05-18-37-46.jpg" alt="Image 17" border="0"></a>
<a href="https://ibb.co/QXDZgJ1"><img src="https://i.ibb.co/QXDZgJ1/reup-be-ana-pga-chuan-mat-xinh-body-dep-vu-to-dam-tiep-cac-boss-3113753-original.jpg" alt="Image 18" border="0"></a>
<a href="https://ibb.co/vhc79wJ"><img src="https://i.ibb.co/vhc79wJ/taoanhdep-lam-net-anh-22071.jpg" alt="Image 19" border="0"></a>
<a href="https://ibb.co/rQpDrXj"><img src="https://i.ibb.co/rQpDrXj/taoanhdep-lam-net-anh-84350.jpg" alt="Image 20" border="0"></a>
<a href="https://ibb.co/NncCRYJ"><img src="https://i.ibb.co/NncCRYJ/photo-9-2024-10-23-11-52-15.jpg" alt="Image 21" border="0"></a>
<a href="https://ibb.co/B4SWLf2"><img src="https://i.ibb.co/B4SWLf2/photo-4-2024-10-23-11-52-15.jpg" alt="Image 22" border="0"></a>
<a href="https://ibb.co/3TBjJrS"><img src="https://i.ibb.co/3TBjJrS/photo-3-2024-10-23-11-52-15.jpg" alt="Image 23" border="0"></a>
<a href="https://ibb.co/mNNL9h6"><img src="https://i.ibb.co/mNNL9h6/photo-8-2024-10-23-11-51-38.jpg" alt="Image 24" border="0"></a>
<a href="https://ibb.co/5RBJHX0"><img src="https://i.ibb.co/5RBJHX0/photo-2024-09-05-18-25-49.jpg" alt="Image 25" border="0"></a>
<a href="https://ibb.co/c10Lbzk"><img src="https://i.ibb.co/c10Lbzk/photo-2024-09-05-18-37-42-2.jpg" alt="Image 26" border="0"></a>
<a href="https://ibb.co/q7kXCmx"><img src="https://i.ibb.co/q7kXCmx/photo-2024-09-05-18-37-43.jpg" alt="Image 27" border="0"></a>
<a href="https://ibb.co/HrWycSc"><img src="https://i.ibb.co/HrWycSc/photo-2024-09-05-18-35-45-4.jpg" alt="Image 28" border="0"></a>
<a href="https://ibb.co/xXN7XND"><img src="https://i.ibb.co/xXN7XND/photo-2024-09-05-18-37-46.jpg" alt="Image 29" border="0"></a>
<a href="https://ibb.co/wRg0Fxr"><img src="https://i.ibb.co/wRg0Fxr/photo-2024-09-05-18-37-54.jpg" alt="Image 30" border="0"></a>
<a href="https://ibb.co/hVvFThy"><img src="https://i.ibb.co/hVvFThy/photo-2024-07-08-15-35-10.jpg" alt="Image 31" border="0"></a>
<a href="https://ibb.co/XVFxydz"><img src="https://i.ibb.co/XVFxydz/photo-2024-07-08-18-29-39.jpg" alt="Image 32" border="0"></a>
<a href="https://ibb.co/C1vzDrm"><img src="https://i.ibb.co/C1vzDrm/photo-2024-07-13-20-02-05.jpg" alt="Image 33" border="0"></a>
<a href="https://ibb.co/P4N1RxC"><img src="https://i.ibb.co/P4N1RxC/photo-2024-07-16-19-46-04.jpg" alt="Image 34" border="0"></a>
<a href="https://ibb.co/cbFvT6w"><img src="https://i.ibb.co/cbFvT6w/photo-2024-07-17-21-33-48.jpg" alt="Image 35" border="0"></a>
<a href="https://ibb.co/mDgpphk"><img src="https://i.ibb.co/mDgpphk/photo-2024-07-17-22-06-53.jpg" alt="Image 36" border="0"></a>
<a href="https://ibb.co/fxYN92r"><img src="https://i.ibb.co/fxYN92r/photo-2024-07-26-20-22-05.jpg" alt="Image 37" border="0"></a>
<a href="https://ibb.co/hfPm5kQ"><img src="https://i.ibb.co/hfPm5kQ/photo-2024-07-27-19-41-23.jpg" alt="Image 38" border="0"></a>
<a href="https://ibb.co/6gJpcCv"><img src="https://i.ibb.co/6gJpcCv/photo-2024-08-01-19-45-35.jpg" alt="Image 39" border="0"></a>
<a href="https://ibb.co/xMgVzrm"><img src="https://i.ibb.co/xMgVzrm/photo-2024-08-02-21-35-06.jpg" alt="Image 40" border="0"></a>
<a href="https://ibb.co/7SyF1KP"><img src="https://i.ibb.co/7SyF1KP/photo-2024-08-11-13-02-15.jpg" alt="Image 41" border="0"></a>
<a href="https://ibb.co/7NP8yrr"><img src="https://i.ibb.co/7NP8yrr/photo-2024-08-11-20-22-43.jpg" alt="Image 42" border="0"></a>
<a href="https://ibb.co/6FSKKz0"><img src="https://i.ibb.co/6FSKKz0/photo-2024-08-12-13-41-26.jpg" alt="Image 43" border="0"></a>
<a href="https://ibb.co/1RfR70n"><img src="https://i.ibb.co/1RfR70n/photo-2024-08-14-21-11-07.jpg" alt="Image 44" border="0"></a>
<a href="https://ibb.co/5n5Fvcv"><img src="https://i.ibb.co/5n5Fvcv/photo-2024-08-14-22-24-10.jpg" alt="Image 45" border="0"></a>
<a href="https://ibb.co/P91y2Dp"><img src="https://i.ibb.co/P91y2Dp/photo-2024-08-15-12-49-14.jpg" alt="Image 46" border="0"></a>
<a href="https://ibb.co/rpSrxZv"><img src="https://i.ibb.co/rpSrxZv/photo-2024-08-18-18-37-18.jpg" alt="Image 47" border="0"></a>
<a href="https://ibb.co/bN1JjqW"><img src="https://i.ibb.co/bN1JjqW/photo-2024-08-19-22-58-05.jpg" alt="Image 48" border="0"></a>
<a href="https://ibb.co/g7GNv7g"><img src="https://i.ibb.co/g7GNv7g/photo-2024-08-20-14-51-53.jpg" alt="Image 49" border="0"></a>
<a href="https://ibb.co/2qwCJnX"><img src="https://i.ibb.co/2qwCJnX/photo-2024-08-23-13-26-54.jpg" alt="Image 50" border="0"></a>
<a href="https://ibb.co/n7cmdBv"><img src="https://i.ibb.co/n7cmdBv/photo-2024-08-28-15-21-12.jpg" alt="Image 51" border="0"></a>
<a href="https://ibb.co/m86KxLK"><img src="https://i.ibb.co/m86KxLK/photo-2024-08-29-21-21-48.jpg" alt="Image 52" border="0"></a>
<a href="https://ibb.co/F0LX904"><img src="https://i.ibb.co/F0LX904/photo-2024-09-02-21-10-06.jpg" alt="Image 53" border="0"></a>
<a href="https://ibb.co/DDfzdWD"><img src="https://i.ibb.co/DDfzdWD/photo-2024-09-09-13-05-48.jpg" alt="Image 54" border="0"></a>
<a href="https://ibb.co/nQBW2Nc"><img src="https://i.ibb.co/nQBW2Nc/photo-2024-09-09-13-05-50.jpg" alt="Image 55" border="0"></a>
<a href="https://ibb.co/2Z6T8pw"><img src="https://i.ibb.co/2Z6T8pw/photo-2024-09-09-20-28-17.jpg" alt="Image 56" border="0"></a>
<a href="https://ibb.co/Yh4GSS9"><img src="https://i.ibb.co/Yh4GSS9/photo-2024-09-11-17-36-56.jpg" alt="Image 57" border="0"></a>
<a href="https://ibb.co/X3Vw2Dx"><img src="https://i.ibb.co/X3Vw2Dx/photo-2024-09-11-19-40-50.jpg" alt="Image 58" border="0"></a>
<a href="https://ibb.co/BNJtPRk"><img src="https://i.ibb.co/BNJtPRk/photo-2024-09-12-18-59-24.jpg" alt="Image 59" border="0"></a>
<a href="https://ibb.co/S5cZB7m"><img src="https://i.ibb.co/S5cZB7m/419418603-1508797216580744-6598850606428340490-n.jpg" alt="Image 60" border="0"></a>
<a href="https://ibb.co/bHLbVdD"><img src="https://i.ibb.co/bHLbVdD/455691559-122111257202434651-6263614150393024155-n.jpg" alt="Image 61" border="0"></a>
<a href="https://ibb.co/qYSb9Mm"><img src="https://i.ibb.co/qYSb9Mm/photo-2024-06-24-20-18-13.jpg" alt="Image 62" border="0"></a>
<a href="https://ibb.co/hfRfHRZ"><img src="https://i.ibb.co/hfRfHRZ/taoanhdep-lam-net-anh-38084.jpg" alt="Image 63" border="0"></a>
<a href="https://ibb.co/zsGMw70"><img src="https://i.ibb.co/zsGMw70/review-of-hay-tim-em-dam-for-reup-be-ana-pga-chuan-mat-xinh-body-dep-vu-to-dam-tiep-cac-boss-3134082.jpg" alt="Image 64" border="0"></a>
<a href="https://ibb.co/y0ghTLq"><img src="https://i.ibb.co/y0ghTLq/reup-trieu-uyen-cuc-pham-sieu-non-to-nong-bong-ngot-ngao-dang-yeu-3218910-original.jpg" alt="Image 65" border="0"></a>
<a href="https://ibb.co/ZHt0m10"><img src="https://i.ibb.co/ZHt0m10/reup-trieu-uyen-cuc-pham-sieu-non-to-nong-bong-ngot-ngao-dang-yeu-2970339-original.jpg" alt="Image 66" border="0"></a>
<a href="https://ibb.co/x1fnZ28"><img src="https://i.ibb.co/x1fnZ28/reup-trieu-uyen-cuc-pham-sieu-non-to-nong-bong-ngot-ngao-dang-yeu-2961977-original.jpg" alt="Image 67" border="0"></a>
<a href="https://ibb.co/cNswv30"><img src="https://i.ibb.co/cNswv30/review-of-luke-for-sieu-pham-mia-thien-than-2k4-moi-lon-tieu-muoi-douyin-hong-hao-3258387-original.jpg" alt="Image 68" border="0"></a>
<a href="https://ibb.co/tBvCVwX"><img src="https://i.ibb.co/tBvCVwX/photo-2024-09-05-18-55-28-2.jpg" alt="Image 69" border="0"></a>
<a href="https://ibb.co/wJcM7dm"><img src="https://i.ibb.co/wJcM7dm/photo-2024-08-19-21-10-58.jpg" alt="Image 70" border="0"></a>
<a href="https://ibb.co/pX3P1kG"><img src="https://i.ibb.co/pX3P1kG/photo-2024-08-28-19-44-03.jpg" alt="Image 71" border="0"></a>
<a href="https://ibb.co/TmHHqC7"><img src="https://i.ibb.co/TmHHqC7/photo-2024-09-09-13-05-49.jpg" alt="Image 72" border="0"></a>

</div>
</div>
</div>
</div>

<style>
    /* Animation cuộn từ phải sang trái */
    @keyframes slide {
    0% {
    transform: translateX(0); /* Bắt đầu từ vị trí ban đầu */
    }
    100% {
    transform: translateX(-100%); /* Cuộn đến hết bộ ảnh */
    }
    @keyframes slide {
        0% {
            transform: translate3d(0, 0, 0); /* Sử dụng translate3d */
        }
        100% {
            transform: translate3d(-100%, 0, 0); /* Cuộn đến hết bộ ảnh */
        }
    }
    }
    /* CSS cho các thiết bị có chiều rộng màn hình nhỏ hơn 3000px */
    @media (max-width: 3000px) {
        .slider-images {
            animation: slide 20s linear infinite; /* Điều chỉnh tốc độ cuộn cho thiết bị di động */
        }
    }
    @media (max-width: 600px) {
        .slider-images img {
            width: 120px; /* Giảm kích thước hình ảnh trên điện thoại */
            margin-right: 5px; /* Giảm khoảng cách giữa các hình ảnh */
        }
    }

    /* Khung chứa các hình ảnh */
.slider {
overflow: hidden; /* Ẩn các hình ảnh khi chúng cuộn ra khỏi khung nhìn */
width: 100%; /* Chiều rộng khung chứa */
}

/* Các hình ảnh sẽ được cuộn */
.slider-images {
display: flex;
width: 800%; /* Gấp đôi để chứa cả 2 bộ ảnh */
animation: slide 50s linear infinite; /* Animation cuộn với thời gian 30 giây */
}

/* Cài đặt cho hình ảnh */
.slider-images img {
width: 150px; /* Đặt chiều rộng của mỗi ảnh */
height: auto; /* Giữ tỉ lệ hình ảnh */
margin-right: -15px; /* Khoảng cách giữa các hình ảnh */
border-radius: 5px; /* Bo góc ảnh */
}

{
    font-size:30px;
    text-align: center; /* Căn giữa tiêu đề * /* 
    background: linear-gradient(45deg, #ff79a1, #ffdd40); /* Hiệu ứng gradient từ hồng sang vàng */
    -webkit-background-clip: text; /* Hiển thị gradient trên văn bản */
    -webkit-text-fill-color: transparent; /* Đặt màu văn bản trong suốt để hiển thị gradient */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Tạo đổ bóng cho tiêu đề */
    border: 2px solid #ff79a1; /* Tạo viền 3px với màu hồng */
}
</style>
<script>
    // JavaScript để sắp xếp ngẫu nhiên hình ảnh khi tải trang
    window.onload = function() {
        const sliderImages = document.querySelector('.slider-images');
        const images = Array.from(sliderImages.children);

        // Sắp xếp ngẫu nhiên
        images.sort(() => Math.random() - 0.5);

        // Xóa các ảnh hiện tại và thêm ảnh đã sắp xếp lại
        sliderImages.innerHTML = '';
        images.forEach(image => sliderImages.appendChild(image));
    };

    document.querySelectorAll('.slider-images a').forEach(function(anchor) {
    anchor.addEventListener('click', function(e) {
        e.preventDefault(); // Chặn thao tác nhấp vào liên kết
    });
});
</script>
</body>
</html>




<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thống kê</title>
</head>
<body>


    <script>let online = 427;  // Số người online ban đầu
        let vipMembers = 3821;  // Tổng VIP Members ban đầu
        let visitCount = 105581;  // Tổng lượt truy cập ban đầu

    function updateOnline() {
        // Chọn ngẫu nhiên mức thay đổi từ mảng
        const changes = [5, 13, 24, 32, 15, 11, 22, 11, 15, 17, 5, 17, 4, 19, 22, 12, 15, 29, 7, 12, 22, 11, 7, 12];
        let change = changes[Math.floor(Math.random() * changes.length)];
        
        // Xác định tăng hoặc giảm
        if (Math.random() < 0.5) {
            change = -change; // 50% cơ hội để giảm thay vì tăng
        }

        // Cập nhật số online trong giới hạn từ 347 đến 612
        online = Math.max(147, Math.min(212, online + change));
        document.getElementById("online").innerText = online;
    }

    function updateVipMembers() {
        // Cộng thêm 1 vào tổng số VIP Members sau mỗi 10 phút
        vipMembers += 1;
        document.getElementById("vipMembers").innerText = vipMembers;
    }

    function updatevisitCount() {
        // Tăng lượt truy cập ngẫu nhiên
        visitCount += Math.floor(Math.random() * 50); // Tăng ngẫu nhiên từ 1 đến 50 lượt truy cập
        document.getElementById("visitCount").innerText = visitCount;
    }

    // Cập nhật số người online mỗi 1 giây
    setInterval(function() {
        updateOnline();
    }, 3000);

    // Cập nhật số VIP Members mỗi 10 phút (600000 ms)
    setInterval(function() {
        updateVipMembers();
    }, 600000);

    // Cập nhật tổng lượt truy cập mỗi 5 giây
    setInterval(function() {
        updatevisitCount();
    }, 5000);
</script>

</body>
</html>

  <style>
    
    

    

     

    /* Điều chỉnh kích thước cho tất cả các hình ảnh trong phần thông tin */
.info-image {
    width: 170px; /* Đặt chiều rộng của hình ảnh */
    height: 100px; /* Chiều cao sẽ tự động điều chỉnh theo tỷ lệ */
    border-radius: 10px; /* Tạo góc bo tròn nhẹ */
    margin-bottom: 10px; /* Thêm khoảng cách dưới hình ảnh */
}
/* Nhúng các phông chữ hiện đại */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap');

/* Toàn bộ trang */
body {
    font-family: 'Poppins', sans-serif; /* Phông chữ hiện đại */
    background-color:  #c6c9ba; /* Màu nền nút cam đậm */
    color: #000000; /* Màu chữ trắng */
    margin: 0;
    border: 2px solid #008cff; /* Viền bạc */
    padding: 0;
    line-height: 1.6;

    box-shadow: 0 4px 8px #000000;
}

/* Tiêu đề nổi bật */
 h3 {
    font-size: 20px; /* Kích thước chữ */
    font-family: "Poppins", sans-serif;       
    font-weight: 700;
    color: #006eff;
    text-transform: uppercase; /* Chữ in hoa */
    letter-spacing: 2px; /* Khoảng cách giữa các chữ */
     border-radius: 10px; /* Bo tròn góc nút */ 
     top: -70px; /* Căn lên đầu */
}

/* Nút bấm ấn tượng */

.login-btns {
             position: absolute; /* Sử dụng absolute để căn chỉnh chính xác */
            top: -20px; /* Căn lên đầu */
            right: -60px; /* Căn sang góc phải */
            border-radius: 5px; /* Bo góc lớn cho nút */
            padding: 0px 0px;     /* Đệm cho nút */
            background-color: transparent; /* Màu nền nút */
            font-size: 14px;
            font-weight: 200; /* Giảm độ đậm của chữ (400 là bình thường, không quá đậm) */
            transition: background-color 0.3s ease;
        }

button {
   
    color: #ff0000; /* Màu chữ vàng */
    border-radius: 10px;
    padding: 5px 9px;
    background-color: #000000;
    font-weight: bold;
   
    transition: background-color 0.3s, transform 0.3s, box-shadow 0.3s;
    
}
button:hover {
    background-color: #ff3300; /* Màu nền khi hover */
    color: #000000 /* Màu chữ khi hover */
    transform: scale(1.05); /* Hiệu ứng phóng to nhẹ khi hover */
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.8); /* Hiệu ứng đổ bóng đậm */
}

/* Hộp thông tin */
.container {
    background-color: #C0C0C0 /* Màu nền nút cam đậm */
    padding: 40px;
    border-radius: 20px;
    color: #000000; /* Màu chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
    margin-top: 10px
}

/* Liên kết với hiệu ứng */
a { 
    color: #ffffff;
    text-decoration: none;
    font-weight: 700;
    border-bottom: 2px solid transparent; /* Đường viền ẩn ban đầu */
    transition: border-color 0.3s ease;
}

a:hover {
    border-color: #ffffff; /* Đường viền hiện ra khi hover */
}

/* Hình ảnh với hiệu ứng */
img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  
     
}

img:hover {
    transform: scale(1.05); /* Phóng to nhẹ khi hover */
    

    
}


/* Breadcrumb (dấu vết điều hướng) */
.breadcrumb {
    margin-top: -50px; /* Điều chỉnh giá trị này theo nhu cầu */
    font-size: 14px;
    font-weight: 700;
    color: #000000; /* Màu chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
    margin-bottom: 20px;
    text-align: center;
    transition: background-color 0.3s, transform 0.3s, box-shadow 0.3s;
}

.breadcrumb a {
    margin-top: -50px; /* Điều chỉnh giá trị này theo nhu cầu */
    color: #000000; /* Màu chữ đen */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Đổ bóng cho chữ */
    text-decoration: none;
    transition: background-color 0.3s, transform 0.3s, box-shadow 0.3s;
}

.breadcrumb a:hover {
    text-decoration: underline;
}

/* Footer */
.footer {
    background-color: #000000; /* Màu nền nút cam đậm */
    color: #000000; /* Màu chữ trắng */
    text-align: center;
    padding: 20px 0;
    font-size: 14px;
    box-shadow: 0 4px 8px #000000;
}

.footer a {
    color: #ff3d00;
    text-decoration: none;
}

.footer a:hover {
    text-decoration: underline;
}

/* Điều chỉnh kích thước hình ảnh trong phần gallery */
.gallery-image {
    width:200px; /* Giảm kích thước hình ảnh trong phần gallery */
    height: auto; /* Giữ tỷ lệ hình ảnh */
    margin-right: 10px; /* Khoảng cách giữa các hình ảnh */
    border-radius: 10px; /* Bo góc nhẹ cho hình ảnh */
}

/* Cài đặt phông chữ */
@import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css');








    .fixed-logo {
    position: fixed;   /* Cố định logo */
    top: 10px;         /* Khoảng cách từ trên */
    left: 10px;        /* Khoảng cách từ trái */
    width: 170px;      /* Kích thước logo */
    z-index: 999;      /* Đảm bảo logo nằm trên cùng */
}

.fixed-logo img {
    width: 350px;           /* Kích thước logo (tùy chỉnh theo ý muốn) */
    height: auto;           /* Tự động điều chỉnh chiều cao dựa trên chiều rộng */
    border-radius: 5px;     /* Bo góc nhẹ cho logo */
    box-shadow: 0 4px 8px #000000;
}


.slider-images {
    display: flex;
    padding: 10px 0;
    gap: 40px; /* Thêm khoảng cách giữa các hình ảnh */
}

.slider-images img {
        width: 150px;
        height: 200px;
        object-fit: cover;
        border-radius: 5px;
        border: 2px solid #ffffff; /* Viền bạc */
}

body {
    font-family: 'Poppins", sans-serif;
    background-color: #000000; /* Màu nền nút cam đậm */
    border: 2px solid #ffffff; /* Viền bạc */

    border-radius: 10px;   
    padding: 0 3%; /* Điều chỉnh padding hai bên cho cả trang */
}

.container {
    width: 90%; /* Thu gọn nội dung trang */
    padding: 20px;
    background: linear-gradient(135deg, #f7a7c5, #d14d83); /* Nền hồng gradient */
    margin-top: 20px
    color: #ffffff; /* Chữ trắng */
    border: 1px solid #ffffff; /* Viền vàng */

}


    #toggle-chat-btn:hover {
        background-color: #ffffff; /* Màu nền khi hover */
        
    }
  </style>
</head>
<body>

    
   
    
  
  <script>
    



    function toggleContent(region, type) {
    // Tạo danh sách các phần tử cần quản lý
    const sections = ['info', 'images', 'bookings'];


    // Duyệt qua danh sách và ẩn tất cả các phần tử không phải là phần tử đang được click
    sections.forEach(section => {
        const contentDiv = document.getElementById(`${section}-${region}`);
        if (section === type) {
            contentDiv.style.display = (contentDiv.style.display === "block") ? "none" : "block";
        } else {
            contentDiv.style.display = "none"; // Ẩn tất cả các phần tử không được nhấn
        }
    });
}





  </script>

</body>
</html>
