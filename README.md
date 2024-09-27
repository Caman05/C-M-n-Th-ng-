# Cá Mặn Tháng 5
- index.html         (Trang chủ)
- style.css          (File CSS cho giao diện)
- script.js          (File JS để thêm các chức năng)
- stories/           (Thư mục chứa các truyện)
    - story1.html
    - story2.html
- images/            (Thư mục chứa ảnh)
- <!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trang chủ - Đọc truyện online</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Đọc truyện online</h1>
        <nav>
            <ul>
                <li><a href="index.html">Trang chủ</a></li>
                <li><a href="#top-truyen">Top truyện</a></li>
                <li><a href="#the-loai">Thể loại</a></li>
            </ul>
        </nav>
    </header>

    <section id="top-truyen">
        <h2>Top truyện hay</h2>
        <div class="truyen-list">
            <article>
                <a href="stories/story1.html">
                    <img src="images/truyen1.jpg" alt="Truyện 1">
                    <h3>Truyện 1: Chi đại xuyên thành người đẹp mỏng manh dễ vỡ</h3>
                </a>
                <p>Một câu chuyện đầy kịch tính về một cô gái mạnh mẽ và quyết đoán.</p>
            </article>
            <article>
                <a href="stories/story2.html">
                    <img src="images/truyen2.jpg" alt="Truyện 2">
                    <h3>Truyện 2: Tên truyện thứ hai</h3>
                </a>
                <p>Truyện kể về hành trình trưởng thành của nhân vật chính.</p>
            </article>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Đọc truyện online. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    margin: 0;
    padding: 0;
}

header {
    background-color: #333;
    color: #fff;
    padding: 1rem;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 1rem;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

#top-truyen {
    margin: 2rem auto;
    padding: 0 1rem;
    max-width: 1200px;
}

.truyen-list {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    justify-content: space-around;
}

article {
    background-color: #fff;
    padding: 1rem;
    border: 1px solid #ccc;
    width: 300px;
    text-align: center;
}

article img {
    max-width: 100%;
    height: auto;
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1rem;
    position: relative;
    bottom: 0;
    width: 100%;
}
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chi đại xuyên thành người đẹp mỏng manh dễ vỡ</title>
    <link rel="stylesheet" href="../style.css">
</head>
<body>
    <header>
        <h1>Chi đại xuyên thành người đẹp mỏng manh dễ vỡ</h1>
        <nav>
            <ul>
                <li><a href="../index.html">Trang chủ</a></li>
            </ul>
        </nav>
    </header>

    <article>
        <h2>Tên truyện: Chi đại xuyên thành người đẹp mỏng manh dễ vỡ</h2>
        <p>[Nội dung chương truyện...]</p>
    </article>

    <footer>
        <p>&copy; 2024 Đọc truyện online. All rights reserved.</p>
    </footer>
</body>
</html>
document.addEventListener("DOMContentLoaded", function() {
    const darkModeToggle = document.createElement('button');
    darkModeToggle.textContent = "Toggle Dark Mode";
    darkModeToggle.style.position = "fixed";
    darkModeToggle.style.bottom = "20px";
    darkModeToggle.style.right = "20px";
    document.body.appendChild(darkModeToggle);

    darkModeToggle.addEventListener("click", function() {
        document.body.classList.toggle("dark-mode");
    });
});

// CSS bổ sung cho dark mode
body.dark-mode {
    background-color: #121212;
    color: #fff;
}

header.dark-mode {
    background-color: #1f1f1f;
}

footer.dark-mode {
    background-color: #1f1f1f;
}
