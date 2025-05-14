<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trang Chủ - HomeHub</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .hero-bg {
            background-image: url('https://images.unsplash.com/photo-1560518883-ce09059eeffa?q=80&w=1973&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
            background-size: cover;
            background-position: center;
        }
        .property-card img {
            aspect-ratio: 16 / 10;
            object-fit: cover;
        }
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        ::-webkit-scrollbar-thumb {
            background: #888;
            border-radius: 10px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #555;
        }
    </style>
</head>
<body class="bg-gray-100">

    <header class="bg-white shadow-md sticky top-0 z-50">
        <div class="container mx-auto px-4 py-4 flex flex-wrap justify-between items-center">
            <a href="index.html" class="text-2xl font-bold text-indigo-600">
                <i class="fas fa-home mr-2"></i>HomeHub
            </a>

            <nav class="hidden md:flex items-center space-x-4 lg:space-x-6">
                <a href="listings.html?type=nha-nguyen-can" class="text-gray-600 hover:text-indigo-600 transition duration-300">Nhà Nguyên Căn</a>
                <a href="listings.html?type=chung-cu" class="text-gray-600 hover:text-indigo-600 transition duration-300">Chung Cư</a>
                <div class="relative group">
                    <button class="text-gray-600 hover:text-indigo-600 transition duration-300 focus:outline-none">
                        Loại Khác <i class="fas fa-chevron-down text-xs ml-1"></i>
                    </button>
                    <div class="absolute left-0 mt-2 w-48 bg-white rounded-md shadow-lg py-1 z-20 opacity-0 group-hover:opacity-100 transition-opacity duration-300 invisible group-hover:visible">
                        <a href="listings.html?type=dat-nen" class="block px-4 py-2 text-sm text-gray-700 hover:bg-indigo-50 hover:text-indigo-600">Đất Nền</a>
                        <a href="listings.html?type=biet-thu" class="block px-4 py-2 text-sm text-gray-700 hover:bg-indigo-50 hover:text-indigo-600">Biệt Thự</a>
                        <a href="listings.html?type=mat-bang" class="block px-4 py-2 text-sm text-gray-700 hover:bg-indigo-50 hover:text-indigo-600">Mặt Bằng Kinh Doanh</a>
                    </div>
                </div>
            </nav>

            <div class="hidden md:flex items-center space-x-3">
                <a href="submit-property.html" class="bg-green-500 hover:bg-green-600 text-white font-semibold py-2 px-4 rounded-lg transition duration-300 text-sm">
                    <i class="fas fa-plus-circle mr-1"></i> Đăng Tin
                </a>
                <a href="login.html" class="text-gray-600 hover:text-indigo-600 transition duration-300">Đăng Nhập</a>
                <a href="register.html" class="bg-indigo-600 hover:bg-indigo-700 text-white font-semibold py-2 px-4 rounded-lg transition duration-300">Đăng Ký</a>
            </div>

            <div class="md:hidden">
                <button id="mobile-menu-button" class="text-gray-600 hover:text-indigo-600 focus:outline-none">
                    <i class="fas fa-bars text-xl"></i>
                </button>
            </div>
        </div>

        <div id="mobile-menu" class="hidden md:hidden bg-white shadow-lg">
            <a href="listings.html?type=nha-nguyen-can" class="block px-4 py-3 text-gray-600 hover:bg-indigo-50 hover:text-indigo-600 transition duration-300">Nhà Nguyên Căn</a>
            <a href="listings.html?type=chung-cu" class="block px-4 py-3 text-gray-600 hover:bg-indigo-50 hover:text-indigo-600 transition duration-300">Chung Cư</a>
            <a href="listings.html?type=dat-nen" class="block px-4 py-3 text-gray-600 hover:bg-indigo-50 hover:text-indigo-600 transition duration-300">Đất Nền</a>
            <a href="listings.html?type=biet-thu" class="block px-4 py-3 text-gray-600 hover:bg-indigo-50 hover:text-indigo-600 transition duration-300">Biệt Thự</a>
             <a href="listings.html?type=mat-bang" class="block px-4 py-3 text-gray-600 hover:bg-indigo-50 hover:text-indigo-600 transition duration-300">Mặt Bằng Kinh Doanh</a>
            <hr class="my-1">
            <a href="submit-property.html" class="block px-4 py-3 text-green-500 hover:bg-green-50 hover:text-green-600 font-semibold transition duration-300"><i class="fas fa-plus-circle mr-1"></i> Đăng Tin</a>
            <a href="login.html" class="block px-4 py-3 text-gray-600 hover:bg-indigo-50 hover:text-indigo-600 transition duration-300">Đăng Nhập</a>
            <a href="register.html" class="block px-4 py-3 bg-indigo-600 text-white text-center rounded-b-lg hover:bg-indigo-700 transition duration-300">Đăng Ký</a>
        </div>
    </header>

    <section class="hero-bg py-20 md:py-32">
        <div class="container mx-auto px-4 text-center">
            <h1 class="text-4xl md:text-5xl font-bold text-white mb-6 leading-tight">Tìm Kiếm Ngôi Nhà Mơ Ước Của Bạn</h1>
            <p class="text-lg md:text-xl text-gray-200 mb-10 max-w-2xl mx-auto">Khám phá hàng ngàn tin đăng bất động sản chính chủ, giá tốt nhất tại HomeHub.</p>

            <form action="listings.html" method="GET" class="max-w-3xl mx-auto bg-white p-6 rounded-lg shadow-xl">
                <div class="flex flex-col md:flex-row md:space-x-4 space-y-4 md:space-y-0">
                    <input type="text" name="keyword" placeholder="Nhập địa điểm, từ khóa, quận, dự án..." class="flex-grow p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent outline-none transition duration-300">
                    <button type="submit" class="bg-indigo-600 hover:bg-indigo-700 text-white font-semibold py-3 px-8 rounded-lg transition duration-300">
                        <i class="fas fa-search mr-2"></i>Tìm Kiếm
                    </button>
                </div>
                <div class="grid grid-cols-2 sm:grid-cols-2 md:grid-cols-4 gap-4 mt-6">
                    <div>
                        <label for="filter-district" class="sr-only">Quận</label>
                        <select id="filter-district" name="district" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent outline-none transition duration-300 bg-white">
                            <option value="">Chọn Quận</option>
                            <option value="q1">Quận 1</option>
                            <option value="q2">Quận 2</option>
                            <option value="q3">Quận 3</option>
                            <option value="q4">Quận 4</option>
                            <option value="q5">Quận 5</option>
                            <option value="q6">Quận 6</option>
                            <option value="q7">Quận 7</option>
                            <option value="q8">Quận 8</option>
                            <option value="q9">Quận 9</option>
                            <option value="q10">Quận 10</option>
                            <option value="q11">Quận 11</option>
                            <option value="q12">Quận 12</option>
                            <option value="tanbinh">Tân Bình</option>
                            <option value="binhtan">Bình Tân</option>
                            <option value="phunhuan">Phú Nhuận</option>
                            <option value="govap">Gò Vấp</option>
                            <option value="binhthanh">Bình Thạnh</option>
                            <option value="thuduc">TP. Thủ Đức</option>
                        </select>
                    </div>
                    <div>
                        <label for="filter-price" class="sr-only">Mức Giá</label>
                        <select id="filter-price" name="price" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent outline-none transition duration-300 bg-white">
                            <option value="">Mức Giá</option>
                            <option value="0-1">Dưới 1 tỷ</option>
                            <option value="1-3">1 - 3 tỷ</option>
                            <option value="3-5">3 - 5 tỷ</option>
                            <option value="5-10">5 - 10 tỷ</option>
                            <option value="10-20">10 - 20 tỷ</option>
                            <option value="20-0">Trên 20 tỷ</option>
                        </select>
                    </div>
                    <div>
                        <label for="filter-area" class="sr-only">Diện Tích</label>
                        <select id="filter-area" name="area" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent outline-none transition duration-300 bg-white">
                            <option value="">Diện Tích</option>
                            <option value="0-30">Dưới 30 m²</option>
                            <option value="30-50">30 - 50 m²</option>
                            <option value="50-80">50 - 80 m²</option>
                            <option value="80-100">80 - 100 m²</option>
                            <option value="100-150">100 - 150 m²</option>
                            <option value="150-0">Trên 150 m²</option>
                        </select>
                    </div>
                    <div>
                        <label for="filter-type" class="sr-only">Loại Nhà</label>
                        <select id="filter-type" name="type" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent outline-none transition duration-300 bg-white">
                            <option value="">Loại Nhà</option>
                            <option value="nha-rieng">Nhà Riêng</option>
                            <option value="can-ho">Căn Hộ Chung Cư</option>
                            <option value="dat-nen">Đất Nền</option>
                            <option value="biet-thu">Biệt Thự</option>
                            <option value="mat-bang">Mặt Bằng Kinh Doanh</option>
                            <option value="phong-tro">Phòng Trọ</option>
                        </select>
                    </div>
                </div>
            </form>
        </div>
    </section>

    <section class="py-12 md:py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-gray-800 mb-3 text-center">Bất Động Sản Nổi Bật</h2>
            <p class="text-gray-600 text-center mb-10 max-w-xl mx-auto">Những lựa chọn tốt nhất được nhiều người quan tâm, cập nhật liên tục.</p>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="property-card bg-white rounded-xl shadow-lg overflow-hidden hover:shadow-2xl transition-shadow duration-300">
                    <a href="property-details.html?id=1" class="block">
                        <img src="https://placehold.co/600x400/e2e8f0/cbd5e0?text=Ảnh+BĐS+1" alt="[Image of Căn Hộ Cao Cấp Quận 1]" class="w-full h-56 object-cover">
                    </a>
                    <div class="p-6">
                        <div class="flex justify-between items-start mb-2">
                            <a href="property-details.html?id=1" class="block">
                                <h3 class="text-xl font-semibold text-gray-800 hover:text-indigo-600 transition duration-300 leading-tight">Căn Hộ Cao Cấp Quận 1, View Sông</h3>
                            </a>
                            <button class="text-red-500 hover:text-red-600 text-xl p-1 -mr-1" onclick="toggleFavorite(this)">
                                <i class="far fa-heart"></i>
                            </button>
                        </div>
                        <p class="text-sm text-gray-500 mb-3"><i class="fas fa-map-marker-alt mr-1 text-indigo-500"></i> Phường Bến Nghé, Quận 1, TP. HCM</p>
                        <div class="text-2xl font-bold text-indigo-600 mb-3">5.2 Tỷ VNĐ</div>
                        <div class="flex justify-between text-sm text-gray-600 border-t pt-3">
                            <span><i class="fas fa-bed mr-1 text-indigo-400"></i> 2 PN</span>
                            <span><i class="fas fa-bath mr-1 text-indigo-400"></i> 2 WC</span>
                            <span><i class="fas fa-ruler-combined mr-1 text-indigo-400"></i> 75 m²</span>
                        </div>
                         <p class="text-xs text-gray-400 mt-3">Đăng 2 giờ trước</p>
                    </div>
                </div>

                <div class="property-card bg-white rounded-xl shadow-lg overflow-hidden hover:shadow-2xl transition-shadow duration-300">
                    <a href="property-details.html?id=2" class="block">
                        <img src="https://placehold.co/600x400/d1fae5/6ee7b7?text=Ảnh+BĐS+2" alt="[Image of Nhà Phố Mặt Tiền Quận 3]" class="w-full h-56 object-cover">
                    </a>
                    <div class="p-6">
                         <div class="flex justify-between items-start mb-2">
                            <a href="property-details.html?id=2" class="block">
                                <h3 class="text-xl font-semibold text-gray-800 hover:text-indigo-600 transition duration-300 leading-tight">Nhà Phố Mặt Tiền Kinh Doanh Quận 3</h3>
                            </a>
                            <button class="text-gray-400 hover:text-red-500 text-xl p-1 -mr-1" onclick="toggleFavorite(this)">
                                <i class="far fa-heart"></i>
                            </button>
                        </div>
                        <p class="text-sm text-gray-500 mb-3"><i class="fas fa-map-marker-alt mr-1 text-indigo-500"></i> Phường 6, Quận 3, TP. HCM</p>
                        <div class="text-2xl font-bold text-indigo-600 mb-3">15 Tỷ VNĐ</div>
                        <div class="flex justify-between text-sm text-gray-600 border-t pt-3">
                            <span><i class="fas fa-bed mr-1 text-indigo-400"></i> 4 PN</span>
                            <span><i class="fas fa-bath mr-1 text-indigo-400"></i> 3 WC</span>
                            <span><i class="fas fa-ruler-combined mr-1 text-indigo-400"></i> 120 m²</span>
                        </div>
                        <p class="text-xs text-gray-400 mt-3">Đăng hôm qua</p>
                    </div>
                </div>

                <div class="property-card bg-white rounded-xl shadow-lg overflow-hidden hover:shadow-2xl transition-shadow duration-300">
                    <a href="property-details.html?id=3" class="block">
                        <img src="https://placehold.co/600x400/e0f2fe/7dd3fc?text=Ảnh+BĐS+3" alt="[Image of Biệt Thự Sân Vườn]" class="w-full h-56 object-cover">
                    </a>
                    <div class="p-6">
                        <div class="flex justify-between items-start mb-2">
                             <a href="property-details.html?id=3" class="block">
                                <h3 class="text-xl font-semibold text-gray-800 hover:text-indigo-600 transition duration-300 leading-tight">Biệt Thự Sân Vườn Gần Công Viên</h3>
                            </a>
                            <button class="text-red-500 hover:text-red-600 text-xl p-1 -mr-1" onclick="toggleFavorite(this)">
                                <i class="fas fa-heart"></i>
                            </button>
                        </div>
                        <p class="text-sm text-gray-500 mb-3"><i class="fas fa-map-marker-alt mr-1 text-indigo-500"></i> Phường Thảo Điền, TP. Thủ Đức</p>
                        <div class="text-2xl font-bold text-indigo-600 mb-3">35 Tỷ VNĐ</div>
                        <div class="flex justify-between text-sm text-gray-600 border-t pt-3">
                            <span><i class="fas fa-bed mr-1 text-indigo-400"></i> 5 PN</span>
                            <span><i class="fas fa-bath mr-1 text-indigo-400"></i> 5 WC</span>
                            <span><i class="fas fa-ruler-combined mr-1 text-indigo-400"></i> 350 m²</span>
                        </div>
                         <p class="text-xs text-gray-400 mt-3">Đăng 3 ngày trước</p>
                    </div>
                </div>
                <div class="property-card bg-white rounded-xl shadow-lg overflow-hidden hover:shadow-2xl transition-shadow duration-300">
                    <a href="property-details.html?id=4" class="block">
                        <img src="https://placehold.co/600x400/fef3c7/fcd34d?text=Ảnh+BĐS+4" alt="[Image of Đất Nền Dự Án]" class="w-full h-56 object-cover">
                    </a>
                    <div class="p-6">
                        <div class="flex justify-between items-start mb-2">
                            <a href="property-details.html?id=4" class="block">
                                <h3 class="text-xl font-semibold text-gray-800 hover:text-indigo-600 transition duration-300 leading-tight">Đất Nền Dự Án Ven Sông</h3>
                            </a>
                            <button class="text-gray-400 hover:text-red-500 text-xl p-1 -mr-1" onclick="toggleFavorite(this)">
                                <i class="far fa-heart"></i>
                            </button>
                        </div>
                        <p class="text-sm text-gray-500 mb-3"><i class="fas fa-map-marker-alt mr-1 text-indigo-500"></i> Huyện Cần Giờ, TP. HCM</p>
                        <div class="text-2xl font-bold text-indigo-600 mb-3">2.5 Tỷ VNĐ</div>
                        <div class="flex justify-between text-sm text-gray-600 border-t pt-3">
                            <span><i class="fas fa-vector-square mr-1 text-indigo-400"></i> Sổ hồng</span>
                            <span><i class="fas fa-road mr-1 text-indigo-400"></i> Đường 12m</span>
                            <span><i class="fas fa-ruler-combined mr-1 text-indigo-400"></i> 100 m²</span>
                        </div>
                        <p class="text-xs text-gray-400 mt-3">Đăng 1 tuần trước</p>
                    </div>
                </div>
                <div class="property-card bg-white rounded-xl shadow-lg overflow-hidden hover:shadow-2xl transition-shadow duration-300">
                    <a href="property-details.html?id=5" class="block">
                        <img src="https://placehold.co/600x400/fee2e2/fca5a5?text=Ảnh+BĐS+5" alt="[Image of Mặt Bằng Kinh Doanh]" class="w-full h-56 object-cover">
                    </a>
                    <div class="p-6">
                        <div class="flex justify-between items-start mb-2">
                            <a href="property-details.html?id=5" class="block">
                                <h3 class="text-xl font-semibold text-gray-800 hover:text-indigo-600 transition duration-300 leading-tight">Mặt Bằng Kinh Doanh Trung Tâm</h3>
                            </a>
                            <button class="text-red-500 hover:text-red-600 text-xl p-1 -mr-1" onclick="toggleFavorite(this)">
                                <i class="fas fa-heart"></i>
                            </button>
                        </div>
                        <p class="text-sm text-gray-500 mb-3"><i class="fas fa-map-marker-alt mr-1 text-indigo-500"></i> Quận 10, TP. HCM</p>
                        <div class="text-2xl font-bold text-indigo-600 mb-3">30 Triệu/tháng</div>
                        <div class="flex justify-between text-sm text-gray-600 border-t pt-3">
                            <span><i class="fas fa-arrows-alt-h mr-1 text-indigo-400"></i> Mặt tiền 5m</span>
                            <span><i class="fas fa-toilet mr-1 text-indigo-400"></i> Lối đi riêng</span>
                            <span><i class="fas fa-ruler-combined mr-1 text-indigo-400"></i> 80 m²</span>
                        </div>
                        <p class="text-xs text-gray-400 mt-3">Đăng 5 ngày trước</p>
                    </div>
                </div>
                <div class="property-card bg-white rounded-xl shadow-lg overflow-hidden hover:shadow-2xl transition-shadow duration-300">
                    <a href="property-details.html?id=6" class="block">
                        <img src="https://placehold.co/600x400/f3e8ff/c084fc?text=Ảnh+BĐS+6" alt="[Image of Căn Hộ Dịch Vụ]" class="w-full h-56 object-cover">
                    </a>
                    <div class="p-6">
                        <div class="flex justify-between items-start mb-2">
                            <a href="property-details.html?id=6" class="block">
                                <h3 class="text-xl font-semibold text-gray-800 hover:text-indigo-600 transition duration-300 leading-tight">Căn Hộ Dịch Vụ Đủ Nội Thất</h3>
                            </a>
                            <button class="text-gray-400 hover:text-red-500 text-xl p-1 -mr-1" onclick="toggleFavorite(this)">
                                <i class="far fa-heart"></i>
                            </button>
                        </div>
                        <p class="text-sm text-gray-500 mb-3"><i class="fas fa-map-marker-alt mr-1 text-indigo-500"></i> Quận Phú Nhuận, TP. HCM</p>
                        <div class="text-2xl font-bold text-indigo-600 mb-3">12 Triệu/tháng</div>
                        <div class="flex justify-between text-sm text-gray-600 border-t pt-3">
                            <span><i class="fas fa-bed mr-1 text-indigo-400"></i> 1 PN</span>
                            <span><i class="fas fa-bath mr-1 text-indigo-400"></i> 1 WC</span>
                            <span><i class="fas fa-ruler-combined mr-1 text-indigo-400"></i> 45 m²</span>
                        </div>
                        <p class="text-xs text-gray-400 mt-3">Đăng hôm nay</p>
                    </div>
                </div>
            </div>

            <div class="text-center mt-12">
                <a href="listings.html" class="bg-indigo-600 hover:bg-indigo-700 text-white font-semibold py-3 px-8 rounded-lg transition duration-300 text-lg">
                    Xem Thêm Tất Cả <i class="fas fa-arrow-right ml-2"></i>
                </a>
            </div>
        </div>
    </section>

    <section class="py-12 md:py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-gray-800 mb-3 text-center">Tại Sao Chọn HomeHub?</h2>
            <p class="text-gray-600 text-center mb-10 max-w-xl mx-auto">Nền tảng tin cậy, đa dạng lựa chọn và hỗ trợ tận tâm.</p>
            <div class="grid md:grid-cols-3 gap-8 text-center">
                <div class="p-6">
                    <div class="text-indigo-600 text-5xl mb-4"><i class="fas fa-check-circle"></i></div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Tin Đăng Xác Thực</h3>
                    <p class="text-gray-600">Mọi tin đăng đều được kiểm duyệt kỹ lưỡng, đảm bảo thông tin chính xác và minh bạch.</p>
                </div>
                <div class="p-6">
                    <div class="text-indigo-600 text-5xl mb-4"><i class="fas fa-search-dollar"></i></div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Giá Tốt Nhất</h3>
                    <p class="text-gray-600">Kết nối trực tiếp với chính chủ, không qua trung gian, giúp bạn có được mức giá ưu đãi.</p>
                </div>
                <div class="p-6">
                    <div class="text-indigo-600 text-5xl mb-4"><i class="fas fa-headset"></i></div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Hỗ Trợ 24/7</h3>
                    <p class="text-gray-600">Đội ngũ hỗ trợ chuyên nghiệp luôn sẵn sàng giải đáp mọi thắc mắc của bạn.</p>
                </div>
            </div>
        </div>
    </section>

    <footer class="bg-gray-800 text-gray-300 py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8 mb-8">
                <div>
                    <h5 class="text-xl font-semibold text-white mb-4">HomeHub</h5>
                    <p class="text-sm">Nền tảng kết nối mua bán, cho thuê bất động sản chính chủ hàng đầu Việt Nam.</p>
                    <div class="mt-4 flex space-x-3">
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300"><i class="fab fa-facebook-f text-xl"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300"><i class="fab fa-youtube text-xl"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300"><i class="fab fa-tiktok text-xl"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300"><i class="fab fa-instagram text-xl"></i></a>
                    </div>
                </div>
                <div>
                    <h5 class="text-lg font-semibold text-white mb-4">Về HomeHub</h5>
                    <ul class="space-y-2 text-sm">
                        <li><a href="about.html" class="hover:text-indigo-400 transition duration-300">Giới thiệu</a></li>
                        <li><a href="contact.html" class="hover:text-indigo-400 transition duration-300">Liên hệ</a></li>
                        <li><a href="#" class="hover:text-indigo-400 transition duration-300">Tuyển dụng</a></li>
                        <li><a href="blog.html" class="hover:text-indigo-400 transition duration-300">Blog Tin Tức</a></li>
                    </ul>
                </div>
                <div>
                    <h5 class="text-lg font-semibold text-white mb-4">Hỗ Trợ Khách Hàng</h5>
                    <ul class="space-y-2 text-sm">
                        <li><a href="faq.html" class="hover:text-indigo-400 transition duration-300">Câu hỏi thường gặp</a></li>
                        <li><a href="guide.html" class="hover:text-indigo-400 transition duration-300">Hướng dẫn đăng tin</a></li>
                        <li><a href="#" class="hover:text-indigo-400 transition duration-300">Báo lỗi</a></li>
                        <li><a href="privacy.html" class="hover:text-indigo-400 transition duration-300">Chính sách bảo mật</a></li>
                        <li><a href="terms.html" class="hover:text-indigo-400 transition duration-300">Điều khoản sử dụng</a></li>
                    </ul>
                </div>
                <div>
                    <h5 class="text-lg font-semibold text-white mb-4">Đăng Ký Nhận Tin</h5>
                    <p class="text-sm mb-3">Nhận thông tin mới nhất về thị trường và các ưu đãi đặc biệt từ HomeHub.</p>
                    <form id="subscribe-form" class="flex">
                        <input type="email" id="subscribe-email" name="email" placeholder="Email của bạn" class="w-full p-2 rounded-l-md text-gray-800 focus:outline-none focus:ring-2 focus:ring-indigo-500" required>
                        <button type="submit" class="bg-indigo-600 hover:bg-indigo-700 text-white p-2 px-4 rounded-r-md transition duration-300">Gửi</button>
                    </form>
                    <p id="subscribe-message" class="text-sm mt-2"></p>
                    <div class="mt-4">
                        <h5 class="text-sm font-semibold text-white mb-2">Tải Ứng Dụng HomeHub</h5>
                        <div class="flex space-x-2">
                            <a href="#" class="bg-gray-700 hover:bg-gray-600 p-2 rounded-md inline-block"><img src="https://placehold.co/120x40/ffffff/000000?text=App+Store" alt="[Image of Tải từ App Store]" class="h-8"></a>
                            <a href="#" class="bg-gray-700 hover:bg-gray-600 p-2 rounded-md inline-block"><img src="https://placehold.co/120x40/ffffff/000000?text=Google+Play" alt="[Image of Tải từ Google Play]" class="h-8"></a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="border-t border-gray-700 pt-8 text-center text-sm">
                <p>&copy; <span id="current-year"></span> HomeHub. Bảo lưu mọi quyền.</p>
                <p>Địa chỉ: 123 Đường ABC, Phường XYZ, Quận LMN, TP. Hồ Chí Minh</p>
            </div>
        </div>
    </footer>

    <script>
        document.getElementById('current-year').textContent = new Date().getFullYear();

        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
            const icon = mobileMenuButton.querySelector('i');
            if (mobileMenu.classList.contains('hidden')) {
                icon.classList.remove('fa-times');
                icon.classList.add('fa-bars');
            } else {
                icon.classList.remove('fa-bars');
                icon.classList.add('fa-times');
            }
        });

        const mobileMenuLinks = mobileMenu.querySelectorAll('a');
        mobileMenuLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
                const icon = mobileMenuButton.querySelector('i');
                icon.classList.remove('fa-times');
                icon.classList.add('fa-bars');
            });
        });
        
        function toggleFavorite(button) {
            const icon = button.querySelector('i');
            icon.classList.toggle('far'); // regular heart
            icon.classList.toggle('fas'); // solid heart
            if (icon.classList.contains('fas')) {
                button.classList.remove('text-gray-400');
                button.classList.add('text-red-500');
            } else {
                button.classList.remove('text-red-500');
                button.classList.add('text-gray-400');
            }
        }

        const subscribeForm = document.getElementById('subscribe-form');
        const subscribeMessage = document.getElementById('subscribe-message');
        if (subscribeForm) {
            subscribeForm.addEventListener('submit', function(e) {
                e.preventDefault();
                const email = document.getElementById('subscribe-email').value;
                if (email) {
                    subscribeMessage.textContent = 'Cảm ơn bạn đã đăng ký!';
                    subscribeMessage.className = 'text-sm mt-2 text-green-400';
                    document.getElementById('subscribe-email').value = ''; 
                } else {
                    subscribeMessage.textContent = 'Vui lòng nhập email hợp lệ.';
                    subscribeMessage.className = 'text-sm mt-2 text-red-400';
                }
                setTimeout(() => {
                    subscribeMessage.textContent = '';
                }, 3000);
            });
        }
    </script>

</body>
</html>
