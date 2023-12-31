<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
        /* 在這裡添加您的自定義樣式 */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 1em;
            text-align: center;
        }

        section {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        h1, h2, p {
            color: #333;
        }

        /* 輪播樣式 */
        .slideshow-container {
            max-width: 1000px;
            position: relative;
            margin: auto;
        }

        .mySlides {
            display: none;
        }

        .mySlides img {
            width: 100%;
            height: auto;
        }

        /* 翻頁點樣式 */
        .dot {
            height: 15px;
            width: 15px;
            margin: 0 2px;
            background-color: #bbb;
            border-radius: 50%;
            display: inline-block;
            transition: background-color 0.6s ease;
        }

        .active {
            background-color: #717171;
        }
    </style>
</head>

<body>

    <header>
        <h1>未來之星 — 探索新世界 班展</h1>
    </header>

    <!-- 輪播圖片 -->
    <div class="slideshow-container">
        <div class="mySlides">
            <img src="https://www.tdri.org.tw/wp-content/uploads/2019/10/2019.10.03_Supersouth-237.jpg" alt="Image 1">
        </div>

        <div class="mySlides">
            <img src="https://cdn.fundesign.tv/wp-content/uploads/2022/10/2266AE7E-CD88-451E-B6D9-3A10181234AE-L0-001-1024x683.jpg" alt="Image 2">
        </div>

        <div class="mySlides">
            <img src="https://www.designexpo.org.tw/uploads/exhibition_pic/image/320/thumb_TLS_8729.jpg" alt="Image 3">
        </div>
    </div>

    <!-- 翻頁點 -->
    <div style="text-align:center">
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
    </div>

    <section>
        <h2>歡迎來到「未來之星 — 探索新世界」班展！</h2>
        <!-- 以下是展示亮點、活動亮點和其他內容 -->
            <h3>12/20(四)-12/24(日)10:00-16:00</h3>
    
            <!-- 具體展示亮點和活動亮點 -->
    
            <h2>展示亮點：</h2>
            <ol>
                <li>未來職業探索：學生將展示他們對未來的職業興趣，透過展覽來呈現他們夢想中的職業、技能和事業方向。</li>
                <li>科技創新：探索學生們的科技創新作品，這些作品將展示他們對未來科技趨勢的理解和應用，可能包括機器學習、人工智慧和可持續技術。</li>
                <li>藝術與表演：欣賞來自藝術和表演藝術領域的學生才華，包括繪畫、攝影、音樂和戲劇表演，探索藝術如何影響我們的未來。</li>
                <li>環保與永續：睜大眼睛看待未來的地球，學生將展示他們在環保和永續發展方面的努力，並提出解決方案以應對未來的環境挑戰。</li>
            </ol>
    
            <h2>活動亮點：</h2>
            <ul>
                <li>未來論壇：學生將參與未來論壇，分享他們對未來的看法、夢想和挑戰，與觀眾互動，啟發更多有關未來的思考。</li>
                <li>科技體驗區：提供給參觀者的互動體驗區，讓他們親自感受未來的科技創新，如虛擬現實、機器人技術等。</li>
                <li>藝術工作坊：讓參觀者參與藝術工作坊，體驗藝術的魅力，並將自己的創意帶回家。</li>
            </ul>
            
            <p>我們期待您的加入，一同探索學生們對未來的各種憧憬和可能性。讓我們共同啟發和培養這群「未來之星」！</p>
    </section>
    
    <section>

        <h2>關於我們</h2>
        <p>推廣班展是一個致力於提供高質量教育資源的平台。我們匯集了來自各行各業的專業人士，為學習者提供全面的課程體驗。</p>

        <!-- 其他內容 -->

        <h2>聯絡我們</h2>
        <p>有任何問題或疑慮？請隨時與我們聯繫。我們樂意聆聽您的反饋並提供支持。</p>
        <p>電子郵件contact@example.com</p>
    </section>

    <script>
        var slideIndex = 0;
        showSlides();

        function showSlides() {
            var i;
            var slides = document.getElementsByClassName("mySlides");
            var dots = document.getElementsByClassName("dot");
            for (i = 0; i < slides.length; i++) {
                slides[i].style.display = "none";
            }
            slideIndex++;
            if (slideIndex > slides.length) { slideIndex = 1 }
            for (i = 0; i < dots.length; i++) {
                dots[i].className = dots[i].className.replace(" active", "");
            }
            slides[slideIndex - 1].style.display = "block";
            dots[slideIndex - 1].className += " active";
            setTimeout(showSlides, 2000); // 切換圖片的時間間隔，單位為毫秒（這裡是2秒）
        }
   
   </script>

</body>

</html>
