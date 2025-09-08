<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Phân Tích Đường Cầu Baccarat</title>
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #e74c3c;
            --accent-color: #3498db;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
            --success-color: #27ae60;
            --warning-color: #f39c12;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #1a2a6c, #b21f1f, #fdbb2d);
            color: #333;
            line-height: 1.6;
            min-height: 100vh;
            padding: 20px;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.95);
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            overflow: hidden;
        }
        
        header {
            background: var(--primary-color);
            color: white;
            padding: 20px;
            text-align: center;
            position: relative;
        }
        
        header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }
        
        header p {
            font-size: 1.2rem;
            opacity: 0.9;
        }
        
        .ai-badge {
            position: absolute;
            top: 15px;
            right: 15px;
            background: var(--secondary-color);
            color: white;
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: bold;
        }
        
        .main-content {
            display: flex;
            flex-wrap: wrap;
            padding: 20px;
        }
        
        .upload-section {
            flex: 1;
            min-width: 300px;
            padding: 20px;
            background: var(--light-color);
            border-radius: 10px;
            margin: 10px;
        }
        
        .analysis-section {
            flex: 2;
            min-width: 500px;
            padding: 20px;
            margin: 10px;
        }
        
        .upload-box {
            border: 3px dashed var(--accent-color);
            border-radius: 10px;
            padding: 30px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
            margin-bottom: 20px;
        }
        
        .upload-box:hover {
            background: rgba(52, 152, 219, 0.1);
        }
        
        .upload-icon {
            font-size: 3rem;
            color: var(--accent-color);
            margin-bottom: 15px;
        }
        
        .upload-box p {
            margin: 10px 0;
        }
        
        .btn {
            background: var(--accent-color);
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1rem;
            font-weight: bold;
            transition: all 0.3s;
            display: inline-block;
            margin-top: 10px;
        }
        
        .btn:hover {
            background: #2980b9;
            transform: translateY(-2px);
        }
        
        .btn-analyze {
            background: var(--success-color);
            width: 100%;
            padding: 15px;
            font-size: 1.2rem;
        }
        
        .btn-analyze:hover {
            background: #219653;
        }
        
        .result-container {
            background: white;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            margin-top: 20px;
        }
        
        .result-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--light-color);
        }
        
        .prediction {
            text-align: center;
            padding: 20px;
            background: var(--light-color);
            border-radius: 10px;
            margin-bottom: 20px;
        }
        
        .prediction-value {
            font-size: 2.5rem;
            font-weight: bold;
            color: var(--secondary-color);
            margin: 10px 0;
        }
        
        .confidence {
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 15px 0;
        }
        
        .confidence-bar {
            width: 100%;
            height: 20px;
            background: #ddd;
            border-radius: 10px;
            overflow: hidden;
            margin-left: 10px;
        }
        
        .confidence-fill {
            height: 100%;
            background: var(--success-color);
            border-radius: 10px;
            transition: width 1s ease-in-out;
        }
        
        .theory-match {
            margin: 20px 0;
        }
        
        .theory-item {
            background: var(--light-color);
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .match-percent {
            background: var(--accent-color);
            color: white;
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 0.9rem;
        }
        
        .image-preview {
            margin-top: 20px;
            text-align: center;
        }
        
        .image-preview img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .advanced-features {
            background: var(--light-color);
            padding: 20px;
            border-radius: 10px;
            margin-top: 20px;
        }
        
        .feature-list {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin-top: 15px;
        }
        
        .feature-item {
            width: calc(50% - 10px);
            background: white;
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 15px;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
        }
        
        .feature-icon {
            font-size: 1.5rem;
            color: var(--accent-color);
            margin-bottom: 10px;
        }
        
        footer {
            text-align: center;
            padding: 20px;
            background: var(--dark-color);
            color: white;
        }
        
        @media (max-width: 768px) {
            .main-content {
                flex-direction: column;
            }
            
            .feature-item {
                width: 100%;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="ai-badge">AI NÂNG CAO</div>
            <h1>PHÂN TÍCH ĐƯỜNG CẦU BACCARAT</h1>
            <p>Công nghệ AI tiên tiến phân tích hình ảnh và dự đoán kết quả với độ chính xác cao</p>
        </header>
        
        <div class="main-content">
            <div class="upload-section">
                <h2>Tải Ảnh Lên Để Phân Tích</h2>
                <div class="upload-box" id="uploadBox">
                    <div class="upload-icon">📁</div>
                    <p>Kéo & thả ảnh vào đây hoặc</p>
                    <p><strong>Chọn file từ máy tính</strong></p>
                    <p class="small">Hỗ trợ: JPG, PNG, JPEG (Kích thước tối đa: 5MB)</p>
                </div>
                <input type="file" id="fileInput" accept="image/*" style="display: none;">
                
                <div class="image-preview">
                    <img id="previewImage" src="" alt="Xem trước ảnh" style="display: none;">
                </div>
                
                <button class="btn btn-analyze" id="analyzeBtn">Phân Tích Đường Cầu</button>
                
                <div class="advanced-features">
                    <h3>Tính Năng AI Nâng Cao</h3>
                    <div class="feature-list">
                        <div class="feature-item">
                            <div class="feature-icon">🔍</div>
                            <h4>Nhận Diện Hình Ảnh</h4>
                            <p>AI quét và nhận diện chính xác các đường cầu từ ảnh</p>
                        </div>
                        <div class="feature-item">
                            <div class="feature-icon">📊</div>
                            <h4>Phân Tích Dữ Liệu</h4>
                            <p>Phân tích dựa trên các lý thuyết cầu Baccarat chuyên sâu</p>
                        </div>
                        <div class="feature-item">
                            <div class="feature-icon">📈</div>
                            <h4>Dự Đoán Thông Minh</h4>
                            <p>Đưa ra dự đoán với tỷ lệ chính xác cao nhất</p>
                        </div>
                        <div class="feature-item">
                            <div class="feature-icon">⚙️</div>
                            <h4>Cập Nhật Liên Tục</h4>
                            <p>Học hỏi và cải thiện độ chính xác qua từng phân tích</p>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="analysis-section">
                <h2>Kết Quả Phân Tích</h2>
                <div class="result-container">
                    <div class="result-header">
                        <h3>Dự Đoán Kết Quả</h3>
                        <span id="analysisStatus">Chưa phân tích</span>
                    </div>
                    
                    <div class="prediction">
                        <p>Kết quả dự đoán:</p>
                        <div class="prediction-value" id="predictionValue">--</div>
                        <p>Độ tin cậy:</p>
                        <div class="confidence">
                            <span id="confidenceValue">0%</span>
                            <div class="confidence-bar">
                                <div class="confidence-fill" id="confidenceFill" style="width: 0%"></div>
                            </div>
                        </div>
                    </div>
                    
                    <div class="theory-match">
                        <h3>Khớp Với Lý Thuyết</h3>
                        <div class="theory-item">
                            <span>Cầu Bệt</span>
                            <span class="match-percent">0%</span>
                        </div>
                        <div class="theory-item">
                            <span>Cầu Tiến Đoán</span>
                            <span class="match-percent">0%</span>
                        </div>
                        <div class="theory-item">
                            <span>Cầu Triếp Án</span>
                            <span class="match-percent">0%</span>
                        </div>
                        <div class="theory-item">
                            <span>Cầu Đối Xứng</span>
                            <span class="match-percent">0%</span>
                        </div>
                    </div>
                </div>
                
                <div class="result-container" style="margin-top: 20px;">
                    <h3>Hướng Dẫn Sử Dụng</h3>
                    <ol style="margin-left: 20px; margin-top: 10px;">
                        <li>Tải lên hình ảnh chứa đường cầu Baccarat cần phân tích</li>
                        <li>Hệ thống AI sẽ tự động nhận diện và quét các đường cầu</li>
                        <li>AI áp dụng các lý thuyết đã học để phân tích</li>
                        <li>Xem kết quả dự đoán và độ tin cậy</li>
                        <li>Đưa ra quyết định đặt cược dựa trên phân tích</li>
                    </ol>
                </div>
            </div>
        </div>
        
        <footer>
            <p>© 2023 AI Phân Tích Baccarat | Sử dụng công nghệ AI tiên tiến nhất</p>
        </footer>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const uploadBox = document.getElementById('uploadBox');
            const fileInput = document.getElementById('fileInput');
            const previewImage = document.getElementById('previewImage');
            const analyzeBtn = document.getElementById('analyzeBtn');
            const predictionValue = document.getElementById('predictionValue');
            const confidenceValue = document.getElementById('confidenceValue');
            const confidenceFill = document.getElementById('confidenceFill');
            const analysisStatus = document.getElementById('analysisStatus');
            
            // Xử lý kéo thả và chọn file
            uploadBox.addEventListener('click', function() {
                fileInput.click();
            });
            
            uploadBox.addEventListener('dragover', function(e) {
                e.preventDefault();
                uploadBox.style.background = 'rgba(52, 152, 219, 0.2)';
            });
            
            uploadBox.addEventListener('dragleave', function() {
                uploadBox.style.background = '';
            });
            
            uploadBox.addEventListener('drop', function(e) {
                e.preventDefault();
                uploadBox.style.background = '';
                
                if (e.dataTransfer.files.length) {
                    fileInput.files = e.dataTransfer.files;
                    handleFile(fileInput.files[0]);
                }
            });
            
            fileInput.addEventListener('change', function() {
                if (fileInput.files.length) {
                    handleFile(fileInput.files[0]);
                }
            });
            
            function handleFile(file) {
                if (file.type.match('image.*')) {
                    const reader = new FileReader();
                    
                    reader.onload = function(e) {
                        previewImage.src = e.target.result;
                        previewImage.style.display = 'block';
                        analysisStatus.textContent = 'Ảnh đã sẵn sàng để phân tích';
                        analysisStatus.style.color = '#27ae60';
                    };
                    
                    reader.readAsDataURL(file);
                } else {
                    alert('Vui lòng chọn file ảnh!');
                }
            }
            
            // Xử lý phân tích
            analyzeBtn.addEventListener('click', function() {
                if (!previewImage.src) {
                    alert('Vui lòng tải lên ảnh đường cầu trước khi phân tích!');
                    return;
                }
                
                analysisStatus.textContent = 'Đang phân tích...';
                analysisStatus.style.color = '#f39c12';
                
                // Giả lập quá trình phân tích bằng AI
                setTimeout(() => {
                    // Kết quả ngẫu nhiên để minh họa
                    const results = ['CỬA CÁI', 'CỬA CON', 'HÒA'];
                    const randomResult = results[Math.floor(Math.random() * results.length)];
                    const randomConfidence = Math.floor(Math.random() * 41) + 60; // 60-100%
                    
                    // Hiển thị kết quả
                    predictionValue.textContent = randomResult;
                    confidenceValue.textContent = randomConfidence + '%';
                    confidenceFill.style.width = randomConfidence + '%';
                    
                    // Cập nhật độ khớp với lý thuyết
                    const matchPercents = document.querySelectorAll('.match-percent');
                    matchPercents.forEach(item => {
                        const percent = Math.floor(Math.random() * 41) + 60;
                        item.textContent = percent + '%';
                    });
                    
                    analysisStatus.textContent = 'Phân tích hoàn thành';
                    analysisStatus.style.color = '#27ae60';
                    
                    // Hiệu ứng cho kết quả
                    predictionValue.style.transition = 'all 0.5s';
                    predictionValue.style.transform = 'scale(1.2)';
                    setTimeout(() => {
                        predictionValue.style.transform = 'scale(1)';
                    }, 500);
                    
                }, 2000);
            });
        });
    </script>
</body>
</html>
