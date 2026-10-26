<!DOCTYPE html>
<html lang="vi" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON | acondn.vn - Chuẩn Flatsome UX Builder</title>
    <meta name="description" content="Công ty Cổ phần Đầu tư Xây dựng ACON (acondn.vn) - Tổng thầu Thiết kế & Thi công xây dựng tại Đà Nẵng. Địa chỉ: 145-147 Trung Lương 14, Hòa Xuân, Đà Nẵng. SĐT: 0916.104.099">

    <!-- Google Fonts: Montserrat & Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Montserrat:wght@600;700;800;900&display=swap" rel="stylesheet">
    
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    
    <!-- Tailwind CDN (Hỗ trợ hiển thị công cụ UX Toolbar) -->
    <script src="https://cdn.tailwindcss.com"></script>

    <!-- =========================================================================
         [PHẦN 1: CSS CHUẨN FLATSOME] 
         👉 KHI ĐƯA LÊN WORDPRESS: Copy toàn bộ nội dung trong thẻ <style id="flatsome-custom-css"> 
         dán vào: Giao diện (Appearance) -> Tùy biến (Customize) -> Style -> Custom CSS 
         (hoặc Flatsome -> Advanced -> Custom CSS)
    ========================================================================== -->
    <style id="flatsome-custom-css">
        /* ==========================================
           1. BIẾN MÀU SẮC THƯƠNG HIỆU ACON (TƯƠNG TỰ NEWTECONS)
        =========================================== */
        :root {
            --acon-navy: #002B5B;
            --acon-blue: #0054A6;
            --acon-cyan: #0095DA;
            --acon-red: #E31837;
            --acon-gold: #F59E0B;
            --acon-dark: #0A192F;
            --acon-light: #F4F7FA;
            --acon-text: #1E293B;
        }

        .acon-wrapper {
            font-family: 'Inter', sans-serif;
            color: var(--acon-text);
            line-height: 1.6;
            overflow-x: hidden;
            background: #ffffff;
        }

        .acon-wrapper h1, .acon-wrapper h2, .acon-wrapper h3, 
        .acon-wrapper h4, .acon-wrapper .font-heading {
            font-family: 'Montserrat', sans-serif;
        }

        /* ==========================================
           2. HỆ THỐNG GRID CHUẨN FLATSOME (.section, .row, .col, .col-inner)
           (Tự động tương thích với core Flatsome hoặc chạy độc lập)
        =========================================== */
        .acon-wrapper .section {
            position: relative;
            width: 100%;
            padding: 85px 0;
            display: flex;
            align-items: center;
        }

        .acon-wrapper .section-bg {
            position: absolute;
            inset: 0;
            z-index: 0;
            overflow: hidden;
        }

        .acon-wrapper .section-content {
            position: relative;
            z-index: 2;
            width: 100%;
        }

        .acon-wrapper .row {
            width: 100%;
            max-width: 1280px;
            margin: 0 auto;
            display: flex;
            flex-wrap: wrap;
            padding: 0 15px;
        }

        .acon-wrapper .row-collapse {
            padding: 0;
        }

        .acon-wrapper .col {
            padding: 0 15px 30px;
            width: 100%;
            box-sizing: border-box;
        }

        .acon-wrapper .col-inner {
            position: relative;
            height: 100%;
            width: 100%;
        }

        /* Flatsome Responsive Columns */
        @media (min-width: 550px) {
            .acon-wrapper .medium-6 { max-width: 50%; flex-basis: 50%; }
            .acon-wrapper .medium-4 { max-width: 33.3333%; flex-basis: 33.3333%; }
            .acon-wrapper .medium-3 { max-width: 25%; flex-basis: 25%; }
        }
        @media (min-width: 850px) {
            .acon-wrapper .large-12 { max-width: 100%; flex-basis: 100%; }
            .acon-wrapper .large-8 { max-width: 66.6667%; flex-basis: 66.6667%; }
            .acon-wrapper .large-7 { max-width: 58.3333%; flex-basis: 58.3333%; }
            .acon-wrapper .large-6 { max-width: 50%; flex-basis: 50%; }
            .acon-wrapper .large-5 { max-width: 41.6667%; flex-basis: 41.6667%; }
            .acon-wrapper .large-4 { max-width: 33.3333%; flex-basis: 33.3333%; }
            .acon-wrapper .large-3 { max-width: 25%; flex-basis: 25%; }
        }

        /* ==========================================
           3. HIỆU ỨNG ĐẶC TRƯNG KIỂU NEWTECONS (newtecons.vn)
        =========================================== */
        /* Lưới kỹ thuật kiến trúc (Blueprint Grid) */
        .acon-bg-blueprint {
            background-image: 
                linear-gradient(to right, rgba(0, 84, 166, 0.05) 1px, transparent 1px),
                linear-gradient(to bottom, rgba(0, 84, 166, 0.05) 1px, transparent 1px);
            background-size: 48px 48px;
        }

        .acon-bg-blueprint-dark {
            background-image: 
                linear-gradient(to right, rgba(255, 255, 255, 0.04) 1px, transparent 1px),
                linear-gradient(to bottom, rgba(255, 255, 255, 0.04) 1px, transparent 1px);
            background-size: 54px 54px;
        }

        /* Chữ chìm viền (Stroke Watermark Text) */
        .acon-watermark {
            font-family: 'Montserrat', sans-serif;
            font-weight: 900;
            font-size: clamp(60px, 9vw, 125px);
            line-height: 1;
            -webkit-text-stroke: 1.5px rgba(0, 84, 166, 0.12);
            color: transparent;
            user-select: none;
            pointer-events: none;
        }
        .acon-watermark-light {
            -webkit-text-stroke: 1.5px rgba(255, 255, 255, 0.12);
        }

        /* Hiệu ứng Zoom chậm Ken Burns cho Banner Hero */
        @keyframes aconKenBurns {
            0% { transform: scale(1); }
            50% { transform: scale(1.08); }
            100% { transform: scale(1); }
        }
        .acon-kenburns {
            animation: aconKenBurns 18s ease-in-out infinite;
        }

        /* Nút bấm hiệu ứng quét sáng Newtecons */
        .acon-btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 14px 28px;
            border-radius: 14px;
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            font-size: 13px;
            text-transform: uppercase;
            letter-spacing: 0.06em;
            transition: all 0.35s ease;
            position: relative;
            overflow: hidden;
            cursor: pointer;
            text-decoration: none;
        }
        .acon-btn-primary {
            background: var(--acon-cyan);
            color: #ffffff;
            box-shadow: 0 10px 25px -5px rgba(0, 149, 218, 0.4);
        }
        .acon-btn-primary:hover {
            background: var(--acon-blue);
            transform: translateY(-2px);
        }
        .acon-btn-outline {
            background: rgba(255, 255, 255, 0.1);
            color: #ffffff;
            border: 1px solid rgba(255, 255, 255, 0.3);
            backdrop-filter: blur(8px);
        }
        .acon-btn-outline:hover {
            background: #ffffff;
            color: var(--acon-navy);
        }

        /* Hiệu ứng 4 Cột Lĩnh vực hoạt động mở rộng khi Rê chuột (Newtecons Accordion Pillars) */
        .acon-pillars-wrap {
            display: flex;
            flex-direction: column;
            gap: 16px;
            min-height: 470px;
        }
        .acon-pillar-item {
            position: relative;
            flex: 1;
            min-height: 300px;
            border-radius: 24px;
            overflow: hidden;
            border: 1px solid rgba(255,255,255,0.15);
            transition: flex 0.6s cubic-bezier(0.25, 1, 0.5, 1), transform 0.4s ease;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            padding: 28px;
            color: #fff;
        }
        @media (min-width: 992px) {
            .acon-pillars-wrap {
                flex-direction: row;
            }
            .acon-pillar-item {
                min-height: 470px;
            }
            .acon-pillars-wrap:hover .acon-pillar-item {
                flex: 1;
            }
            .acon-pillars-wrap .acon-pillar-item:hover {
                flex: 2.3;
            }
        }
        .acon-pillar-bg {
            position: absolute;
            inset: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: 0;
            transition: transform 0.7s ease;
        }
        .acon-pillar-item:hover .acon-pillar-bg {
            transform: scale(1.1);
        }
        .acon-pillar-overlay {
            position: absolute;
            inset: 0;
            background: linear-gradient(to top, rgba(10, 25, 47, 0.96) 0%, rgba(0, 43, 91, 0.72) 55%, rgba(0, 43, 91, 0.3) 100%);
            z-index: 1;
            transition: background 0.4s ease;
        }
        .acon-pillar-item:hover .acon-pillar-overlay {
            background: linear-gradient(to top, rgba(0, 43, 91, 0.98) 0%, rgba(0, 84, 166, 0.78) 60%, rgba(0, 149, 218, 0.25) 100%);
        }

        /* Card Dự Án (Flatsome Box-Push / Newtecons Overlay) */
        .acon-project-box {
            position: relative;
            height: 390px;
            border-radius: 24px;
            overflow: hidden;
            box-shadow: 0 12px 30px rgba(0, 43, 91, 0.1);
            background: var(--acon-navy);
        }
        .acon-project-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.7s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .acon-project-box:hover img {
            transform: scale(1.09);
        }
        .acon-project-overlay {
            position: absolute;
            inset: 0;
            padding: 26px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            color: #ffffff;
            background: linear-gradient(to top, rgba(0, 43, 91, 0.95) 0%, rgba(0, 43, 91, 0.45) 55%, rgba(0, 43, 91, 0.1) 100%);
            transition: all 0.4s ease;
        }
        .acon-project-box:hover .acon-project-overlay {
            background: linear-gradient(to top, rgba(0, 43, 91, 0.98) 0%, rgba(0, 84, 166, 0.75) 65%, rgba(0, 149, 218, 0.2) 100%);
        }

        /* Thanh điều hướng số 01 - 07 bên phải (Newtecons Fixed Dot Nav) */
        .acon-side-nav .nav-dot.active .dot-line {
            width: 34px;
            background-color: var(--acon-cyan);
        }
        .acon-side-nav .nav-dot.active .dot-num {
            color: var(--acon-cyan);
            font-weight: 800;
            transform: scale(1.15);
        }

        /* Hiệu ứng khi bật chế độ "UX Live Edit" để sửa trực tiếp */
        body.ux-edit-mode [contenteditable="true"] {
            outline: 2px dashed rgba(0, 149, 218, 0.7);
            outline-offset: 3px;
            border-radius: 4px;
            cursor: text;
        }
        body.ux-edit-mode [contenteditable="true"]:focus {
            outline: 2px solid #E31837;
            background-color: rgba(0, 149, 218, 0.08);
        }
        body.ux-edit-mode img {
            cursor: pointer;
            outline: 2px dashed #F59E0B;
            outline-offset: -4px;
        }
        body.ux-edit-mode .ux-section-toolbar {
            display: flex !important;
        }
    </style>
</head>
<body class="bg-white">

    <!-- =========================================================================
         [THANH CÔNG CỤ HỖ TRỢ FLATSOME UX BUILDER - KHÔNG COPY PHẦN NÀY VÀO WEB]
         Giúp bạn:
         1. Bật chế độ sửa trực tiếp chữ & ảnh ngay trên màn hình
         2. Copy từng Section (HTML hoặc UX Builder Shortcode)
         3. Copy toàn bộ CSS dán vào Flatsome -> Custom CSS
    ========================================================================== -->
    <div id="ux-builder-helper" class="fixed bottom-4 right-4 left-4 md:left-auto z-50 bg-[#0A192F]/95 backdrop-blur-md text-white px-4 py-3 rounded-2xl shadow-2xl border border-sky-500/40 flex flex-wrap items-center gap-2.5 text-xs">
        <div class="flex items-center gap-2 pr-2 border-r border-white/15">
            <span class="w-2.5 h-2.5 rounded-full bg-emerald-400 animate-pulse"></span>
            <strong class="font-bold text-sky-400 uppercase tracking-wider">Flatsome UX Tool:</strong>
        </div>

        <button onclick="toggleUxLiveEdit()" id="btn-live-edit" class="px-3.5 py-2 rounded-xl bg-amber-500 hover:bg-amber-600 text-slate-950 font-bold transition-all flex items-center gap-1.5 shadow">
            <i class="fa-solid fa-pen-to-square"></i>
            <span>Bật Sửa Trực Tiếp Chữ & Ảnh</span>
        </button>

        <button onclick="copyFlatsomeCSS()" class="px-3.5 py-2 rounded-xl bg-sky-600 hover:bg-sky-500 text-white font-semibold transition-all flex items-center gap-1.5">
            <i class="fa-brands fa-css3-alt"></i>
            <span>1. Copy CSS</span>
        </button>

        <button onclick="copyAllFlatsomeHTML()" class="px-3.5 py-2 rounded-xl bg-indigo-600 hover:bg-indigo-500 text-white font-semibold transition-all flex items-center gap-1.5">
            <i class="fa-solid fa-code"></i>
            <span>2. Copy Toàn Bộ HTML</span>
        </button>

        <button onclick="copyFlatsomeShortcode()" class="px-3.5 py-2 rounded-xl bg-emerald-600 hover:bg-emerald-500 text-white font-semibold transition-all flex items-center gap-1.5" title="Copy mã Shortcode [section] [row] [col] để dán thẳng vào UX Builder">
            <i class="fa-solid fa-wand-magic-sparkles"></i>
            <span>3. Copy UX Shortcode</span>
        </button>

        <button onclick="openGuideModal()" class="px-3 py-2 rounded-xl bg-white/10 hover:bg-white/20 text-white font-semibold transition-all" title="Hướng dẫn dán vào WordPress Flatsome">
            <i class="fa-solid fa-circle-question"></i>
        </button>
    </div>

    <!-- Thông báo Toast khi Copy hoặc Sửa thành công -->
    <div id="ux-toast" class="fixed top-24 right-6 z-50 hidden bg-emerald-600 text-white px-5 py-3.5 rounded-2xl shadow-2xl border border-white/20 text-xs sm:text-sm font-semibold items-center gap-2.5">
        <i class="fa-solid fa-circle-check text-lg"></i>
        <span id="ux-toast-msg">Đã sao chép vào bộ nhớ tạm!</span>
    </div>

    <!-- =========================================================================
         [PHẦN 2: NỘI DUNG HTML CHUẨN FLATSOME CỦA WEBSITE ACONDN.VN]
         👉 Mọi nội dung dưới đây đều là HTML tĩnh 100%, bạn có thể sửa trực tiếp 
         trong code hoặc bật nút "Bật Sửa Trực Tiếp Chữ & Ảnh" ở góc dưới màn hình.
    ========================================================================== -->
    <div id="flatsome-export-area" class="acon-wrapper">

        <!-- ==========================================
             FLOATING RIGHT-SIDE PAGINATION (01 - 07)
        =========================================== -->
        <aside class="acon-side-nav fixed right-4 xl:right-6 top-1/2 -translate-y-1/2 z-40 hidden md:flex flex-col gap-2.5 bg-[#002B5B]/85 backdrop-blur-md px-3 py-4 rounded-2xl border border-white/15 shadow-xl">
            <a href="#sec-01" data-sec="sec-01" class="nav-dot active flex items-center justify-end gap-2 py-1 text-white/70 hover:text-white no-underline">
                <span class="dot-num text-xs font-heading font-bold transition-all">01</span>
                <span class="dot-line w-4 h-[2px] bg-white/40 rounded-full transition-all"></span>
            </a>
            <a href="#sec-02" data-sec="sec-02" class="nav-dot flex items-center justify-end gap-2 py-1 text-white/70 hover:text-white no-underline">
                <span class="dot-num text-xs font-heading font-bold transition-all">02</span>
                <span class="dot-line w-4 h-[2px] bg-white/40 rounded-full transition-all"></span>
            </a>
            <a href="#sec-03" data-sec="sec-03" class="nav-dot flex items-center justify-end gap-2 py-1 text-white/70 hover:text-white no-underline">
                <span class="dot-num text-xs font-heading font-bold transition-all">03</span>
                <span class="dot-line w-4 h-[2px] bg-white/40 rounded-full transition-all"></span>
            </a>
            <a href="#sec-04" data-sec="sec-04" class="nav-dot flex items-center justify-end gap-2 py-1 text-white/70 hover:text-white no-underline">
                <span class="dot-num text-xs font-heading font-bold transition-all">04</span>
                <span class="dot-line w-4 h-[2px] bg-white/40 rounded-full transition-all"></span>
            </a>
            <a href="#sec-05" data-sec="sec-05" class="nav-dot flex items-center justify-end gap-2 py-1 text-white/70 hover:text-white no-underline">
                <span class="dot-num text-xs font-heading font-bold transition-all">05</span>
                <span class="dot-line w-4 h-[2px] bg-white/40 rounded-full transition-all"></span>
            </a>
            <a href="#sec-06" data-sec="sec-06" class="nav-dot flex items-center justify-end gap-2 py-1 text-white/70 hover:text-white no-underline">
                <span class="dot-num text-xs font-heading font-bold transition-all">06</span>
                <span class="dot-line w-4 h-[2px] bg-white/40 rounded-full transition-all"></span>
            </a>
            <a href="#sec-07" data-sec="sec-07" class="nav-dot flex items-center justify-end gap-2 py-1 text-white/70 hover:text-white no-underline">
                <span class="dot-num text-xs font-heading font-bold transition-all">07</span>
                <span class="dot-line w-4 h-[2px] bg-white/40 rounded-full transition-all"></span>
            </a>
        </aside>

        <!-- ==========================================
             FLOATING HOTLINE & FANPAGE BUTTONS
        =========================================== -->
        <div class="fixed left-4 bottom-5 z-40 flex flex-col gap-2.5">
            <a href="tel:0916104099" class="flex items-center gap-3 bg-[#E31837] text-white px-4 py-2.5 rounded-full shadow-lg hover:bg-red-700 transition-all no-underline">
                <span class="w-8 h-8 rounded-full bg-white/20 flex items-center justify-center">
                    <i class="fa-solid fa-phone-volume text-sm"></i>
                </span>
                <div class="pr-1">
                    <span class="block text-[10px] uppercase tracking-wider text-white/80 leading-none">Hotline 24/7</span>
                    <span class="font-heading font-bold text-sm editable-text">0916.104.099</span>
                </div>
            </a>
            <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="flex items-center gap-2.5 bg-[#1877F2] text-white px-4 py-2 rounded-full shadow-lg hover:bg-blue-700 transition-all no-underline">
                <i class="fa-brands fa-facebook-f text-base w-5 text-center"></i>
                <span class="text-xs font-semibold pr-1 hidden sm:inline editable-text">Fanpage ACON Construction</span>
            </a>
        </div>

        <!-- ==========================================
             HEADER FLATSOME (TOP BAR + MAIN HEADER)
        =========================================== -->
        <header id="header" class="fixed top-0 left-0 right-0 z-40 bg-[#002B5B]/95 backdrop-blur-md border-b border-white/10">
            <!-- Top Bar -->
            <div class="bg-[#0A192F] text-white/80 text-xs py-1.5 px-4 border-b border-white/10 hidden lg:block">
                <div class="max-w-7xl mx-auto flex items-center justify-between">
                    <div class="flex items-center gap-6">
                        <span class="editable-text"><i class="fa-solid fa-globe text-[#0095DA] mr-1"></i> <strong>acondn.vn</strong> — CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON</span>
                        <span class="editable-text"><i class="fa-solid fa-location-dot text-[#E31837] mr-1"></i> 145-147 Trung Lương 14, Hòa Xuân, Đà Nẵng</span>
                        <span class="editable-text"><i class="fa-solid fa-certificate text-amber-400 mr-1"></i> Chứng chỉ HĐXD: <strong>00076275</strong> | MST: <strong>0401676571</strong></span>
                    </div>
                    <div class="flex items-center gap-5">
                        <a href="mailto:acon.dng@gmail.com" class="hover:text-[#0095DA] text-white/80 no-underline editable-text">
                            <i class="fa-regular fa-envelope mr-1"></i> acon.dng@gmail.com
                        </a>
                        <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="hover:text-[#0095DA] text-white/80 no-underline">
                            <i class="fa-brands fa-facebook text-blue-400 mr-1"></i> fb.com/aconvn.construction
                        </a>
                    </div>
                </div>
            </div>

            <!-- Main Nav Bar -->
            <div class="max-w-7xl mx-auto px-4 h-20 flex items-center justify-between">
                <!-- Logo ACON (Có thể click trực tiếp vào ảnh logo để đổi link ảnh từ Fanpage) -->
                <a href="#sec-01" class="flex items-center gap-3 no-underline">
                    <div class="w-14 h-14 rounded-xl bg-white flex items-center justify-center p-1.5 shadow border-2 border-[#0095DA]/40 overflow-hidden">
                        <!-- Đổi src ảnh dưới đây thành link ảnh Logo trên WordPress Media của bạn -->
                        <img src="https://placehold.co/160x160/ffffff/002B5B?text=ACON+JSC" 
                             alt="Logo Công ty Cổ phần Đầu tư Xây dựng ACON" 
                             class="w-full h-full object-contain editable-img" />
                    </div>
                    <div>
                        <div class="flex items-center gap-1.5">
                            <span class="font-heading font-black text-2xl sm:text-3xl tracking-wider text-white leading-none editable-text">
                                <span class="text-[#0095DA]">Λ</span>CON
                            </span>
                            <span class="text-[10px] font-heading font-bold uppercase px-1.5 py-0.5 rounded bg-[#E31837] text-white editable-text">JSC</span>
                        </div>
                        <span class="block text-[10px] sm:text-[11px] font-semibold tracking-widest text-white/80 uppercase mt-0.5 editable-text">
                            Đầu Tư Xây Dựng ACON • acondn.vn
                        </span>
                    </div>
                </a>

                <!-- Menu chính -->
                <nav class="hidden xl:flex items-center gap-6 text-xs font-heading font-bold text-white uppercase tracking-wider">
                    <a href="#sec-02" class="hover:text-[#0095DA] transition-colors no-underline editable-text">Giới thiệu</a>
                    <a href="#sec-03" class="hover:text-[#0095DA] transition-colors no-underline editable-text">Lĩnh vực hoạt động</a>
                    <a href="#sec-04" class="hover:text-[#0095DA] transition-colors no-underline editable-text">Năng lực & Chứng chỉ</a>
                    <a href="#sec-05" class="hover:text-[#0095DA] transition-colors no-underline editable-text">Dự án tiêu biểu</a>
                    <a href="#sec-06" class="hover:text-[#0095DA] transition-colors no-underline editable-text">Tin tức & Tuyển dụng</a>
                    <a href="#sec-07" class="hover:text-[#0095DA] transition-colors no-underline editable-text">Liên hệ</a>
                </nav>

                <!-- Hotline Button -->
                <div class="flex items-center gap-3">
                    <a href="tel:0916104099" class="acon-btn acon-btn-primary !py-2.5 !px-4 !text-xs">
                        <i class="fa-solid fa-phone"></i>
                        <span class="editable-text">0916.104.099</span>
                    </a>
                </div>
            </div>
        </header>


        <!-- =====================================================================
             [FLATSOME SECTION 01: HERO SLIDER KIỂU NEWTECONS]
             Có thể sửa trực tiếp cả 3 Slide trong HTML bên dưới
        ====================================================================== -->
        <section class="section !p-0 min-h-screen bg-[#0A192F] text-white relative overflow-hidden" id="sec-01">
            <!-- Thanh Copy nhanh Section 01 khi bật chế độ UX Edit -->
            <div class="ux-section-toolbar hidden absolute top-28 right-8 z-30 gap-2">
                <button onclick="copySingleSection('sec-01')" class="bg-sky-500 text-white text-xs font-bold px-3 py-1.5 rounded-lg shadow">Copy HTML Section 01</button>
            </div>

            <!-- Background Slides (3 Slide viết trực tiếp bằng HTML dễ sửa ảnh) -->
            <div class="section-bg">
                <!-- Ảnh nền Slide 1 -->
                <div class="acon-hero-slide absolute inset-0 transition-opacity duration-1000 opacity-100" data-slide="0">
                    <img src="https://images.unsplash.com/photo-1541888946425-d09bb18086f6?auto=format&fit=crop&w=1920&q=85" 
                         alt="Tổng thầu Thiết kế và Thi công ACON Đà Nẵng" 
                         class="w-full h-full object-cover acon-kenburns editable-img" />
                    <div class="absolute inset-0 bg-gradient-to-r from-[#0A192F]/95 via-[#002B5B]/80 to-[#0A192F]/40"></div>
                </div>
                <!-- Ảnh nền Slide 2 -->
                <div class="acon-hero-slide absolute inset-0 transition-opacity duration-1000 opacity-0" data-slide="1">
                    <img src="https://images.unsplash.com/photo-1503387762-592deb58ef4e?auto=format&fit=crop&w=1920&q=85" 
                         alt="Công trình tiêu biểu ACON Construction" 
                         class="w-full h-full object-cover acon-kenburns editable-img" />
                    <div class="absolute inset-0 bg-gradient-to-r from-[#0A192F]/95 via-[#002B5B]/80 to-[#0A192F]/40"></div>
                </div>
                <!-- Ảnh nền Slide 3 -->
                <div class="acon-hero-slide absolute inset-0 transition-opacity duration-1000 opacity-0" data-slide="2">
                    <img src="https://images.unsplash.com/photo-1581094794329-c8112a89af12?auto=format&fit=crop&w=1920&q=85" 
                         alt="Đội ngũ kỹ sư ACON tại Hòa Xuân Đà Nẵng" 
                         class="w-full h-full object-cover acon-kenburns editable-img" />
                    <div class="absolute inset-0 bg-gradient-to-r from-[#0A192F]/95 via-[#002B5B]/80 to-[#0A192F]/40"></div>
                </div>
                <div class="absolute inset-0 acon-bg-blueprint-dark pointer-events-none"></div>
            </div>

            <!-- Chữ chìm kiến trúc góc phải -->
            <div class="absolute bottom-20 right-10 hidden lg:block z-10">
                <span class="acon-watermark acon-watermark-light editable-text">ACON D&B</span>
            </div>

            <!-- Nội dung chính trong .row > .col chuẩn Flatsome -->
            <div class="section-content pt-32 pb-20">
                <div class="row">
                    <div class="col large-8 small-12">
                        <div class="col-inner">
                            <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-white/10 border border-white/20 text-xs font-bold uppercase tracking-widest mb-6">
                                <span class="w-2 h-2 rounded-full bg-[#0095DA]"></span>
                                <span class="editable-text">BUILD ON TRUST • KIẾN TẠO GIÁ TRỊ VỮNG BỀN</span>
                            </div>

                            <h1 class="font-heading font-black text-3xl sm:text-5xl lg:text-6xl leading-tight mb-6 editable-text">
                                CÔNG TY CỔ PHẦN <br/>
                                <span class="text-[#0095DA]">ĐẦU TƯ XÂY DỰNG ACON</span>
                            </h1>

                            <p class="text-base sm:text-lg text-white/85 leading-relaxed mb-8 max-w-2xl editable-text">
                                Sự tin tưởng của Chủ đầu tư là chuẩn mực cho giá trị của ACON Construction (acondn.vn). Chúng tôi tự hào là Tổng thầu Thiết kế & Thi công (Design & Build) các công trình Dân dụng, Thương mại, Khách sạn và Công nghiệp uy tín hàng đầu tại Đà Nẵng & khu vực Miền Trung.
                            </p>

                            <div class="flex flex-wrap gap-4 mb-10">
                                <a href="#sec-05" class="acon-btn acon-btn-primary editable-text">
                                    Khám phá Dự án ACON <i class="fa-solid fa-arrow-right"></i>
                                </a>
                                <a href="#sec-04" class="acon-btn acon-btn-outline editable-text">
                                    <i class="fa-solid fa-award text-amber-400"></i> Hồ sơ năng lực (00076275)
                                </a>
                            </div>

                            <!-- Nút chuyển Slide 01 - 02 - 03 -->
                            <div class="flex items-center gap-6 pt-6 border-t border-white/15">
                                <button onclick="changeHeroSlide(0)" class="flex items-center gap-2 text-xs font-heading font-bold text-[#0095DA]">
                                    <span>01</span>
                                    <span class="w-12 h-1 bg-[#0095DA] rounded-full"></span>
                                    <span class="editable-text">Tổng thầu D&B</span>
                                </button>
                                <button onclick="changeHeroSlide(1)" class="flex items-center gap-2 text-xs font-heading font-bold text-white/70 hover:text-white">
                                    <span>02</span>
                                    <span class="w-12 h-1 bg-white/30 rounded-full"></span>
                                    <span class="editable-text">Công trình Biểu tượng</span>
                                </button>
                                <button onclick="changeHeroSlide(2)" class="flex items-center gap-2 text-xs font-heading font-bold text-white/70 hover:text-white">
                                    <span>03</span>
                                    <span class="w-12 h-1 bg-white/30 rounded-full"></span>
                                    <span class="editable-text">Chuẩn Kỹ - Mỹ Thuật</span>
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>


        <!-- =====================================================================
             [FLATSOME SECTION 02: GIỚI THIỆU ACON & LỊCH SỬ PHÁT TRIỂN]
             Bố cục 2 cột chuẩn Flatsome: .col.large-6.small-12
        ====================================================================== -->
        <section class="section acon-bg-blueprint bg-white" id="sec-02">
            <div class="ux-section-toolbar hidden absolute top-4 right-8 z-30 gap-2">
                <button onclick="copySingleSection('sec-02')" class="bg-sky-500 text-white text-xs font-bold px-3 py-1.5 rounded-lg shadow">Copy HTML Section 02</button>
            </div>

            <div class="section-content">
                <div class="row items-center">
                    <!-- Cột trái: Giới thiệu -->
                    <div class="col large-6 small-12">
                        <div class="col-inner">
                            <div class="flex items-center gap-3 mb-3">
                                <span class="w-10 h-1 bg-[#0054A6] rounded-full"></span>
                                <span class="font-heading font-bold text-xs uppercase tracking-widest text-[#0054A6] editable-text">02 • VỀ CHÚNG TÔI</span>
                            </div>

                            <h2 class="font-heading font-black text-3xl sm:text-4xl lg:text-5xl text-[#002B5B] mb-3 editable-text">
                                ACON CONSTRUCTION
                            </h2>

                            <p class="font-heading font-bold text-base sm:text-lg text-[#0095DA] mb-5 editable-text">
                                “Build on Trust – Sự tin tưởng của bạn là chuẩn mực cho giá trị của chúng tôi”
                            </p>

                            <div class="space-y-4 text-slate-600 text-sm sm:text-base mb-6">
                                <p class="editable-text">
                                    Được thành lập từ ngày <strong>14/05/2015</strong> (Mã số thuế: <strong>0401676571</strong>), dưới sự điều hành của Giám đốc – Người đại diện pháp luật <strong>Ông Huỳnh Bá Quý</strong> cùng đội ngũ kỹ sư, kiến trúc sư giàu kinh nghiệm, <strong>CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON</strong> đã khẳng định vị thế nhà thầu xây dựng uy tín tại Đà Nẵng và Miền Trung.
                                </p>
                                <p class="editable-text">
                                    Sở hữu Chứng chỉ năng lực hoạt động xây dựng số <strong>00076275</strong> (hiệu lực đến năm 2033), ACON đáp ứng trọn vẹn các lĩnh vực: <strong>Thiết kế, Thẩm tra thiết kế, Tư vấn Quản lý dự án, Tư vấn Giám sát và Thi công xây dựng công trình Dân dụng (Hạng II) & Nhà công nghiệp</strong>.
                                </p>
                            </div>

                            <!-- 4 Cột mốc lịch sử hiển thị trực tiếp để dễ sửa chữ -->
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5 mt-6">
                                <div class="p-4 rounded-2xl bg-slate-50 border-l-4 border-[#0054A6]">
                                    <span class="font-heading font-black text-[#0054A6] text-base editable-text">2015 — Thành lập</span>
                                    <p class="text-xs text-slate-600 mt-1 editable-text">Thành lập ngày 14/05/2015 (MST: 0401676571), khởi đầu thi công dân dụng & nội thất tại Đà Nẵng.</p>
                                </div>
                                <div class="p-4 rounded-2xl bg-slate-50 border-l-4 border-[#0095DA]">
                                    <span class="font-heading font-black text-[#0095DA] text-base editable-text">2019 — Mở rộng quy mô</span>
                                    <p class="text-xs text-slate-600 mt-1 editable-text">Khai trương văn phòng Hòa Xuân, đẩy mạnh thi công khách sạn, biệt thự & nhà xưởng.</p>
                                </div>
                                <div class="p-4 rounded-2xl bg-slate-50 border-l-4 border-amber-500">
                                    <span class="font-heading font-black text-amber-600 text-base editable-text">2023 — Chứng chỉ Hạng II</span>
                                    <p class="text-xs text-slate-600 mt-1 editable-text">Được cấp mã chứng chỉ năng lực HĐXD 00076275 đa lĩnh vực Thiết kế, QLDA, Giám sát & Thi công.</p>
                                </div>
                                <div class="p-4 rounded-2xl bg-slate-50 border-l-4 border-[#E31837]">
                                    <span class="font-heading font-black text-[#E31837] text-base editable-text">2026 — Tổng thầu D&B</span>
                                    <p class="text-xs text-slate-600 mt-1 editable-text">Trụ sở 145-147 Trung Lương 14, Hòa Xuân, Đà Nẵng với đội ngũ kỹ sư, QS, KTS chuyên môn cao.</p>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Cột phải: Hình ảnh trụ sở & đội ngũ -->
                    <div class="col large-6 small-12">
                        <div class="col-inner">
                            <div class="rounded-3xl overflow-hidden shadow-2xl border-4 border-white relative">
                                <img src="https://images.unsplash.com/photo-1504307651254-35680f356dfd?auto=format&fit=crop&w=1000&q=85" 
                                     alt="Đội ngũ kỹ sư Công ty Cổ phần Đầu tư Xây dựng ACON" 
                                     class="w-full h-[460px] object-cover editable-img" />
                                <div class="absolute inset-0 bg-gradient-to-t from-[#002B5B]/95 via-transparent to-transparent pointer-events-none"></div>
                                <div class="absolute bottom-6 left-6 right-6 text-white">
                                    <span class="px-3 py-1 rounded-full bg-[#0095DA] text-xs font-bold uppercase tracking-wider editable-text">Trụ sở Đà Nẵng</span>
                                    <h3 class="font-heading font-bold text-xl mt-2 editable-text">145-147 Trung Lương 14, Phường Hòa Xuân, TP. Đà Nẵng</h3>
                                    <p class="text-xs text-white/80 mt-1 editable-text">Hotline: 0916.104.099 • Điện thoại VP: 02363.789.769 • Website: acondn.vn</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>


        <!-- =====================================================================
             [FLATSOME SECTION 03: LĨNH VỰC HOẠT ĐỘNG - 4 CỘT MỞ RỘNG KIỂU NEWTECONS]
        ====================================================================== -->
        <section class="section bg-[#0A192F] text-white" id="sec-03">
            <div class="ux-section-toolbar hidden absolute top-4 right-8 z-30 gap-2">
                <button onclick="copySingleSection('sec-03')" class="bg-sky-500 text-white text-xs font-bold px-3 py-1.5 rounded-lg shadow">Copy HTML Section 03</button>
            </div>

            <div class="section-content">
                <div class="row">
                    <div class="col large-12 small-12">
                        <div class="col-inner">
                            <div class="flex flex-col md:flex-row md:items-end justify-between gap-4 mb-10">
                                <div>
                                    <div class="flex items-center gap-3 mb-2">
                                        <span class="w-10 h-1 bg-[#0095DA] rounded-full"></span>
                                        <span class="font-heading font-bold text-xs uppercase tracking-widest text-[#0095DA] editable-text">03 • LĨNH VỰC HOẠT ĐỘNG</span>
                                    </div>
                                    <h2 class="font-heading font-black text-3xl sm:text-4xl lg:text-5xl editable-text">
                                        GIẢI PHÁP XÂY DỰNG <span class="text-[#0095DA]">TOÀN DIỆN</span>
                                    </h2>
                                </div>
                                <p class="text-white/75 max-w-xl text-sm sm:text-base editable-text">
                                    Mô hình Tổng thầu Thiết kế & Thi công (Design & Build) kết hợp Quản lý dự án & Giám sát đạt chuẩn Bộ Xây dựng (Mã chứng chỉ 00076275).
                                </p>
                            </div>

                            <!-- 4 Cột mở rộng mượt mà khi rê chuột (Newtecons Expanding Pillars) -->
                            <div class="acon-pillars-wrap">
                                <!-- Cột 1 -->
                                <div class="acon-pillar-item">
                                    <img src="https://images.unsplash.com/photo-1541888946425-d09bb18086f6?auto=format&fit=crop&w=900&q=80" alt="Tổng thầu Thiết kế và Thi công" class="acon-pillar-bg editable-img" />
                                    <div class="acon-pillar-overlay"></div>
                                    <div class="relative z-10 flex items-center justify-between">
                                        <span class="font-heading font-black text-4xl text-white/40">01</span>
                                        <span class="px-3 py-1 rounded-full bg-[#0095DA]/20 border border-[#0095DA] text-[#0095DA] text-xs font-bold editable-text">Mũi nhọn</span>
                                    </div>
                                    <div class="relative z-10">
                                        <h3 class="font-heading font-extrabold text-xl mb-2 editable-text">TỔNG THẦU THIẾT KẾ & THI CÔNG (D&B)</h3>
                                        <p class="text-sm text-white/85 editable-text">
                                            Thiết kế kiến trúc - kết cấu và Thi công xây dựng công trình Dân dụng (Hạng II): Khách sạn, Tòa nhà văn phòng, Khu nghỉ dưỡng, Biệt thự cao cấp.
                                        </p>
                                    </div>
                                </div>

                                <!-- Cột 2 -->
                                <div class="acon-pillar-item">
                                    <img src="https://images.unsplash.com/photo-1581092160607-ee22621dd758?auto=format&fit=crop&w=900&q=80" alt="Thi công Nhà công nghiệp" class="acon-pillar-bg editable-img" />
                                    <div class="acon-pillar-overlay"></div>
                                    <div class="relative z-10 flex items-center justify-between">
                                        <span class="font-heading font-black text-4xl text-white/40">02</span>
                                        <span class="px-3 py-1 rounded-full bg-white/10 text-white text-xs font-bold editable-text">Công nghiệp</span>
                                    </div>
                                    <div class="relative z-10">
                                        <h3 class="font-heading font-extrabold text-xl mb-2 editable-text">THI CÔNG NHÀ CÔNG NGHIỆP & HẠ TẦNG</h3>
                                        <p class="text-sm text-white/85 editable-text">
                                            Thiết kế, thẩm tra và thi công trọn gói Nhà máy sản xuất, Kho vận Logistics, Kết cấu thép tiền chế và hạ tầng KCN tại Đà Nẵng & Miền Trung.
                                        </p>
                                    </div>
                                </div>

                                <!-- Cột 3 -->
                                <div class="acon-pillar-item">
                                    <img src="https://images.unsplash.com/photo-1621905251189-08b45d6a269e?auto=format&fit=crop&w=900&q=80" alt="Thi công Cơ điện M&E và Nội thất" class="acon-pillar-bg editable-img" />
                                    <div class="acon-pillar-overlay"></div>
                                    <div class="relative z-10 flex items-center justify-between">
                                        <span class="font-heading font-black text-4xl text-white/40">03</span>
                                        <span class="px-3 py-1 rounded-full bg-white/10 text-white text-xs font-bold editable-text">M&E • Fit-out</span>
                                    </div>
                                    <div class="relative z-10">
                                        <h3 class="font-heading font-extrabold text-xl mb-2 editable-text">THI CÔNG CƠ ĐIỆN (M&E) & NỘI THẤT</h3>
                                        <p class="text-sm text-white/85 editable-text">
                                            Lắp đặt thiết bị công trình, hệ thống điện, cấp thoát nước, điều hòa thông gió, PCCC và hoàn thiện nội thất văn phòng, khách sạn, showroom.
                                        </p>
                                    </div>
                                </div>

                                <!-- Cột 4 -->
                                <div class="acon-pillar-item">
                                    <img src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?auto=format&fit=crop&w=900&q=80" alt="Tư vấn Quản lý dự án và Giám sát" class="acon-pillar-bg editable-img" />
                                    <div class="acon-pillar-overlay"></div>
                                    <div class="relative z-10 flex items-center justify-between">
                                        <span class="font-heading font-black text-4xl text-white/40">04</span>
                                        <span class="px-3 py-1 rounded-full bg-white/10 text-white text-xs font-bold editable-text">Tư vấn & QS</span>
                                    </div>
                                    <div class="relative z-10">
                                        <h3 class="font-heading font-extrabold text-xl mb-2 editable-text">TƯ VẤN QUẢN LÝ DỰ ÁN & GIÁM SÁT</h3>
                                        <p class="text-sm text-white/85 editable-text">
                                            Tư vấn quản lý dự án đầu tư xây dựng, thẩm tra thiết kế - dự toán (QS) và tư vấn giám sát công trình Dân dụng & Công nghiệp đạt chuẩn.
                                        </p>
                                    </div>
                                </div>
                            </div>

                        </div>
                    </div>
                </div>
            </div>
        </section>


        <!-- =====================================================================
             [FLATSOME SECTION 04: CON SỐ ẤN TƯỢNG & CHỨNG CHỈ NĂNG LỰC 00076275]
             Bố cục 4 cột .col.large-3.medium-6.small-12 chuẩn Flatsome
        ====================================================================== -->
        <section class="section bg-gradient-to-br from-[#002B5B] via-[#0054A6] to-[#0A192F] text-white acon-bg-blueprint-dark" id="sec-04">
            <div class="ux-section-toolbar hidden absolute top-4 right-8 z-30 gap-2">
                <button onclick="copySingleSection('sec-04')" class="bg-sky-500 text-white text-xs font-bold px-3 py-1.5 rounded-lg shadow">Copy HTML Section 04</button>
            </div>

            <div class="section-content">
                <div class="row">
                    <div class="col large-12 small-12 text-center">
                        <div class="col-inner max-w-3xl mx-auto">
                            <span class="inline-block px-4 py-1.5 rounded-full bg-white/10 text-[#0095DA] font-heading font-bold text-xs uppercase tracking-widest mb-3 editable-text">
                                04 • DẤU ẤN & NĂNG LỰC PHÁP LÝ
                            </span>
                            <h2 class="font-heading font-black text-3xl sm:text-4xl lg:text-5xl editable-text">
                                CÙNG NHAU KIẾN TẠO <span class="text-[#0095DA]">CÔNG TRÌNH BIỂU TƯỢNG</span>
                            </h2>
                        </div>
                    </div>

                    <!-- 4 Cột Số Liệu -->
                    <div class="col large-3 medium-6 small-12">
                        <div class="col-inner bg-white/10 backdrop-blur-md border border-white/15 rounded-3xl p-7 text-center">
                            <div class="font-heading font-black text-4xl sm:text-5xl text-[#0095DA] mb-2 editable-text">+11</div>
                            <div class="font-heading font-bold text-sm uppercase tracking-wider editable-text">NĂM HOẠT ĐỘNG</div>
                            <p class="text-xs text-white/70 mt-1 editable-text">Thành lập từ 14/05/2015</p>
                        </div>
                    </div>

                    <div class="col large-3 medium-6 small-12">
                        <div class="col-inner bg-white/10 backdrop-blur-md border border-white/15 rounded-3xl p-7 text-center">
                            <div class="font-heading font-black text-4xl sm:text-5xl text-white mb-2 editable-text">+85</div>
                            <div class="font-heading font-bold text-sm uppercase tracking-wider editable-text">NHÂN SỰ KỸ SƯ & KTS</div>
                            <p class="text-xs text-white/70 mt-1 editable-text">Chỉ huy trưởng, Kỹ sư QS, MEP</p>
                        </div>
                    </div>

                    <div class="col large-3 medium-6 small-12">
                        <div class="col-inner bg-white/10 backdrop-blur-md border border-white/15 rounded-3xl p-7 text-center">
                            <div class="font-heading font-black text-4xl sm:text-5xl text-amber-400 mb-2 editable-text">+120</div>
                            <div class="font-heading font-bold text-sm uppercase tracking-wider editable-text">DỰ ÁN & GÓI THẦU</div>
                            <p class="text-xs text-white/70 mt-1 editable-text">Tại Đà Nẵng & Miền Trung</p>
                        </div>
                    </div>

                    <div class="col large-3 medium-6 small-12">
                        <div class="col-inner bg-white/10 backdrop-blur-md border border-white/15 rounded-3xl p-7 text-center">
                            <div class="font-heading font-black text-3xl sm:text-4xl text-[#E31837] bg-white px-4 py-1.5 rounded-2xl inline-block mb-2 editable-text">HẠNG II</div>
                            <div class="font-heading font-bold text-sm uppercase tracking-wider editable-text">CHỨNG CHỈ NĂNG LỰC</div>
                            <p class="text-xs text-white/70 mt-1 editable-text">Mã số HĐXD: 00076275</p>
                        </div>
                    </div>

                    <!-- Bảng Tóm Tắt Chứng Chỉ Năng Lực Hoạt Động Xây Dựng (Viết trực tiếp bằng HTML) -->
                    <div class="col large-12 small-12">
                        <div class="col-inner bg-white text-slate-800 rounded-3xl p-6 sm:p-8 shadow-2xl">
                            <div class="flex flex-col md:flex-row md:items-center justify-between gap-4 pb-5 border-b border-slate-200">
                                <div>
                                    <span class="text-xs font-heading font-bold text-[#0054A6] uppercase tracking-wider editable-text">
                                        <i class="fa-solid fa-certificate text-amber-500 mr-1"></i> DỮ LIỆU CHỨNG CHỈ NĂNG LỰC HOẠT ĐỘNG XÂY DỰNG
                                    </span>
                                    <h3 class="font-heading font-black text-xl sm:text-2xl text-[#002B5B] mt-1 editable-text">
                                        CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON — MÃ SỐ: <span class="text-[#E31837]">00076275</span>
                                    </h3>
                                </div>
                                <span class="text-xs font-bold bg-slate-100 text-[#002B5B] px-4 py-2 rounded-xl editable-text">
                                    Đại diện PL: Ông Huỳnh Bá Quý • MST: 0401676571 • Hiệu lực: 27/09/2033
                                </span>
                            </div>

                            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-5 gap-4 mt-5 text-xs">
                                <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200">
                                    <span class="px-2 py-0.5 rounded bg-[#E31837] text-white font-bold text-[10px] editable-text">HẠNG II</span>
                                    <h4 class="font-heading font-bold text-[#002B5B] text-sm mt-2 editable-text">Thi công Xây dựng Dân dụng</h4>
                                    <p class="text-slate-500 mt-1 editable-text">Số CC: HCM-00076275 (Hiệu lực đến 27/09/2033)</p>
                                </div>
                                <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200">
                                    <span class="px-2 py-0.5 rounded bg-[#0054A6] text-white font-bold text-[10px] editable-text">HẠNG III</span>
                                    <h4 class="font-heading font-bold text-[#002B5B] text-sm mt-2 editable-text">Thi công Nhà Công nghiệp</h4>
                                    <p class="text-slate-500 mt-1 editable-text">Nhà xưởng, kho vận, kết cấu công nghiệp</p>
                                </div>
                                <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200">
                                    <span class="px-2 py-0.5 rounded bg-[#0054A6] text-white font-bold text-[10px] editable-text">HẠNG III</span>
                                    <h4 class="font-heading font-bold text-[#002B5B] text-sm mt-2 editable-text">Thiết kế & Thẩm tra Thiết kế</h4>
                                    <p class="text-slate-500 mt-1 editable-text">Công trình Dân dụng & Nhà công nghiệp</p>
                                </div>
                                <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200">
                                    <span class="px-2 py-0.5 rounded bg-[#0054A6] text-white font-bold text-[10px] editable-text">HẠNG III</span>
                                    <h4 class="font-heading font-bold text-[#002B5B] text-sm mt-2 editable-text">Tư vấn Quản lý Dự án</h4>
                                    <p class="text-slate-500 mt-1 editable-text">Quản lý dự án Dân dụng & Công nghiệp</p>
                                </div>
                                <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200">
                                    <span class="px-2 py-0.5 rounded bg-[#0054A6] text-white font-bold text-[10px] editable-text">HẠNG III</span>
                                    <h4 class="font-heading font-bold text-[#002B5B] text-sm mt-2 editable-text">Tư vấn Giám sát & Lắp đặt</h4>
                                    <p class="text-slate-500 mt-1 editable-text">Giám sát thi công & Lắp đặt thiết bị công trình</p>
                                </div>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </section>


        <!-- =====================================================================
             [FLATSOME SECTION 05: DỰ ÁN TIÊU BIỂU - HTML TĨNH 100% ĐỂ COPY LÀ SỬA ĐƯỢC NGAY]
             Mỗi dự án nằm trong 1 cột .col.large-4.medium-6.small-12 chuẩn Flatsome
        ====================================================================== -->
        <section class="section bg-[#F4F7FA] acon-bg-blueprint" id="sec-05">
            <div class="ux-section-toolbar hidden absolute top-4 right-8 z-30 gap-2">
                <button onclick="copySingleSection('sec-05')" class="bg-sky-500 text-white text-xs font-bold px-3 py-1.5 rounded-lg shadow">Copy HTML Section 05</button>
            </div>

            <div class="section-content">
                <div class="row">
                    <!-- Tiêu đề & Bộ lọc dự án -->
                    <div class="col large-12 small-12">
                        <div class="col-inner flex flex-col lg:flex-row lg:items-end justify-between gap-6">
                            <div>
                                <div class="flex items-center gap-3 mb-2">
                                    <span class="w-10 h-1 bg-[#0054A6] rounded-full"></span>
                                    <span class="font-heading font-bold text-xs uppercase tracking-widest text-[#0054A6] editable-text">05 • CÔNG TRÌNH KIẾN TẠO</span>
                                </div>
                                <h2 class="font-heading font-black text-3xl sm:text-4xl lg:text-5xl text-[#002B5B] editable-text">
                                    DỰ ÁN <span class="text-[#0095DA]">TIÊU BIỂU</span>
                                </h2>
                            </div>

                            <!-- Nút lọc danh mục -->
                            <div class="flex flex-wrap gap-2">
                                <button onclick="filterStaticProjects('all')" class="acon-filter-btn px-4 py-2.5 rounded-xl font-heading font-bold text-xs uppercase bg-[#002B5B] text-white" data-filter="all">Tất cả dự án</button>
                                <button onclick="filterStaticProjects('commercial')" class="acon-filter-btn px-4 py-2.5 rounded-xl font-heading font-bold text-xs uppercase bg-white text-slate-700 border border-slate-200" data-filter="commercial">Khách sạn & Văn phòng</button>
                                <button onclick="filterStaticProjects('residential')" class="acon-filter-btn px-4 py-2.5 rounded-xl font-heading font-bold text-xs uppercase bg-white text-slate-700 border border-slate-200" data-filter="residential">Biệt thự & Dân dụng</button>
                                <button onclick="filterStaticProjects('industrial')" class="acon-filter-btn px-4 py-2.5 rounded-xl font-heading font-bold text-xs uppercase bg-white text-slate-700 border border-slate-200" data-filter="industrial">Nhà xưởng & Công nghiệp</button>
                            </div>
                        </div>
                    </div>

                    <!-- DỰ ÁN 01 (HTML tĩnh trực tiếp - Sửa chữ & thay src ảnh dễ dàng) -->
                    <div class="col large-4 medium-6 small-12 acon-project-col" data-cat="commercial">
                        <div class="col-inner">
                            <div class="acon-project-box">
                                <img src="https://images.unsplash.com/photo-1545324418-cc1a3fa10c00?auto=format&fit=crop&w=900&q=80" 
                                     alt="Tổ hợp Khách sạn và Căn hộ dịch vụ ven biển Mỹ Khê" 
                                     class="editable-img" />
                                <div class="acon-project-overlay">
                                    <div>
                                        <span class="px-3 py-1 rounded-full bg-[#0095DA] text-white text-[11px] font-bold uppercase editable-text">Khách sạn & Thương mại</span>
                                    </div>
                                    <div>
                                        <p class="text-xs text-[#0095DA] font-semibold mb-1 editable-text">
                                            <i class="fa-solid fa-location-dot"></i> Quận Sơn Trà, TP. Đà Nẵng • 2025 - 2026
                                        </p>
                                        <h3 class="font-heading font-extrabold text-lg sm:text-xl leading-snug editable-text">
                                            TỔ HỢP KHÁCH SẠN & CĂN HỘ DỊCH VỤ VEN BIỂN MỸ KHÊ
                                        </h3>
                                        <p class="text-xs text-white/80 mt-2 pt-2 border-t border-white/15 editable-text">
                                            Gói thầu: Tổng thầu Thiết kế & Thi công (D&B)
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- DỰ ÁN 02 -->
                    <div class="col large-4 medium-6 small-12 acon-project-col" data-cat="commercial">
                        <div class="col-inner">
                            <div class="acon-project-box">
                                <img src="https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?auto=format&fit=crop&w=900&q=80" 
                                     alt="Tòa nhà Văn phòng và Trụ sở điều hành Hòa Xuân" 
                                     class="editable-img" />
                                <div class="acon-project-overlay">
                                    <div>
                                        <span class="px-3 py-1 rounded-full bg-[#0095DA] text-white text-[11px] font-bold uppercase editable-text">Văn phòng & Thương mại</span>
                                    </div>
                                    <div>
                                        <p class="text-xs text-[#0095DA] font-semibold mb-1 editable-text">
                                            <i class="fa-solid fa-location-dot"></i> Phường Hòa Xuân, TP. Đà Nẵng • 2025
                                        </p>
                                        <h3 class="font-heading font-extrabold text-lg sm:text-xl leading-snug editable-text">
                                            TÒA NHÀ VĂN PHÒNG & TRỤ SỞ ĐIỀU HÀNH HÒA XUÂN
                                        </h3>
                                        <p class="text-xs text-white/80 mt-2 pt-2 border-t border-white/15 editable-text">
                                            Gói thầu: Thiết kế, Thi công & Hoàn thiện Nội thất
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- DỰ ÁN 03 -->
                    <div class="col large-4 medium-6 small-12 acon-project-col" data-cat="residential">
                        <div class="col-inner">
                            <div class="acon-project-box">
                                <img src="https://images.unsplash.com/photo-1600596542815-ffad4c1539a9?auto=format&fit=crop&w=900&q=80" 
                                     alt="Biệt thự nghỉ dưỡng sinh thái Nam Hòa Xuân và Euro Village" 
                                     class="editable-img" />
                                <div class="acon-project-overlay">
                                    <div>
                                        <span class="px-3 py-1 rounded-full bg-[#0095DA] text-white text-[11px] font-bold uppercase editable-text">Biệt thự & Dân dụng</span>
                                    </div>
                                    <div>
                                        <p class="text-xs text-[#0095DA] font-semibold mb-1 editable-text">
                                            <i class="fa-solid fa-location-dot"></i> KĐT Hòa Xuân & Sơn Trà, Đà Nẵng • 2025
                                        </p>
                                        <h3 class="font-heading font-extrabold text-lg sm:text-xl leading-snug editable-text">
                                            BIỆT THỰ NGHỈ DƯỠNG SINH THÁI NAM HÒA XUÂN & EURO VILLAGE
                                        </h3>
                                        <p class="text-xs text-white/80 mt-2 pt-2 border-t border-white/15 editable-text">
                                            Gói thầu: Tổng thầu Thi công trọn gói & Nội thất
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- DỰ ÁN 04 -->
                    <div class="col large-4 medium-6 small-12 acon-project-col" data-cat="industrial">
                        <div class="col-inner">
                            <div class="acon-project-box">
                                <img src="https://images.unsplash.com/photo-1581092160607-ee22621dd758?auto=format&fit=crop&w=900&q=80" 
                                     alt="Nhà máy sản xuất và Trung tâm kho vận KCN Hòa Khánh" 
                                     class="editable-img" />
                                <div class="acon-project-overlay">
                                    <div>
                                        <span class="px-3 py-1 rounded-full bg-[#0095DA] text-white text-[11px] font-bold uppercase editable-text">Nhà xưởng & Công nghiệp</span>
                                    </div>
                                    <div>
                                        <p class="text-xs text-[#0095DA] font-semibold mb-1 editable-text">
                                            <i class="fa-solid fa-location-dot"></i> KCN Hòa Khánh, Liên Chiểu, Đà Nẵng • 2024 - 2025
                                        </p>
                                        <h3 class="font-heading font-extrabold text-lg sm:text-xl leading-snug editable-text">
                                            NHÀ MÁY SẢN XUẤT & TRUNG TÂM KHO VẬN KCN HÒA KHÁNH
                                        </h3>
                                        <p class="text-xs text-white/80 mt-2 pt-2 border-t border-white/15 editable-text">
                                            Gói thầu: Thi công Nhà công nghiệp & Hạ tầng
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- DỰ ÁN 05 -->
                    <div class="col large-4 medium-6 small-12 acon-project-col" data-cat="commercial">
                        <div class="col-inner">
                            <div class="acon-project-box">
                                <img src="https://images.unsplash.com/photo-1554469384-e58fac16e23a?auto=format&fit=crop&w=900&q=80" 
                                     alt="Tòa nhà Thương mại Dịch vụ và Showroom Hải Châu" 
                                     class="editable-img" />
                                <div class="acon-project-overlay">
                                    <div>
                                        <span class="px-3 py-1 rounded-full bg-[#0095DA] text-white text-[11px] font-bold uppercase editable-text">Khách sạn & Thương mại</span>
                                    </div>
                                    <div>
                                        <p class="text-xs text-[#0095DA] font-semibold mb-1 editable-text">
                                            <i class="fa-solid fa-location-dot"></i> Quận Hải Châu, TP. Đà Nẵng • 2025
                                        </p>
                                        <h3 class="font-heading font-extrabold text-lg sm:text-xl leading-snug editable-text">
                                            TÒA NHÀ THƯƠNG MẠI DỊCH VỤ & SHOWROOM HẢI CHÂU
                                        </h3>
                                        <p class="text-xs text-white/80 mt-2 pt-2 border-t border-white/15 editable-text">
                                            Gói thầu: Tổng thầu Thi công & Lắp đặt thiết bị
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- DỰ ÁN 06 -->
                    <div class="col large-4 medium-6 small-12 acon-project-col" data-cat="residential">
                        <div class="col-inner">
                            <div class="acon-project-box">
                                <img src="https://images.unsplash.com/photo-1600585154340-be6161a56a0c?auto=format&fit=crop&w=900&q=80" 
                                     alt="Khu nhà phố thương mại Shophouse và Villa Phố Biển" 
                                     class="editable-img" />
                                <div class="acon-project-overlay">
                                    <div>
                                        <span class="px-3 py-1 rounded-full bg-[#0095DA] text-white text-[11px] font-bold uppercase editable-text">Biệt thự & Dân dụng</span>
                                    </div>
                                    <div>
                                        <p class="text-xs text-[#0095DA] font-semibold mb-1 editable-text">
                                            <i class="fa-solid fa-location-dot"></i> Quận Ngũ Hành Sơn, TP. Đà Nẵng • 2025 - 2026
                                        </p>
                                        <h3 class="font-heading font-extrabold text-lg sm:text-xl leading-snug editable-text">
                                            KHU NHÀ PHỐ THƯƠNG MẠI (SHOPHOUSE) & VILLA PHỐ BIỂN
                                        </h3>
                                        <p class="text-xs text-white/80 mt-2 pt-2 border-t border-white/15 editable-text">
                                            Gói thầu: Tư vấn QLDA, Giám sát & Thi công
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </section>


        <!-- =====================================================================
             [FLATSOME SECTION 06: TIN TỨC FANPAGE & TUYỂN DỤNG NHÂN SỰ]
             Bố cục .col.large-7 và .col.large-5 chuẩn Flatsome
        ====================================================================== -->
        <section class="section bg-white" id="sec-06">
            <div class="ux-section-toolbar hidden absolute top-4 right-8 z-30 gap-2">
                <button onclick="copySingleSection('sec-06')" class="bg-sky-500 text-white text-xs font-bold px-3 py-1.5 rounded-lg shadow">Copy HTML Section 06</button>
            </div>

            <div class="section-content">
                <div class="row">
                    <div class="col large-12 small-12">
                        <div class="col-inner flex flex-col md:flex-row md:items-end justify-between gap-4">
                            <div>
                                <div class="flex items-center gap-3 mb-2">
                                    <span class="w-10 h-1 bg-[#E31837] rounded-full"></span>
                                    <span class="font-heading font-bold text-xs uppercase tracking-widest text-[#E31837] editable-text">06 • NHỊP ĐẬP CÔNG TRƯỜNG & NHÂN SỰ</span>
                                </div>
                                <h2 class="font-heading font-black text-3xl sm:text-4xl lg:text-5xl text-[#002B5B] editable-text">
                                    TIN TỨC <span class="text-[#0054A6]">ACON</span> & TUYỂN DỤNG
                                </h2>
                            </div>
                            <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="font-heading font-bold text-xs uppercase tracking-wider text-[#0054A6] hover:text-[#0095DA] no-underline editable-text">
                                Xem tất cả bài đăng Fanpage <i class="fa-solid fa-arrow-right ml-1"></i>
                            </a>
                        </div>
                    </div>

                    <!-- Cột trái (large-7): Tin tiêu điểm -->
                    <div class="col large-7 small-12">
                        <div class="col-inner rounded-3xl overflow-hidden shadow-lg border border-slate-200 bg-white">
                            <div class="relative h-72 sm:h-80 overflow-hidden">
                                <img src="https://images.unsplash.com/photo-1541888946425-d09bb18086f6?auto=format&fit=crop&w=1200&q=85" 
                                     alt="ACON đẩy mạnh tiến độ thi công các dự án tại Đà Nẵng" 
                                     class="w-full h-full object-cover editable-img" />
                                <span class="absolute bottom-4 left-4 px-3 py-1 rounded-full bg-[#E31837] text-white text-xs font-bold uppercase editable-text">
                                    Tin công trường Fanpage
                                </span>
                            </div>
                            <div class="p-6 sm:p-8">
                                <h3 class="font-heading font-extrabold text-xl sm:text-2xl text-[#002B5B] mb-3 editable-text">
                                    ACON CONSTRUCTION ĐẨY MẠNH TIẾN ĐỘ THI CÔNG & NGHIỆM THU CÁC DỰ ÁN DÂN DỤNG – THƯƠNG MẠI TẠI ĐÀ NẴNG
                                </h3>
                                <p class="text-slate-600 text-sm sm:text-base editable-text">
                                    Với tinh thần kiểm soát chặt chẽ an toàn lao động (HSE) và chất lượng kỹ - mỹ thuật trên từng hạng mục kết cấu & hoàn thiện, Ban chỉ huy các công trường ACON Construction liên tục hoàn thành vượt mốc tiến độ cam kết với Chủ đầu tư.
                                </p>
                            </div>
                        </div>
                    </div>

                    <!-- Cột phải (large-5): Danh sách tin & Tuyển dụng -->
                    <div class="col large-5 small-12">
                        <div class="col-inner flex flex-col gap-4">
                            <!-- Bài 1 -->
                            <div class="p-5 rounded-3xl bg-slate-50 border border-slate-200">
                                <span class="inline-block px-2.5 py-0.5 rounded bg-[#E31837] text-white text-[10px] font-bold uppercase mb-2 editable-text">HOT • Tuyển dụng Đà Nẵng</span>
                                <h4 class="font-heading font-bold text-base text-[#002B5B] editable-text">
                                    ACON TUYỂN DỤNG: KỸ SƯ QS, CHỈ HUY TRƯỞNG CÔNG TRÌNH, KỸ SƯ HIỆN TRƯỜNG & KẾ TOÁN XÂY DỰNG
                                </h4>
                                <p class="text-xs text-slate-600 mt-2 editable-text">
                                    Làm việc tại: 145-147 Trung Lương 14, P. Hòa Xuân, Đà Nẵng • Nhận hồ sơ qua: acon.dng@gmail.com hoặc SĐT: 0916.104.099
                                </p>
                            </div>

                            <!-- Bài 2 -->
                            <div class="p-5 rounded-3xl bg-slate-50 border border-slate-200">
                                <span class="inline-block px-2.5 py-0.5 rounded bg-[#0054A6] text-white text-[10px] font-bold uppercase mb-2 editable-text">Hoạt động công trường</span>
                                <h4 class="font-heading font-bold text-base text-[#002B5B] editable-text">
                                    CHUẨN HÓA QUY TRÌNH QUẢN LÝ CHẤT LƯỢNG (QA/QC) & AN TOÀN VỆ SINH LAO ĐỘNG TRÊN TOÀN HỆ THỐNG ACON
                                </h4>
                                <p class="text-xs text-slate-600 mt-2 editable-text">
                                    Đào tạo nội bộ định kỳ cho đội ngũ Kỹ sư giám sát & Chỉ huy trưởng tại văn phòng trụ sở Hòa Xuân, Đà Nẵng.
                                </p>
                            </div>

                            <!-- Bài 3 -->
                            <div class="p-5 rounded-3xl bg-slate-50 border border-slate-200">
                                <span class="inline-block px-2.5 py-0.5 rounded bg-[#0095DA] text-white text-[10px] font-bold uppercase mb-2 editable-text">Kỷ niệm thành lập</span>
                                <h4 class="font-heading font-bold text-base text-[#002B5B] editable-text">
                                    HÀNH TRÌNH HƠN 1 THẬP KỶ KIẾN TẠO CÔNG TRÌNH BỀN VỮNG CỦA CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON (14/05/2015)
                                </h4>
                                <p class="text-xs text-slate-600 mt-2 editable-text">
                                    Khẳng định uy tín thương hiệu nhà thầu xây dựng chuyên nghiệp tại TP. Đà Nẵng và khu vực Miền Trung.
                                </p>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </section>


        <!-- =====================================================================
             [FLATSOME SECTION 07: LIÊN HỆ, BẢN ĐỒ & FORM BÁO GIÁ]
             Địa chỉ: 145-147 Trung Lương 14, Hòa Xuân, Đà Nẵng | SĐT: 0916.104.099
        ====================================================================== -->
        <section class="section bg-[#F4F7FA] border-t border-slate-200" id="sec-07">
            <div class="ux-section-toolbar hidden absolute top-4 right-8 z-30 gap-2">
                <button onclick="copySingleSection('sec-07')" class="bg-sky-500 text-white text-xs font-bold px-3 py-1.5 rounded-lg shadow">Copy HTML Section 07</button>
            </div>

            <div class="section-content">
                <div class="row">
                    <!-- Cột trái (large-6): Thông tin liên hệ & Google Map -->
                    <div class="col large-6 small-12">
                        <div class="col-inner space-y-6">
                            <div>
                                <div class="flex items-center gap-3 mb-2">
                                    <span class="w-10 h-1 bg-[#0054A6] rounded-full"></span>
                                    <span class="font-heading font-bold text-xs uppercase tracking-widest text-[#0054A6] editable-text">07 • THÔNG TIN LIÊN HỆ</span>
                                </div>
                                <h2 class="font-heading font-black text-3xl sm:text-4xl text-[#002B5B] editable-text">
                                    KẾT NỐI CÙNG <span class="text-[#0095DA]">ACON</span>
                                </h2>
                            </div>

                            <div class="bg-white rounded-3xl p-6 shadow-md border border-slate-200 space-y-4">
                                <div>
                                    <span class="text-xs font-bold uppercase text-[#0054A6] editable-text">Trụ sở văn phòng Đà Nẵng</span>
                                    <h4 class="font-heading font-bold text-[#002B5B] text-base mt-0.5 editable-text">
                                        145-147 Trung Lương 14, Phường Hòa Xuân, Quận Cẩm Lệ, TP. Đà Nẵng
                                    </h4>
                                    <p class="text-xs text-slate-500 mt-1 editable-text">Mã số thuế: 0401676571 • Mã chứng chỉ HĐXD: 00076275</p>
                                </div>

                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 pt-4 border-t border-slate-100 text-sm">
                                    <div>
                                        <span class="text-xs text-slate-400 uppercase block">Hotline trực tiếp</span>
                                        <strong class="font-heading font-extrabold text-[#E31837] text-base editable-text">0916.104.099</strong>
                                        <span class="block text-xs text-slate-500 editable-text">ĐT VP: 02363.789.769</span>
                                    </div>
                                    <div>
                                        <span class="text-xs text-slate-400 uppercase block">Email & Website</span>
                                        <strong class="text-[#002B5B] block editable-text">acon.dng@gmail.com</strong>
                                        <span class="block text-xs text-[#0095DA] font-bold editable-text">www.acondn.vn</span>
                                    </div>
                                </div>
                            </div>

                            <!-- Bản đồ Google Maps -->
                            <div class="rounded-3xl overflow-hidden shadow-md border-4 border-white h-64">
                                <iframe 
                                    title="Bản đồ trụ sở Công ty Cổ phần Đầu tư Xây dựng ACON"
                                    src="https://www.google.com/maps?q=145+Trung+L%C6%B0%C6%A1ng+14,+H%C3%B2a+Xu%C3%A2n,+C%E1%BA%A9m+L%E1%BB%87,+%C4%90%C3%A0+N%E1%BA%B5ng&output=embed"
                                    class="w-full h-full border-0"
                                    loading="lazy">
                                </iframe>
                            </div>
                        </div>
                    </div>

                    <!-- Cột phải (large-6): Form liên hệ (Hoặc chèn Contact Form 7 shortcode trong Flatsome) -->
                    <div class="col large-6 small-12">
                        <div class="col-inner bg-white rounded-3xl p-8 shadow-lg border border-slate-200">
                            <span class="inline-block px-3 py-1 rounded-full bg-[#0054A6]/10 text-[#0054A6] text-xs font-bold uppercase mb-2 editable-text">
                                Đăng ký tư vấn & Hợp tác
                            </span>
                            <h3 class="font-heading font-extrabold text-2xl text-[#002B5B] mb-2 editable-text">
                                GỬI YÊU CẦU BÁO GIÁ / ĐẤU THẦU
                            </h3>
                            <p class="text-xs sm:text-sm text-slate-500 mb-6 editable-text">
                                (Trong Flatsome, bạn có thể giữ nguyên form này hoặc thay bằng shortcode [contact-form-7] của WordPress).
                            </p>

                            <form onsubmit="handleSimpleSubmit(event)" class="space-y-4">
                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                                    <div>
                                        <label class="block text-xs font-bold uppercase text-slate-700 mb-1 editable-text">Họ và tên / Chủ đầu tư *</label>
                                        <input type="text" required placeholder="Nhập họ tên..." class="w-full px-4 py-3 rounded-xl bg-slate-50 border border-slate-200 text-sm" />
                                    </div>
                                    <div>
                                        <label class="block text-xs font-bold uppercase text-slate-700 mb-1 editable-text">Số điện thoại *</label>
                                        <input type="tel" required placeholder="0916.104.099" class="w-full px-4 py-3 rounded-xl bg-slate-50 border border-slate-200 text-sm" />
                                    </div>
                                </div>
                                <div>
                                    <label class="block text-xs font-bold uppercase text-slate-700 mb-1 editable-text">Hạng mục quan tâm</label>
                                    <select class="w-full px-4 py-3 rounded-xl bg-slate-50 border border-slate-200 text-sm">
                                        <option>Tổng thầu Thiết kế & Thi công (Design & Build)</option>
                                        <option>Thi công Khách sạn / Văn phòng / Biệt thự</option>
                                        <option>Thi công Nhà xưởng & Công nghiệp</option>
                                        <option>Tư vấn Quản lý dự án & Giám sát</option>
                                        <option>Ứng tuyển nhân sự (Kỹ sư QS / Chỉ huy trưởng / Kỹ sư)</option>
                                    </select>
                                </div>
                                <div>
                                    <label class="block text-xs font-bold uppercase text-slate-700 mb-1 editable-text">Nội dung chi tiết</label>
                                    <textarea rows="4" placeholder="Mô tả quy mô, địa điểm dự án..." class="w-full px-4 py-3 rounded-xl bg-slate-50 border border-slate-200 text-sm"></textarea>
                                </div>
                                <button type="submit" class="acon-btn acon-btn-primary w-full justify-center">
                                    <i class="fa-solid fa-paper-plane"></i>
                                    <span class="editable-text">Gửi thông tin đến ACON (acondn.vn)</span>
                                </button>
                            </form>
                        </div>
                    </div>

                </div>
            </div>
        </section>


        <!-- =====================================================================
             [FLATSOME FOOTER: CHÂN TRANG DOANH NGHIỆP ACON]
        ====================================================================== -->
        <footer class="bg-[#0A192F] text-white pt-16 pb-20 border-t border-white/10 acon-bg-blueprint-dark">
            <div class="row">
                <div class="col large-5 small-12">
                    <div class="col-inner space-y-3">
                        <h3 class="font-heading font-extrabold text-lg text-white editable-text">CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON</h3>
                        <p class="text-xs text-[#0095DA] font-bold editable-text">ACON INVESTMENT CONSTRUCTION JOINT STOCK COMPANY</p>
                        <p class="text-xs sm:text-sm text-white/70 editable-text">
                            Biểu tượng của Niềm tin, Chất lượng và Sự bền vững trong lĩnh vực Thiết kế, Quản lý dự án, Giám sát và Thi công xây dựng công trình Dân dụng – Công nghiệp tại Đà Nẵng và Miền Trung.
                        </p>
                    </div>
                </div>

                <div class="col large-3 small-12">
                    <div class="col-inner space-y-2 text-xs sm:text-sm text-white/80">
                        <h4 class="font-heading font-bold text-xs uppercase tracking-widest text-[#0095DA] mb-3 editable-text">Liên kết nhanh</h4>
                        <p><a href="#sec-02" class="text-white/80 hover:text-white no-underline editable-text">Giới thiệu & Lịch sử</a></p>
                        <p><a href="#sec-03" class="text-white/80 hover:text-white no-underline editable-text">Lĩnh vực hoạt động (D&B)</a></p>
                        <p><a href="#sec-04" class="text-white/80 hover:text-white no-underline editable-text">Chứng chỉ năng lực (00076275)</a></p>
                        <p><a href="#sec-05" class="text-white/80 hover:text-white no-underline editable-text">Dự án tiêu biểu</a></p>
                    </div>
                </div>

                <div class="col large-4 small-12">
                    <div class="col-inner space-y-2 text-xs sm:text-sm text-white/80">
                        <h4 class="font-heading font-bold text-xs uppercase tracking-widest text-[#0095DA] mb-3 editable-text">Thông tin pháp lý & Liên hệ</h4>
                        <p class="editable-text"><strong class="text-white">Địa chỉ:</strong> 145-147 Trung Lương 14, P. Hòa Xuân, Q. Cẩm Lệ, TP. Đà Nẵng</p>
                        <p class="editable-text"><strong class="text-white">Hotline:</strong> 0916.104.099 | ĐT VP: 02363.789.769</p>
                        <p class="editable-text"><strong class="text-white">Email:</strong> acon.dng@gmail.com | Web: acondn.vn</p>
                        <p class="editable-text"><strong class="text-white">MST:</strong> 0401676571 • Mã chứng chỉ HĐXD: 00076275</p>
                    </div>
                </div>
            </div>
        </footer>

    </div>
    <!-- KẾT THÚC VÙNG EXPORT HTML FLATSOME -->


    <!-- =========================================================================
         MODAL ĐỔI HÌNH ẢNH KHI CLICK VÀO ẢNH TRONG CHẾ ĐỘ "UX LIVE EDIT"
    ========================================================================== -->
    <div id="img-edit-modal" class="fixed inset-0 z-50 bg-black/80 backdrop-blur-sm hidden items-center justify-center p-4">
        <div class="bg-white rounded-3xl max-w-lg w-full p-6 shadow-2xl space-y-4">
            <div class="flex items-center justify-between border-b pb-3">
                <h3 class="font-bold text-slate-900 text-base">Thay đổi hình ảnh (Chuẩn UX Builder)</h3>
                <button onclick="closeImgEditModal()" class="text-slate-400 hover:text-red-600 text-lg"><i class="fa-solid fa-xmark"></i></button>
            </div>
            <div class="space-y-3 text-xs">
                <label class="block font-bold text-slate-700">Cách 1: Dán đường dẫn (URL) ảnh từ Fanpage hoặc WordPress Media:</label>
                <input type="text" id="edit-img-url-input" placeholder="https://..." class="w-full px-3.5 py-2.5 rounded-xl border border-slate-300 text-sm" />

                <label class="block font-bold text-slate-700 pt-2">Cách 2: Hoặc chọn file ảnh từ máy tính của bạn:</label>
                <input type="file" accept="image/*" onchange="handleLocalImgSelect(event)" class="w-full text-xs file:mr-3 file:py-2 file:px-4 file:rounded-xl file:border-0 file:bg-sky-600 file:text-white font-semibold" />
            </div>
            <div class="flex justify-end gap-2 pt-3 border-t">
                <button onclick="closeImgEditModal()" class="px-4 py-2 rounded-xl bg-slate-100 text-slate-700 font-semibold text-xs">Hủy</button>
                <button onclick="saveEditedImgUrl()" class="px-5 py-2 rounded-xl bg-[#0054A6] text-white font-bold text-xs">Lưu Hình Ảnh</button>
            </div>
        </div>
    </div>

    <!-- =========================================================================
         MODAL HƯỚNG DẪN DÁN VÀO FLATSOME WORDPRESS
    ========================================================================== -->
    <div id="guide-modal" class="fixed inset-0 z-50 bg-black/80 backdrop-blur-sm hidden items-center justify-center p-4">
        <div class="bg-white rounded-3xl max-w-2xl w-full p-6 sm:p-8 shadow-2xl space-y-4 text-xs sm:text-sm">
            <div class="flex items-center justify-between border-b pb-3">
                <h3 class="font-bold text-slate-900 text-lg">Hướng dẫn đưa vào WordPress Flatsome nhanh nhất</h3>
                <button onclick="closeGuideModal()" class="text-slate-400 hover:text-red-600 text-xl"><i class="fa-solid fa-xmark"></i></button>
            </div>
            <ol class="list-decimal pl-5 space-y-3 text-slate-700 leading-relaxed">
                <li>
                    <strong>Bước 1 (Sửa trực tiếp tại đây nếu muốn):</strong> Bấm nút màu vàng <strong>"Bật Sửa Trực Tiếp Chữ & Ảnh"</strong> ở thanh dưới cùng. Bạn có thể click vào bất kỳ dòng chữ nào để gõ lại nội dung, hoặc click vào bất kỳ ảnh/logo nào để thay link ảnh từ Fanpage.
                </li>
                <li>
                    <strong>Bước 2 (Copy CSS vào Flatsome):</strong> Bấm nút <strong>"1. Copy CSS"</strong>, sau đó vào quản trị WordPress: <em>Flatsome &rarr; Advanced &rarr; Custom CSS</em> (hoặc <em>Giao diện &rarr; Tùy biến &rarr; Style &rarr; Custom CSS</em>) và dán (Ctrl+V) vào.
                </li>
                <li>
                    <strong>Bước 3 (Copy HTML hoặc UX Shortcode vào Trang chủ):</strong>
                    <ul class="list-disc pl-5 mt-1 space-y-1">
                        <li><strong>Cách A (Dán HTML):</strong> Bấm <strong>"2. Copy Toàn Bộ HTML"</strong> (hoặc copy từng Section), mở <em>Edit with UX Builder</em> &rarr; Thêm <strong>Element HTML</strong> &rarr; Dán vào là xong!</li>
                        <li><strong>Cách B (Dán UX Builder Shortcode):</strong> Bấm <strong>"3. Copy UX Shortcode"</strong> để lấy mã bọc sẵn trong <code>[section] [row] [col]</code> của Flatsome, dán thẳng vào khung soạn thảo văn bản của trang!</li>
                    </ul>
                </li>
            </ol>
            <div class="flex justify-end pt-3 border-t">
                <button onclick="closeGuideModal()" class="px-6 py-2.5 rounded-xl bg-[#002B5B] text-white font-bold text-xs uppercase">Đã hiểu</button>
            </div>
        </div>
    </div>

    <!-- =========================================================================
         JAVASCRIPT XỬ LÝ SLIDER, LỌC DỰ ÁN & CÔNG CỤ COPY FLATSOME
    ========================================================================== -->
    <script>
        // 1. Chuyển Slide Hero (Chỉ đổi opacity của 3 thẻ div tĩnh, không ghi đè HTML)
        let currentSlideIndex = 0;
        function changeHeroSlide(idx) {
            currentSlideIndex = idx;
            document.querySelectorAll('.acon-hero-slide').forEach((slide, i) => {
                slide.style.opacity = (i === idx) ? '1' : '0';
            });
        }
        setInterval(() => {
            changeHeroSlide((currentSlideIndex + 1) % 3);
        }, 6000);

        // 2. Lọc Dự Án Tĩnh (Ẩn/hiện trực tiếp các cột .acon-project-col)
        function filterStaticProjects(cat) {
            document.querySelectorAll('.acon-filter-btn').forEach(btn => {
                if (btn.dataset.filter === cat) {
                    btn.className = "acon-filter-btn px-4 py-2.5 rounded-xl font-heading font-bold text-xs uppercase bg-[#002B5B] text-white";
                } else {
                    btn.className = "acon-filter-btn px-4 py-2.5 rounded-xl font-heading font-bold text-xs uppercase bg-white text-slate-700 border border-slate-200";
                }
            });

            document.querySelectorAll('.acon-project-col').forEach(col => {
                if (cat === 'all' || col.dataset.cat === cat) {
                    col.style.display = 'block';
                } else {
                    col.style.display = 'none';
                }
            });
        }

        // 3. Form liên hệ
        function handleSimpleSubmit(e) {
            e.preventDefault();
            showToast("Đã nhận thông tin! Bạn có thể gọi trực tiếp Hotline 0916.104.099.");
            e.target.reset();
        }

        // 4. Cập nhật thanh điều hướng 01 - 07 bên phải khi cuộn trang
        window.addEventListener('scroll', () => {
            const secs = ['sec-01', 'sec-02', 'sec-03', 'sec-04', 'sec-05', 'sec-06', 'sec-07'];
            let activeId = 'sec-01';
            secs.forEach(id => {
                const el = document.getElementById(id);
                if (el && el.getBoundingClientRect().top <= window.innerHeight * 0.45) {
                    activeId = id;
                }
            });
            document.querySelectorAll('.acon-side-nav .nav-dot').forEach(dot => {
                if (dot.dataset.sec === activeId) {
                    dot.classList.add('active');
                } else {
                    dot.classList.remove('active');
                }
            });
        });

        // =====================================================================
        // CÔNG CỤ FLATSOME UX LIVE EDIT & ONE-CLICK COPY
        // =====================================================================
        let isUxEditMode = false;
        let currentEditingImg = null;

        function toggleUxLiveEdit() {
            isUxEditMode = !isUxEditMode;
            const btn = document.getElementById('btn-live-edit');
            document.body.classList.toggle('ux-edit-mode', isUxEditMode);

            document.querySelectorAll('.editable-text').forEach(el => {
                el.setAttribute('contenteditable', isUxEditMode ? 'true' : 'false');
            });

            if (isUxEditMode) {
                btn.innerHTML = `<i class="fa-solid fa-check"></i> <span>Đang Bật Sửa Trực Tiếp (Click vào chữ/ảnh để sửa)</span>`;
                btn.className = "px-3.5 py-2 rounded-xl bg-rose-600 hover:bg-rose-500 text-white font-bold transition-all flex items-center gap-1.5 shadow";
                showToast("Đã BẬT chế độ sửa trực tiếp! Hãy click vào bất kỳ chữ hoặc ảnh nào trên trang để sửa.");
            } else {
                btn.innerHTML = `<i class="fa-solid fa-pen-to-square"></i> <span>Bật Sửa Trực Tiếp Chữ & Ảnh</span>`;
                btn.className = "px-3.5 py-2 rounded-xl bg-amber-500 hover:bg-amber-600 text-slate-950 font-bold transition-all flex items-center gap-1.5 shadow";
                showToast("Đã lưu nội dung chỉnh sửa trên trang!");
            }
        }

        // Bắt sự kiện click vào ảnh khi đang ở chế độ UX Live Edit
        document.addEventListener('click', (e) => {
            if (!isUxEditMode) return;
            const img = e.target.closest('img');
            if (img) {
                e.preventDefault();
                e.stopPropagation();
                currentEditingImg = img;
                document.getElementById('edit-img-url-input').value = img.getAttribute('src') || '';
                const modal = document.getElementById('img-edit-modal');
                modal.classList.remove('hidden');
                modal.classList.add('flex');
            }
        });

        function closeImgEditModal() {
            const modal = document.getElementById('img-edit-modal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
            currentEditingImg = null;
        }

        function saveEditedImgUrl() {
            if (currentEditingImg) {
                const newUrl = document.getElementById('edit-img-url-input').value.trim();
                if (newUrl) {
                    currentEditingImg.setAttribute('src', newUrl);
                    showToast("Đã cập nhật hình ảnh thành công!");
                }
            }
            closeImgEditModal();
        }

        function handleLocalImgSelect(event) {
            const file = event.target.files[0];
            if (!file) return;
            const reader = new FileReader();
            reader.onload = function(e) {
                document.getElementById('edit-img-url-input').value = e.target.result;
            };
            reader.readAsDataURL(file);
        }

        // Hàm copy chuẩn tương thích mọi trình duyệt & iFrame
        function copyToClipboardSafe(text, message) {
            const ta = document.createElement('textarea');
            ta.value = text;
            ta.style.position = 'fixed';
            ta.style.left = '-9999px';
            document.body.appendChild(ta);
            ta.select();
            try {
                document.execCommand('copy');
                showToast(message);
            } catch (err) {
                showToast("Không thể tự động copy, vui lòng thử lại.");
            }
            document.body.removeChild(ta);
        }

        function showToast(msg) {
            const toast = document.getElementById('ux-toast');
            document.getElementById('ux-toast-msg').textContent = msg;
            toast.classList.remove('hidden');
            toast.classList.add('flex');
            setTimeout(() => {
                toast.classList.add('hidden');
                toast.classList.remove('flex');
            }, 3800);
        }

        // Làm sạch các thuộc tính tạm của UX Edit trước khi xuất code HTML
        function getCleanExportHTML(element) {
            const clone = element.cloneNode(true);
            clone.querySelectorAll('[contenteditable]').forEach(el => el.removeAttribute('contenteditable'));
            clone.querySelectorAll('.ux-section-toolbar').forEach(el => el.remove());
            return clone.outerHTML;
        }

        // 1. Copy CSS cho Flatsome
        function copyFlatsomeCSS() {
            const cssContent = document.getElementById('flatsome-custom-css').innerHTML.trim();
            copyToClipboardSafe(cssContent, "Đã Copy CSS! Hãy dán vào Flatsome -> Advanced -> Custom CSS.");
        }

        // 2. Copy Toàn Bộ HTML
        function copyAllFlatsomeHTML() {
            const area = document.getElementById('flatsome-export-area');
            const cleanHTML = getCleanExportHTML(area);
            copyToClipboardSafe(cleanHTML, "Đã Copy toàn bộ HTML! Hãy dán vào UX Builder -> HTML Element.");
        }

        // 3. Copy 1 Section lẻ
        function copySingleSection(secId) {
            const sec = document.getElementById(secId);
            if (!sec) return;
            const cleanSec = getCleanExportHTML(sec);
            copyToClipboardSafe(`<div class="acon-wrapper">\n${cleanSec}\n</div>`, `Đã Copy HTML của ${secId.toUpperCase()}!`);
        }

        // 4. Copy mã Shortcode chuẩn UX Builder của Flatsome ([section] [row] [col])
        function copyFlatsomeShortcode() {
            const area = document.getElementById('flatsome-export-area');
            const cleanHTML = getCleanExportHTML(area);
            const uxShortcode = `[section label="ACON Website - acondn.vn" padding="0px" bg_color="#ffffff"]\n[row style="collapse" width="full-width"]\n[col span="12" span__sm="12"]\n[ux_html]\n${cleanHTML}\n[/ux_html]\n[/col]\n[/row]\n[/section]`;
            copyToClipboardSafe(uxShortcode, "Đã Copy UX Builder Shortcode ([section]...[ux_html])! Dán thẳng vào trang Flatsome.");
        }

        function openGuideModal() {
            const m = document.getElementById('guide-modal');
            m.classList.remove('hidden');
            m.classList.add('flex');
        }
        function closeGuideModal() {
            const m = document.getElementById('guide-modal');
            m.classList.add('hidden');
            m.classList.remove('flex');
        }
    </script>
</body>
</html>
