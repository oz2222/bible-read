<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no, viewport-fit=cover">
    <title>우리 함께 성경 읽기표</title>
    
    <!-- iOS Web App Meta Tags (진짜 어플처럼 전체화면으로 실행되게 만드는 마법의 태그) -->
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <meta name="apple-mobile-web-app-title" content="성경읽기표">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts for elegant Korean text -->
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300;400;500;700;900&family=Playfair+Display:ital,wght@0,600;1,400&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Noto Sans KR', sans-serif;
            background-color: #f7f5f0; /* Soft warm ivory paper background */
            -webkit-tap-highlight-color: transparent;
        }
        .serif-title {
            font-family: 'Playfair Display', 'Noto Sans KR', serif;
        }
        /* Custom Scrollbar for elegant look */
        ::-webkit-scrollbar {
            width: 6px;
            height: 6px;
        }
        ::-webkit-scrollbar-track {
            background: #f1ede4;
        }
        ::-webkit-scrollbar-thumb {
            background: #c5bfae;
            border-radius: 3px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #a39c89;
        }
        .chapter-btn {
            transition: all 0.2s cubic-bezier(0.4, 0, 0.2, 1);
        }
        /* iOS Safe Area spacing for standalone mode */
        @supports (padding-top: env(safe-area-inset-top)) {
            header {
                padding-top: calc(env(safe-area-inset-top) + 0.5rem);
            }
        }
    </style>
</head>
<body class="text-stone-800 min-h-screen flex flex-col antialiased">

    <!-- Top Navigation Header -->
    <header class="bg-emerald-900 text-stone-100 shadow-md sticky top-0 z-40 transition-all">
        <div class="max-w-7xl mx-auto px-4 py-3.5 flex flex-wrap items-center justify-between gap-3">
            <div class="flex items-center space-x-3">
                <div class="bg-amber-100 text-emerald-900 w-10 h-10 rounded-full flex items-center justify-center shadow-inner">
                    <i class="fa-solid fa-book-bible text-xl"></i>
                </div>
                <div>
                    <h1 class="text-lg md:text-xl font-bold tracking-tight flex items-center gap-2">
                        <span>우리 함께 성경 읽기</span>
                        <span class="text-xs bg-emerald-800 text-amber-200 border border-emerald-700 px-2 py-0.5 rounded-full font-normal">신구약 완독표</span>
                    </h1>
                    <p class="text-xs text-emerald-200/80 font-light hidden sm:block">"주의 말씀은 내 발에 등이요 내 길에 빛이니이다" (시 119:105)</p>
                </div>
            </div>

            <!-- Profile and Options Buttons -->
            <div class="flex items-center gap-2">
                <!-- User Selector Dropdown -->
                <div class="relative inline-block text-left">
                    <button id="userDropdownBtn" onclick="toggleUserDropdown()" class="bg-emerald-800 hover:bg-emerald-700 text-stone-100 px-3.5 py-1.5 rounded-lg text-sm font-medium flex items-center gap-2 border border-emerald-700 shadow-sm transition-all">
                        <i class="fa-solid fa-user-circle text-lg text-amber-300"></i>
                        <span id="currentUserDisplay">사용자 선택</span>
                        <i class="fa-solid fa-chevron-down text-xs opacity-70"></i>
                    </button>
                    <!-- Dropdown Menu -->
                    <div id="userDropdownMenu" class="hidden absolute right-0 mt-2 w-56 rounded-xl bg-white shadow-xl ring-1 ring-black ring-opacity-5 divide-y divide-stone-100 z-50 animate-fade-in-down origin-top-right">
                        <div class="py-1" id="userListContainer">
                            <!-- Dynamic User Profiles go here -->
                        </div>
                        <div class="py-1.5 px-3">
                            <button onclick="openAddUserModal()" class="w-full text-left px-2 py-1.5 text-xs text-emerald-700 font-medium hover:bg-emerald-50 rounded-lg flex items-center gap-1.5">
                                <i class="fa-solid fa-plus-circle"></i> 함께 읽을 사람 추가
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Shared/Sync Option -->
                <button onclick="openShareModal()" class="bg-amber-600 hover:bg-amber-500 text-white p-2 rounded-lg text-sm font-medium shadow-sm transition-all" title="데이터 공유 및 백업">
                    <i class="fa-solid fa-share-nodes"></i>
                </button>
            </div>
        </div>
    </header>

    <!-- Main Content Grid -->
    <main class="flex-grow max-w-7xl w-full mx-auto p-3 md:p-6 grid grid-cols-1 lg:grid-cols-12 gap-6">

        <!-- Left Panel: Profile Progression Comparison & motivational quotes -->
        <section class="lg:col-span-4 space-y-6">

            <!-- Profile Card -->
            <div class="bg-white rounded-2xl p-5 shadow-sm border border-stone-200/80 relative overflow-hidden">
                <div class="absolute -right-4 -bottom-4 text-stone-100 pointer-events-none opacity-40">
                    <i class="fa-solid fa-dove text-9xl"></i>
                </div>
                
                <div class="flex items-center justify-between mb-4">
                    <div class="flex items-center gap-2.5">
                        <div id="userBadgeColor" class="w-4 h-4 rounded-full bg-emerald-600"></div>
                        <h2 class="text-xl font-bold text-stone-800" id="activeUserName">나</h2>
                    </div>
                    <span class="text-xs text-stone-500 font-medium" id="bibleCompleteDateEstimation">완독 예정일 계산 중...</span>
                </div>

                <!-- Main Progress Ring & Stat -->
                <div class="flex items-center gap-5 my-4">
                    <div class="relative w-24 h-24 flex items-center justify-center flex-shrink-0">
                        <svg class="w-full h-full transform -rotate-90">
                            <!-- Track -->
                            <circle cx="48" cy="48" r="40" stroke="#f1ede4" stroke-width="8" fill="transparent" />
                            <!-- Progress Bar -->
                            <circle id="progressRing" cx="48" cy="48" r="40" stroke="#10b981" stroke-width="8" fill="transparent" 
                                    stroke-dasharray="251.2" stroke-dashoffset="251.2" stroke-linecap="round" class="transition-all duration-500" />
                        </svg>
                        <div class="absolute inset-0 flex flex-col items-center justify-center">
                            <span class="text-lg font-black tracking-tight" id="progressPercentage">0%</span>
                            <span class="text-[10px] text-stone-400 font-bold uppercase">Progress</span>
                        </div>
                    </div>

                    <div class="flex-grow space-y-1.5 min-w-0">
                        <div>
                            <span class="text-xs text-stone-400 font-semibold block">총 읽은 분량</span>
                            <span class="text-lg font-bold text-stone-700 truncate block"><span id="totalCheckedChapters">0</span> <span class="text-xs text-stone-400">/ 1,189 장</span></span>
                        </div>
                        <div class="grid grid-cols-2 gap-2 pt-1 border-t border-stone-100">
                            <div>
                                <span class="text-[10px] text-stone-400 block font-semibold">구약 (929장)</span>
                                <span class="text-xs font-bold text-stone-600" id="otProgressText">0 / 929</span>
                            </div>
                            <div>
                                <span class="text-[10px] text-stone-400 block font-semibold">신약 (260장)</span>
                                <span class="text-xs font-bold text-stone-600" id="ntProgressText">0 / 260</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Settings: Target Daily Reading -->
                <div class="bg-stone-50 rounded-xl p-3 border border-stone-100 text-xs text-stone-600 space-y-2.5">
                    <div class="flex justify-between items-center">
                        <span class="font-medium">하루 목표 읽기 분량:</span>
                        <div class="flex items-center gap-1.5">
                            <input type="number" id="dailyGoalInput" value="3" min="1" max="100" onchange="updateDailyGoal()" class="w-12 text-center border border-stone-300 rounded px-1 py-0.5 focus:outline-emerald-600 font-bold text-stone-800">
                            <span>장씩</span>
                        </div>
                    </div>
                    <div class="flex justify-between items-center text-stone-500">
                        <span>완독 소요 일수:</span>
                        <span class="font-semibold text-stone-700" id="remainingDaysDisplay">약 397일</span>
                    </div>
                </div>
            </div>

            <!-- Real-time Cloud Sync Card (실시간 무선 공유 카드 - 이제 기본적으로 무조건 보입니다!) -->
            <div id="cloudSyncCard" class="bg-gradient-to-br from-emerald-50 to-amber-50/50 rounded-2xl p-5 shadow-sm border border-emerald-100/60 relative overflow-hidden">
                <div class="flex items-center justify-between mb-2">
                    <h3 class="font-bold text-emerald-950 text-xs tracking-wide flex items-center gap-1.5">
                        <i id="cloudStatusIcon" class="fa-solid fa-cloud-arrow-up text-stone-400"></i>
                        <span>실시간 무선 연동방</span>
                    </h3>
                    <span id="cloudStatusBadge" class="text-[10px] bg-stone-200 text-stone-600 px-2 py-0.5 rounded-full font-semibold">연동 전</span>
                </div>
                <p id="cloudStatusDesc" class="text-[11px] text-stone-600 mb-3.5 leading-relaxed">
                    원하는 방 이름을 입력하고 함께 접속해 보세요! 멀리 떨어져 있어도 실시간으로 체크 내용이 자동 공유됩니다. (가입 필요 없음)
                </p>
                <!-- Form to Join -->
                <div id="cloudActionForm" class="flex gap-2">
                    <input type="text" id="cloudRoomInput" placeholder="예: 은혜와지우" class="flex-grow px-3 py-2 rounded-xl border border-stone-200 text-xs focus:outline-emerald-600 bg-white shadow-inner font-semibold">
                    <button onclick="connectCloudRoom()" class="bg-emerald-800 hover:bg-emerald-700 text-white font-bold px-3.5 py-2 rounded-xl text-xs transition-all whitespace-nowrap">
                        연동하기
                    </button>
                </div>
                <!-- Connected Status UI -->
                <div id="cloudActiveForm" class="hidden flex items-center justify-between bg-white/90 p-3 rounded-xl border border-emerald-100/50 shadow-sm">
                    <div class="truncate mr-2">
                        <span class="text-[9px] text-stone-400 block font-bold">실시간 연동 중인 방</span>
                        <span id="activeRoomNameDisplay" class="text-xs font-bold text-emerald-800 truncate block">은혜와지우</span>
                    </div>
                    <button onclick="leaveCloudRoom()" class="bg-rose-50 hover:bg-rose-100 text-rose-700 border border-rose-200/40 font-bold px-2.5 py-1.5 rounded-lg text-[10px] transition-all whitespace-nowrap">
                        연동 해제
                    </button>
                </div>
            </div>

            <!-- Together Board (Dynamic Comparison with others) -->
            <div class="bg-white rounded-2xl p-5 shadow-sm border border-stone-200/80">
                <h3 class="font-bold text-stone-800 text-sm tracking-wide uppercase mb-3.5 flex items-center justify-between">
                    <span><i class="fa-solid fa-users-rectangle text-emerald-600 mr-1.5"></i>멤버별 읽기 현황판</span>
                    <span class="text-[10px] text-emerald-800 bg-emerald-50 px-2 py-0.5 rounded-full font-medium">진도 비교</span>
                </h3>
                <div class="space-y-4" id="compareUsersContainer">
                    <!-- Dynamic progression bars for all users -->
                </div>
            </div>

            <!-- Helpful Bible Quotes / Motivation widget -->
            <div class="bg-amber-50/70 border border-amber-200/50 rounded-2xl p-4 text-stone-700 text-xs relative">
                <i class="fa-solid fa-quote-left absolute top-3 left-3 text-amber-200 text-2xl"></i>
                <div class="pl-6 relative z-10">
                    <p id="motivationalVerse" class="italic leading-relaxed font-medium text-stone-600">"여호와의 율법은 완전하여 영혼을 소성시키며 여호와의 증거는 확실하여 우둔한 자를 지혜롭게 하며" (시편 19:7)</p>
                    <button onclick="getNewVerse()" class="mt-2 text-[10px] font-bold text-amber-800 hover:text-amber-900 flex items-center gap-1">
                        <i class="fa-solid fa-rotate-left"></i> 다른 구절 보기
                    </button>
                </div>
            </div>

        </section>

        <!-- Right Panel: Bible Books Checklist & Selection -->
        <section class="lg:col-span-8 space-y-6">

            <!-- Category & Search Tabs -->
            <div class="bg-white p-3.5 rounded-2xl shadow-sm border border-stone-200/80 flex flex-wrap items-center justify-between gap-3">
                <!-- Tabs -->
                <div class="flex bg-stone-100 p-1 rounded-xl gap-1">
                    <button onclick="filterBibleCategory('전체')" id="tabBtn_전체" class="category-tab px-4 py-1.5 rounded-lg text-xs font-semibold tracking-wide transition-all bg-white text-stone-800 shadow-sm">
                        전체 (66권)
                    </button>
                    <button onclick="filterBibleCategory('구약')" id="tabBtn_구약" class="category-tab px-4 py-1.5 rounded-lg text-xs font-semibold tracking-wide transition-all text-stone-500 hover:text-stone-800">
                        구약 (39권)
                    </button>
                    <button onclick="filterBibleCategory('신약')" id="tabBtn_신약" class="category-tab px-4 py-1.5 rounded-lg text-xs font-semibold tracking-wide transition-all text-stone-500 hover:text-stone-800">
                        신약 (27권)
                    </button>
                </div>

                <!-- Simple Search bar -->
                <div class="relative w-full sm:w-auto">
                    <i class="fa-solid fa-magnifying-glass absolute left-3 top-2.5 text-stone-400 text-xs"></i>
                    <input type="text" id="searchInput" oninput="searchBibleBook()" placeholder="성경 책 이름 검색... (예: 창세)" class="w-full sm:w-48 pl-8 pr-3 py-1.5 rounded-xl border border-stone-200 text-xs focus:outline-emerald-600">
                </div>
            </div>

            <!-- Double-Column Flex View (Left: Bible Books List, Right: Interactive Chapter Checker) -->
            <div class="grid grid-cols-1 md:grid-cols-12 gap-5 min-h-[500px]">

                <!-- Bible Books Selector (List) -->
                <div class="md:col-span-5 bg-white rounded-2xl shadow-sm border border-stone-200/80 p-3 flex flex-col max-h-[550px]">
                    <span class="text-xs text-stone-400 font-bold px-2 py-1 flex items-center gap-1 border-b border-stone-100 pb-2">
                        <i class="fa-solid fa-scroll"></i> 성경 목록 선택
                    </span>
                    <div class="overflow-y-auto flex-grow divide-y divide-stone-100/60 pr-1 mt-2" id="bibleBookList">
                        <!-- Bible Book Buttons will load dynamically -->
                    </div>
                </div>

                <!-- Interactive Chapter Board -->
                <div class="md:col-span-7 bg-white rounded-2xl shadow-sm border border-stone-200/80 p-4 md:p-5 flex flex-col justify-between max-h-[550px]">
                    
                    <div class="flex-grow flex flex-col overflow-hidden">
                        <!-- Active Book Title Header -->
                        <div class="border-b border-stone-100 pb-3 mb-4 flex flex-wrap items-center justify-between gap-2">
                            <div>
                                <h3 class="text-xl font-bold text-stone-800 flex items-center gap-2">
                                    <span id="activeBookName">창세기</span>
                                    <span id="activeBookEnglish" class="text-xs text-stone-400 font-medium italic">Genesis</span>
                                </h3>
                                <p class="text-xs text-stone-400 font-medium mt-0.5" id="activeBookProgressText">읽은 진도: 0 / 50장</p>
                            </div>

                            <!-- Fast-Action Bulk Controls -->
                            <div class="flex gap-1">
                                <button onclick="bulkCheckActiveBook(true)" class="bg-emerald-50 hover:bg-emerald-100 text-emerald-800 px-2.5 py-1 rounded text-[11px] font-bold transition-all">
                                    <i class="fa-solid fa-check-double mr-0.5"></i> 전체 선택
                                </button>
                                <button onclick="bulkCheckActiveBook(false)" class="bg-stone-50 hover:bg-stone-100 text-stone-500 px-2.5 py-1 rounded text-[11px] font-bold transition-all border border-stone-200/40">
                                    초기화
                                </button>
                            </div>
                        </div>

                        <!-- Main Chapter Buttons Matrix Grid -->
                        <div class="overflow-y-auto flex-grow pr-1" id="chapterMatrixContainer">
                            <!-- Chapter Grid Buttons will load here dynamically -->
                        </div>
                    </div>

                    <!-- Custom Range/Bulk check helper footer -->
                    <div class="bg-stone-50 border border-stone-100 rounded-xl p-3.5 mt-4 text-xs">
                        <div class="flex flex-wrap items-center justify-between gap-2">
                            <span class="text-stone-500 font-medium"><i class="fa-solid fa-wand-magic-sparkles mr-0.5 text-amber-500"></i> 몰아서 선택하기:</span>
                            <div class="flex items-center gap-1.5">
                                <input type="number" id="bulkRangeValue" min="1" max="150" value="10" class="w-12 text-center border border-stone-300 rounded px-1.5 py-0.5 text-stone-800 font-bold">
                                <span class="text-stone-500">장까지 한 번에</span>
                                <button onclick="checkUpToRange()" class="bg-emerald-800 hover:bg-emerald-700 text-white font-bold px-2.5 py-1 rounded transition-all">확인</button>
                            </div>
                        </div>
                    </div>

                </div>

            </div>

        </section>

    </main>

    <!-- Footer Area -->
    <footer class="bg-stone-100 border-t border-stone-200 py-6 mt-12 text-center text-xs text-stone-500">
        <p class="font-semibold mb-1">우리 함께 성경 읽기표 &copy; 2026</p>
        <p>함께 읽는 분들과 독서 진도를 공유하며 성경을 통독해 보세요.</p>
    </footer>

    <!-- ADD USER PROFILE MODAL -->
    <div id="addUserModal" class="hidden fixed inset-0 bg-stone-900/50 backdrop-blur-sm flex items-center justify-center z-50 p-4">
        <div class="bg-white rounded-2xl p-6 max-w-sm w-full shadow-2xl animate-fade-in border border-stone-100">
            <h3 class="font-bold text-lg text-stone-800 mb-4 flex items-center gap-1.5">
                <i class="fa-solid fa-user-plus text-emerald-600"></i> 함께 읽을 멤버 추가
            </h3>
            
            <div class="space-y-4">
                <div>
                    <label class="block text-xs font-bold text-stone-500 mb-1" for="newUserName">이름 (등록할 사람의 이름)</label>
                    <input type="text" id="newUserName" placeholder="예: 박친구, 김은혜, 우리엄마" class="w-full px-3 py-2 rounded-xl border border-stone-200 text-sm focus:outline-emerald-600">
                </div>
                <div>
                    <label class="block text-xs font-bold text-stone-500 mb-1">테마 컬러 선택</label>
                    <div class="grid grid-cols-4 gap-2" id="colorPickerContainer">
                        <button onclick="selectColorBadge('emerald')" class="color-badge border-2 border-emerald-600 w-full py-2 bg-emerald-500 rounded-lg text-white font-bold text-xs">초록</button>
                        <button onclick="selectColorBadge('amber')" class="color-badge border-2 border-transparent w-full py-2 bg-amber-500 rounded-lg text-white font-bold text-xs">황토</button>
                        <button onclick="selectColorBadge('rose')" class="color-badge border-2 border-transparent w-full py-2 bg-rose-500 rounded-lg text-white font-bold text-xs">장미</button>
                        <button onclick="selectColorBadge('blue')" class="color-badge border-2 border-transparent w-full py-2 bg-indigo-500 rounded-lg text-white font-bold text-xs">바다</button>
                    </div>
                </div>
            </div>

            <div class="flex gap-2 mt-6">
                <button onclick="closeAddUserModal()" class="flex-1 bg-stone-100 hover:bg-stone-200 text-stone-600 font-bold py-2 rounded-xl text-sm transition-all">취소</button>
                <button onclick="submitNewUser()" class="flex-1 bg-emerald-800 hover:bg-emerald-700 text-white font-bold py-2 rounded-xl text-sm transition-all">추가하기</button>
            </div>
        </div>
    </div>

    <!-- EXPORT & IMPORT DATA MODAL (Offline Backup) -->
    <div id="shareModal" class="hidden fixed inset-0 bg-stone-900/50 backdrop-blur-sm flex items-center justify-center z-50 p-4">
        <div class="bg-white rounded-2xl p-6 max-w-md w-full shadow-2xl animate-fade-in border border-stone-100">
            <h3 class="font-bold text-lg text-stone-800 mb-2 flex items-center gap-1.5">
                <i class="fa-solid fa-file-export text-amber-600"></i> 백업용 공유코드 추출
            </h3>
            <p class="text-xs text-stone-500 mb-4 leading-relaxed">혹시 기기를 변경해야 하는 경우 아래의 수동 코드를 사용하여 기존 오프라인 데이터를 수동 백업 및 복원할 수 있습니다.</p>

            <div class="space-y-4">
                <div>
                    <label class="block text-xs font-bold text-stone-500 mb-1">내 오프라인 데이터 백업 코드</label>
                    <div class="flex gap-2">
                        <textarea id="shareCodeTextarea" readonly class="w-full px-3 py-2 bg-stone-50 rounded-xl border border-stone-200 text-xs text-stone-600 h-20 resize-none font-mono focus:outline-none"></textarea>
                    </div>
                    <button onclick="copyShareCode()" class="mt-1.5 w-full bg-amber-500 hover:bg-amber-600 text-white text-xs font-bold py-2 rounded-lg transition-all flex items-center justify-center gap-1.5 shadow-sm">
                        <i class="fa-regular fa-copy"></i> 복사하기 (클립보드 저장)
                    </button>
                    <span id="copySuccessMsg" class="hidden text-[11px] text-emerald-600 font-semibold block text-center mt-1"><i class="fa-solid fa-check"></i> 코드가 복사되었습니다!</span>
                </div>
                
                <hr class="border-stone-100">

                <div>
                    <label class="block text-xs font-bold text-stone-500 mb-1" for="importCodeInput">가져온 코드 수동 복원하기</label>
                    <textarea id="importCodeInput" placeholder="이곳에 이전에 복사해둔 백업 코드를 붙여넣어 주세요" class="w-full px-3 py-2 rounded-xl border border-stone-200 text-xs h-20 resize-none font-mono focus:outline-emerald-600"></textarea>
                    <button onclick="importShareCode()" class="mt-1.5 w-full bg-emerald-800 hover:bg-emerald-700 text-white text-xs font-bold py-2 rounded-lg transition-all flex items-center justify-center gap-1.5 shadow-sm">
                        <i class="fa-solid fa-cloud-arrow-down"></i> 코드에서 읽기 데이터 복원하기
                    </button>
                </div>
            </div>

            <div class="mt-5 pt-3 border-t border-stone-100 flex justify-end">
                <button onclick="closeShareModal()" class="bg-stone-200 hover:bg-stone-300 text-stone-700 text-xs font-bold px-4 py-2 rounded-xl transition-all">닫기</button>
            </div>
        </div>
    </div>

    <!-- SCRIPT LOGIC (Firebase SDK modules included natively!) -->
    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
        import { getAuth, signInWithCustomToken, signInAnonymously, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
        import { getFirestore, doc, setDoc, getDoc, collection, onSnapshot, updateDoc } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";

        // Full 66 books mapping (1189 chapters)
        const bibleBooks = [
            // Old Testament
            { id: 1, name: "창세기", eng: "Genesis", chapters: 50, category: "구약" },
            { id: 2, name: "출애굽기", eng: "Exodus", chapters: 40, category: "구약" },
            { id: 3, name: "레위기", eng: "Leviticus", chapters: 27, category: "구약" },
            { id: 4, name: "민수기", eng: "Numbers", chapters: 36, category: "구약" },
            { id: 5, name: "신명기", eng: "Deuteronomy", chapters: 34, category: "구약" },
            { id: 6, name: "여호수아", eng: "Joshua", chapters: 24, category: "구약" },
            { id: 7, name: "사사기", eng: "Judges", chapters: 21, category: "구약" },
            { id: 8, name: "룻기", eng: "Ruth", chapters: 4, category: "구약" },
            { id: 9, name: "사무엘상", eng: "1 Samuel", chapters: 31, category: "구약" },
            { id: 10, name: "사무엘하", eng: "2 Samuel", chapters: 24, category: "구약" },
            { id: 11, name: "열왕기상", eng: "1 Kings", chapters: 22, category: "구약" },
            { id: 12, name: "열왕기하", eng: "2 Kings", chapters: 25, category: "구약" },
            { id: 13, name: "역대상", eng: "1 Chronicles", chapters: 29, category: "구약" },
            { id: 14, name: "역대하", eng: "2 Chronicles", chapters: 36, category: "구약" },
            { id: 15, name: "에스라", eng: "Ezra", chapters: 10, category: "구약" },
            { id: 16, name: "느헤미야", eng: "Nehemiah", chapters: 13, category: "구약" },
            { id: 17, name: "에스더", eng: "Esther", chapters: 10, category: "구약" },
            { id: 18, name: "욥기", eng: "Job", chapters: 42, category: "구약" },
            { id: 19, name: "시편", eng: "Psalms", chapters: 150, category: "구약" },
            { id: 20, name: "잠언", eng: "Proverbs", chapters: 31, category: "구약" },
            { id: 21, name: "전도서", eng: "Ecclesiastes", chapters: 12, category: "구약" },
            { id: 22, name: "아가", eng: "Song of Solomon", chapters: 8, category: "구약" },
            { id: 23, name: "이사야", eng: "Isaiah", chapters: 66, category: "구약" },
            { id: 24, name: "예레미야", eng: "Jeremiah", chapters: 52, category: "구약" },
            { id: 25, name: "예레미야 애가", eng: "Lamentations", chapters: 5, category: "구약" },
            { id: 26, name: "에스겔", eng: "Ezekiel", chapters: 48, category: "구약" },
            { id: 27, name: "다니엘", eng: "Daniel", chapters: 12, category: "구약" },
            { id: 28, name: "호세아", eng: "Hosea", chapters: 14, category: "구약" },
            { id: 29, name: "요엘", eng: "Joel", chapters: 3, category: "구약" },
            { id: 30, name: "아모스", eng: "Amos", chapters: 9, category: "구약" },
            { id: 31, name: "오바댜", eng: "Obadiah", chapters: 1, category: "구약" },
            { id: 32, name: "요나", eng: "Jonah", chapters: 4, category: "구약" },
            { id: 33, name: "미가", eng: "Micah", chapters: 7, category: "구약" },
            { id: 34, name: "나훔", eng: "Nahum", chapters: 3, category: "구약" },
            { id: 35, name: "하박국", eng: "Habakkuk", chapters: 3, category: "구약" },
            { id: 36, name: "스바냐", eng: "Zephaniah", chapters: 3, category: "구약" },
            { id: 37, name: "학개", eng: "Haggai", chapters: 2, category: "구약" },
            { id: 38, name: "스가랴", eng: "Zechariah", chapters: 14, category: "구약" },
            { id: 39, name: "말라기", eng: "Malachi", chapters: 4, category: "구약" },

            // New Testament
            { id: 40, name: "마태복음", eng: "Matthew", chapters: 28, category: "신약" },
            { id: 41, name: "마가복음", eng: "Mark", chapters: 16, category: "신약" },
            { id: 42, name: "누가복음", eng: "Luke", chapters: 24, category: "신약" },
            { id: 43, name: "요한복음", eng: "John", chapters: 21, category: "신약" },
            { id: 44, name: "사도행전", eng: "Acts", chapters: 28, category: "신약" },
            { id: 45, name: "로마서", eng: "Romans", chapters: 16, category: "신약" },
            { id: 46, name: "고린도전서", eng: "1 Corinthians", chapters: 16, category: "신약" },
            { id: 47, name: "고린도후서", eng: "2 Corinthians", chapters: 13, category: "신약" },
            { id: 48, name: "갈라디아서", eng: "Galatians", chapters: 6, category: "신약" },
            { id: 49, name: "에베소서", eng: "Ephesians", chapters: 6, category: "신약" },
            { id: 50, name: "빌립보서", eng: "Philippians", chapters: 4, category: "신약" },
            { id: 51, name: "골로새서", eng: "Colossians", chapters: 4, category: "신약" },
            { id: 52, name: "데살로니가전서", eng: "1 Thessalonians", chapters: 5, category: "신약" },
            { id: 53, name: "데살로니가후서", eng: "2 Thessalonians", chapters: 3, category: "신약" },
            { id: 54, name: "디모데전서", eng: "1 Timothy", chapters: 6, category: "신약" },
            { id: 55, name: "디모데후서", eng: "2 Timothy", chapters: 4, category: "신약" },
            { id: 56, name: "디도서", eng: "Titus", chapters: 3, category: "신약" },
            { id: 57, name: "빌레몬서", eng: "Philemon", chapters: 1, category: "신약" },
            { id: 58, name: "히브리서", eng: "Hebrews", chapters: 13, category: "신약" },
            { id: 59, name: "야고보서", eng: "James", chapters: 5, category: "신약" },
            { id: 60, name: "베드로전서", eng: "1 Peter", chapters: 5, category: "신약" },
            { id: 61, name: "베드로후서", eng: "2 Peter", chapters: 3, category: "신약" },
            { id: 62, name: "요한일서", eng: "1 John", chapters: 5, category: "신약" },
            { id: 63, name: "요한이서", eng: "2 John", chapters: 1, category: "신약" },
            { id: 64, name: "요한삼서", eng: "3 John", chapters: 1, category: "신약" },
            { id: 65, name: "유다서", eng: "Jude", chapters: 1, category: "신약" },
            { id: 66, name: "요한계시록", eng: "Revelation", chapters: 22, category: "신약" }
        ];

        // Biblical quotes database
        const versesList = [
            "\"여호와의 율법은 완전하여 영혼을 소성시키며 여호와의 증거는 확실하여 우둔한 자를 지혜롭게 하며\" (시 19:7)",
            "\"이 율법책을 네 입에서 떠나지 말게 하며 주야로 그것을 묵상하여 그 안에 기록된 대로 다 지켜 행하라 그리하면 네 길이 평탄하게 될 것이며 네가 형통하리라\" (수 1:8)",
            "\"주의 말씀은 내 발에 등이요 내 길에 빛이니이다\" (시 119:105)",
            "\"하나님의 말씀은 살아 있고 활력이 있어 좌우에 날선 어떤 검보다도 예리하여 혼과 영과 및 관절과 골수를 찔러 쪼개기까지 하며 또 마음의 생각과 뜻을 판단하나니\" (히 4:12)",
            "\"이 예언의 말씀을 읽는 자와 듣는 자와 그 가운데에 기록한 것을 지키는 자는 복이 있나니 때가 가까움이라\" (계 1:3)",
            "\"모든 성경은 하나님의 감동으로 된 것으로 교훈과 책망과 바르게 함과 의로 교육하기에 유익하니\" (딤후 3:16)"
        ];

        // Theme colors configurations
        const colorClasses = {
            emerald: { primary: 'bg-emerald-600', text: 'text-emerald-700', bg: 'bg-emerald-50', hover: 'hover:bg-emerald-100', border: 'border-emerald-600', ring: 'ring-emerald-500', btnActive: 'bg-emerald-600 text-white' },
            amber: { primary: 'bg-amber-600', text: 'text-amber-700', bg: 'bg-amber-50', hover: 'hover:bg-amber-100', border: 'border-amber-600', ring: 'ring-amber-500', btnActive: 'bg-amber-600 text-white' },
            rose: { primary: 'bg-rose-600', text: 'text-rose-700', bg: 'bg-rose-50', hover: 'hover:bg-rose-100', border: 'border-rose-600', ring: 'ring-rose-500', btnActive: 'bg-rose-600 text-white' },
            blue: { primary: 'bg-blue-600', text: 'text-blue-700', bg: 'bg-blue-50', hover: 'hover:bg-blue-100', border: 'border-blue-600', ring: 'ring-blue-500', btnActive: 'bg-blue-600 text-white' }
        };

        // Application State
        let state = {
            users: {
                "user_1": { name: "나", color: "emerald", progress: {} },
                "user_2": { name: "함께 읽는 분", color: "amber", progress: {} }
            },
            activeUserId: "user_1",
            activeBookId: 1, // Start with Genesis
            categoryFilter: "전체",
            searchQuery: "",
            selectedModalColor: "emerald",
            dailyGoal: 3
        };

        // Firebase & Fallback Wireless Variables
        let db = null;
        let auth = null;
        let appId = 'default-app-id';
        let isFirebaseEnabled = false;
        let currentRoomId = null;
        let roomUnsubscribe = null;
        let currentUser = null;
        
        // Fallback Web Sync Engine configuration (GitHub Pages fallback)
        let fallbackPollInterval = null;
        const FALLBACK_BUCKET = "oz2222_bible_sync_bucket";

        // Custom LocalStorage utility wrapper
        Storage.prototype.setObj = function(key, obj) {
            return this.setItem(key, JSON.stringify(obj))
        }
        Storage.prototype.getObj = function(key) {
            try {
                return JSON.parse(this.getItem(key));
            } catch (e) {
                return null;
            }
        }

        // Initialize App on DOM Loaded
        window.addEventListener('DOMContentLoaded', () => {
            loadStateFromLocalStorage();
            initFirebaseAndAuth();
            renderUsersDropdown();
            renderBibleBooksList();
            renderChapterGrid();
            renderOverallProgress();
            renderTogetherProgressBoard();
            getNewVerse();
            updateDailyGoal();
        });

        // Initialize Firebase dynamically based on environment configuration safely
        async function initFirebaseAndAuth() {
            const hasConfig = typeof __firebase_config !== 'undefined' && __firebase_config;
            
            // 연동 카드는 이제 깃허브에서도 무조건 보여집니다!
            document.getElementById('cloudSyncCard').classList.remove('hidden');

            if (hasConfig) {
                try {
                    const firebaseConfig = JSON.parse(__firebase_config);
                    const app = initializeApp(firebaseConfig);
                    auth = getAuth(app);
                    db = getFirestore(app);
                    appId = typeof __app_id !== 'undefined' ? __app_id : 'default-app-id';
                    isFirebaseEnabled = true;

                    // Rule 3: Authentication FIRST and await it
                    const initAuth = async () => {
                        if (typeof __initial_auth_token !== 'undefined' && __initial_auth_token) {
                            await signInWithCustomToken(auth, __initial_auth_token);
                        } else {
                            await signInAnonymously(auth);
                        }
                    };
                    await initAuth();

                    // Listen to auth states
                    onAuthStateChanged(auth, (user) => {
                        currentUser = user;
                        if (user) {
                            console.log("Firebase 클라우드 연동 완료:", user.uid);
                            // Auto join saved room if present
                            const savedRoomId = localStorage.getItem('bible_together_room_id');
                            if (savedRoomId) {
                                joinCloudRoom(savedRoomId);
                            }
                        }
                    });

                } catch (e) {
                    console.error("Firebase 로딩 실패, 폴백 무선 동기화 엔진으로 전환:", e);
                    setupFallbackSync();
                }
            } else {
                setupFallbackSync();
            }
        }

        // 깃허브 등 독립 배포 환경을 위한 무선 폴백 엔진 가동
        function setupFallbackSync() {
            console.log("로컬 독립 모드 및 퍼블릭 무선 연동 엔진 작동 중.");
            const savedRoomId = localStorage.getItem('bible_together_room_id');
            if (savedRoomId) {
                joinCloudRoom(savedRoomId);
            }
        }

        // 깃허브 폴백 엔진 데이터 가져오기 (API 전송)
        async function fetchFallbackData(roomId) {
            try {
                const res = await fetch(`https://kvdb.io/${FALLBACK_BUCKET}/room_${roomId}`);
                if (res.ok) {
                    const data = await res.json();
                    if (data && data.users) {
                        // 원격 데이터를 로컬 데이터로 병합 (타임스탬프가 최신인 경우에만 덮어씀)
                        Object.keys(data.users).forEach(uid => {
                            const localUser = state.users[uid];
                            const remoteUser = data.users[uid];
                            if (!localUser || !localUser.updatedAt || (remoteUser.updatedAt > (localUser.updatedAt || 0))) {
                                state.users[uid] = remoteUser;
                            }
                        });
                        saveStateToLocalStorage();
                        
                        // 렌더링 업데이트
                        renderUsersDropdown();
                        renderBibleBooksList();
                        renderChapterGrid();
                        renderOverallProgress();
                        renderTogetherProgressBoard();
                    }
                }
            } catch (e) {
                console.error("폴백 수신 에러:", e);
            }
        }

        // 깃허브 폴백 엔진 데이터 저장하기
        async function saveFallbackData(roomId) {
            try {
                const payload = { users: state.users };
                await fetch(`https://kvdb.io/${FALLBACK_BUCKET}/room_${roomId}`, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });
            } catch (e) {
                console.error("폴백 전송 에러:", e);
            }
        }

        // Join a real-time Room safely
        function joinCloudRoom(roomId) {
            currentRoomId = roomId;
            localStorage.setItem('bible_together_room_id', roomId);

            if (isFirebaseEnabled && currentUser) {
                // --- Firebase 실시간 감지 모드 (Canvas 전용) ---
                if (roomUnsubscribe) roomUnsubscribe();
                const roomDocRef = doc(db, 'artifacts', appId, 'public', 'data', 'rooms', roomId);

                roomUnsubscribe = onSnapshot(roomDocRef, (docSnap) => {
                    if (docSnap.exists()) {
                        const data = docSnap.data();
                        if (data && data.users) {
                            Object.keys(data.users).forEach(uid => {
                                state.users[uid] = data.users[uid];
                            });
                            saveStateToLocalStorage();
                            
                            renderUsersDropdown();
                            renderBibleBooksList();
                            renderChapterGrid();
                            renderOverallProgress();
                            renderTogetherProgressBoard();
                        }
                    } else {
                        setDoc(roomDocRef, { users: state.users });
                    }

                    // UI 연동상태 업데이트
                    updateUIForConnected(roomId);
                }, (error) => {
                    console.error("실시간 수신 에러:", error);
                });
            } else {
                // --- 무선 폴백 엔진 모드 (GitHub Pages 전용) ---
                if (fallbackPollInterval) clearInterval(fallbackPollInterval);
                
                // 최초 즉시 동기화
                fetchFallbackData(roomId);
                
                // 4초 주기 폴링 시작
                fallbackPollInterval = setInterval(() => {
                    fetchFallbackData(roomId);
                }, 4000);

                updateUIForConnected(roomId);
            }
        }

        // 연동 연결 성공 시 UI 처리
        function updateUIForConnected(roomId) {
            document.getElementById('cloudStatusIcon').className = "fa-solid fa-cloud text-emerald-600 animate-pulse";
            document.getElementById('cloudStatusBadge').className = "text-[10px] bg-emerald-100 text-emerald-800 px-2 py-0.5 rounded-full font-semibold";
            document.getElementById('cloudStatusBadge').innerText = isFirebaseEnabled ? "연동됨" : "무선 연동됨";
            document.getElementById('cloudStatusDesc').classList.add('hidden');
            document.getElementById('cloudActionForm').classList.add('hidden');
            document.getElementById('cloudActiveForm').classList.remove('hidden');
            document.getElementById('activeRoomNameDisplay').innerText = roomId;
        }

        // Connect room triggers from UI
        async function connectCloudRoom() {
            const inputVal = document.getElementById('cloudRoomInput').value.trim();
            if (!inputVal) {
                alertModal("입력된 방 이름이 없습니다. 방 이름을 입력해 주세요!");
                return;
            }
            joinCloudRoom(inputVal);
            await syncStateToCloud();
        }

        // Disconnect from real-time sync
        function leaveCloudRoom() {
            if (roomUnsubscribe) roomUnsubscribe();
            if (fallbackPollInterval) clearInterval(fallbackPollInterval);
            currentRoomId = null;
            localStorage.removeItem('bible_together_room_id');

            // Reset UI states
            document.getElementById('cloudStatusIcon').className = "fa-solid fa-cloud-arrow-up text-stone-400";
            document.getElementById('cloudStatusBadge').className = "text-[10px] bg-stone-200 text-stone-600 px-2 py-0.5 rounded-full font-semibold";
            document.getElementById('cloudStatusBadge').innerText = "연동 전";
            document.getElementById('cloudStatusDesc').classList.remove('hidden');
            document.getElementById('cloudActionForm').classList.remove('hidden');
            document.getElementById('cloudActiveForm').classList.add('hidden');
            document.getElementById('cloudRoomInput').value = '';
            
            alertModal("실시간 연동이 해제되었습니다. 이제 오프라인으로 기록됩니다.");
        }

        // Push current active user status to database safely
        async function syncStateToCloud() {
            if (!currentRoomId) return;
            
            const myUserObj = state.users[state.activeUserId];
            if (!myUserObj) return;

            // 업데이트 타임스탬프 설정
            myUserObj.updatedAt = Date.now();
            saveStateToLocalStorage();

            if (isFirebaseEnabled && currentUser) {
                // --- Firebase Firestore 업로드 ---
                const roomDocRef = doc(db, 'artifacts', appId, 'public', 'data', 'rooms', currentRoomId);
                try {
                    await updateDoc(roomDocRef, {
                        [`users.${state.activeUserId}`]: {
                            name: myUserObj.name,
                            color: myUserObj.color,
                            progress: myUserObj.progress,
                            updatedAt: myUserObj.updatedAt
                        }
                    });
                } catch (err) {
                    try {
                        await setDoc(roomDocRef, {
                            users: {
                                [state.activeUserId]: {
                                    name: myUserObj.name,
                                    color: myUserObj.color,
                                    progress: myUserObj.progress,
                                    updatedAt: myUserObj.updatedAt
                                }
                            }
                        }, { merge: true });
                    } catch (e) {
                        console.error("클라우드 업로드 에러:", e);
                    }
                }
            } else {
                // --- 폴백 엔진 업로드 ---
                await saveFallbackData(currentRoomId);
            }
        }

        // Load & Save to LocalStorage
        function loadStateFromLocalStorage() {
            const savedState = localStorage.getObj('bible_together_state');
            if (savedState) {
                state = savedState;
            }
        }

        function saveStateToLocalStorage() {
            localStorage.setObj('bible_together_state', state);
        }

        // Toggle User Selector Dropdown
        function toggleUserDropdown() {
            const menu = document.getElementById('userDropdownMenu');
            menu.classList.toggle('hidden');
        }

        // Close dropdown when clicking outside
        document.addEventListener('click', function(e) {
            const btn = document.getElementById('userDropdownBtn');
            const menu = document.getElementById('userDropdownMenu');
            if (btn && menu && !btn.contains(e.target) && !menu.contains(e.target)) {
                menu.classList.add('hidden');
            }
        });

        // Render Dropdown List of Users
        function renderUsersDropdown() {
            const container = document.getElementById('userListContainer');
            container.innerHTML = '';

            const currentUserObj = state.users[state.activeUserId];
            document.getElementById('currentUserDisplay').innerText = currentUserObj ? currentUserObj.name : "사용자 선택";

            Object.keys(state.users).forEach(uid => {
                const user = state.users[uid];
                const activeIndicator = uid === state.activeUserId ? '<i class="fa-solid fa-check text-emerald-600 ml-auto"></i>' : '';
                const item = document.createElement('button');
                item.className = "w-full text-left px-4 py-2 text-sm text-stone-700 hover:bg-stone-50 flex items-center gap-2.5 transition-all";
                item.onclick = () => {
                    switchActiveUser(uid);
                    toggleUserDropdown();
                };
                item.innerHTML = `
                    <div class="w-3.5 h-3.5 rounded-full ${colorClasses[user.color || 'emerald'].primary}"></div>
                    <span class="font-medium">${user.name}</span>
                    ${activeIndicator}
                `;
                container.appendChild(item);
            });
        }

        // Switch Active User
        function switchActiveUser(uid) {
            if (state.users[uid]) {
                state.activeUserId = uid;
                saveStateToLocalStorage();
                renderUsersDropdown();
                renderBibleBooksList();
                renderChapterGrid();
                renderOverallProgress();
                renderTogetherProgressBoard();
                syncStateToCloud();
            }
        }

        // Profile Add Modal Actions
        function openAddUserModal() {
            document.getElementById('newUserName').value = '';
            selectColorBadge('emerald');
            document.getElementById('addUserModal').classList.remove('hidden');
            toggleUserDropdown();
        }

        function closeAddUserModal() {
            document.getElementById('addUserModal').classList.add('hidden');
        }

        // Select profile color scheme
        function selectColorBadge(color) {
            state.selectedModalColor = color;
            document.querySelectorAll('.color-badge').forEach(badge => {
                badge.classList.remove('border-stone-800', 'ring-2');
                badge.classList.add('border-transparent');
            });
            event.target.classList.add('border-stone-800', 'ring-2');
        }

        // Handle adding a new reader/user profile
        function submitNewUser() {
            const nameInput = document.getElementById('newUserName').value.trim();
            if (!nameInput) {
                alertModal("이름을 입력해 주세요.");
                return;
            }

            const newUid = 'user_' + Date.now();
            state.users[newUid] = {
                name: nameInput,
                color: state.selectedModalColor,
                progress: {}
            };

            state.activeUserId = newUid;
            saveStateToLocalStorage();
            closeAddUserModal();
            renderUsersDropdown();
            renderBibleBooksList();
            renderChapterGrid();
            renderOverallProgress();
            renderTogetherProgressBoard();
            syncStateToCloud();
        }

        // Render Bible Books Left Sidebar
        function renderBibleBooksList() {
            const listContainer = document.getElementById('bibleBookList');
            listContainer.innerHTML = '';

            const currentUserObj = state.users[state.activeUserId];
            if (!currentUserObj) return;

            // Filter books based on active tab and search query
            const filteredBooks = bibleBooks.filter(book => {
                const matchesCategory = state.categoryFilter === "전체" || book.category === state.categoryFilter;
                const matchesSearch = book.name.toLowerCase().includes(state.searchQuery.toLowerCase()) || 
                                      book.eng.toLowerCase().includes(state.searchQuery.toLowerCase());
                return matchesCategory && matchesSearch;
            });

            if (filteredBooks.length === 0) {
                listContainer.innerHTML = `<p class="text-center py-6 text-xs text-stone-400">일치하는 성경이 없습니다.</p>`;
                return;
            }

            filteredBooks.forEach(book => {
                const userProgress = currentUserObj.progress[book.id] || [];
                const readCount = userProgress.length;
                const isCompleted = readCount === book.chapters;
                const percent = Math.round((readCount / book.chapters) * 100);

                const bookBtn = document.createElement('button');
                const isActive = book.id === state.activeBookId;
                
                let activeStyle = isActive 
                    ? `bg-stone-100/90 border-l-4 ${colorClasses[currentUserObj.color || 'emerald'].border} shadow-sm font-semibold`
                    : 'hover:bg-stone-50/70 border-l-4 border-transparent';

                bookBtn.className = `w-full text-left p-3 flex items-center justify-between text-stone-700 transition-all ${activeStyle}`;
                bookBtn.onclick = () => selectBibleBook(book.id);

                bookBtn.innerHTML = `
                    <div class="flex flex-col font-medium">
                        <span class="text-sm tracking-wide flex items-center gap-1.5 font-bold">
                            ${book.name}
                            ${isCompleted ? `<i class="fa-solid fa-circle-check text-[11px] text-emerald-500"></i>` : ''}
                        </span>
                        <span class="text-[10px] text-stone-400 font-normal">${book.eng} &middot; 총 ${book.chapters}장</span>
                    </div>
                    <div class="text-right flex flex-col items-end gap-1">
                        <span class="text-xs font-bold text-stone-600">${readCount}/${book.chapters}장</span>
                        <!-- Tiny Progress Bar -->
                        <div class="w-16 h-1 bg-stone-100 rounded-full overflow-hidden">
                            <div class="h-full ${colorClasses[currentUserObj.color || 'emerald'].primary}" style="width: ${percent}%"></div>
                        </div>
                    </div>
                `;
                listContainer.appendChild(bookBtn);
            });
        }

        // Search bible books filter
        function searchBibleBook() {
            state.searchQuery = document.getElementById('searchInput').value;
            renderBibleBooksList();
        }

        // Category tabs filter
        function filterBibleCategory(category) {
            state.categoryFilter = category;
            
            // Adjust Active Class on Tabs
            document.querySelectorAll('.category-tab').forEach(tab => {
                tab.classList.remove('bg-white', 'text-stone-800', 'shadow-sm');
                tab.classList.add('text-stone-500');
            });

            const activeTab = document.getElementById(`tabBtn_${category}`);
            if (activeTab) {
                activeTab.classList.remove('text-stone-500');
                activeTab.classList.add('bg-white', 'text-stone-800', 'shadow-sm');
            }

            renderBibleBooksList();
        }

        // Change Selected Active Book
        function selectBibleBook(bookId) {
            state.activeBookId = bookId;
            saveStateToLocalStorage();
            renderBibleBooksList();
            renderChapterGrid();
        }

        // Render Main Chapters Grid
        function renderChapterGrid() {
            const book = bibleBooks.find(b => b.id === state.activeBookId);
            if (!book) return;

            const currentUserObj = state.users[state.activeUserId];
            if (!currentUserObj) return;

            // Set headers
            document.getElementById('activeBookName').innerText = book.name;
            document.getElementById('activeBookEnglish').innerText = book.eng;
            
            const userProgress = currentUserObj.progress[book.id] || [];
            document.getElementById('activeBookProgressText').innerText = `읽은 진도: ${userProgress.length} / ${book.chapters}장 (${Math.round((userProgress.length / book.chapters)*100)}%)`;

            const container = document.getElementById('chapterMatrixContainer');
            container.innerHTML = '';

            // Grid Container creation
            const grid = document.createElement('div');
            grid.className = "grid grid-cols-5 sm:grid-cols-6 md:grid-cols-8 gap-2 pb-6";

            for (let ch = 1; ch <= book.chapters; ch++) {
                const isChecked = userProgress.includes(ch);
                const btn = document.createElement('button');
                
                // Color configuration depending on profile theme
                const userTheme = colorClasses[currentUserObj.color || 'emerald'];
                
                let btnStyle = isChecked
                    ? `${userTheme.primary} text-white font-bold border-transparent shadow-sm scale-95`
                    : 'bg-stone-50/70 hover:bg-stone-100 text-stone-600 border border-stone-200/60';

                btn.className = `chapter-btn h-11 w-full rounded-xl text-xs flex flex-col items-center justify-center font-semibold ${btnStyle}`;
                btn.onclick = () => toggleChapter(book.id, ch);
                
                btn.innerHTML = `
                    <span>${ch}장</span>
                    ${isChecked ? '<i class="fa-solid fa-check text-[9px] mt-0.5 opacity-90"></i>' : '<span class="text-[9px] opacity-20 hover:opacity-100">&bull;</span>'}
                `;
                grid.appendChild(btn);
            }

            container.appendChild(grid);
            
            // Sync current book chapters limit with range helper maximum
            document.getElementById('bulkRangeValue').max = book.chapters;
            if (parseInt(document.getElementById('bulkRangeValue').value) > book.chapters) {
                document.getElementById('bulkRangeValue').value = book.chapters;
            }
        }

        // Toggle Chapter check and update cloud database
        function toggleChapter(bookId, chapterNum) {
            const currentUserObj = state.users[state.activeUserId];
            if (!currentUserObj) return;

            if (!currentUserObj.progress[bookId]) {
                currentUserObj.progress[bookId] = [];
            }

            const chapterIndex = currentUserObj.progress[bookId].indexOf(chapterNum);
            if (chapterIndex > -1) {
                currentUserObj.progress[bookId].splice(chapterIndex, 1);
            } else {
                currentUserObj.progress[bookId].push(chapterNum);
            }

            saveStateToLocalStorage();
            renderChapterGrid();
            renderBibleBooksList();
            renderOverallProgress();
            renderTogetherProgressBoard();
            syncStateToCloud();
        }

        // Bulk Actions inside Book
        function bulkCheckActiveBook(isCheckAll) {
            const book = bibleBooks.find(b => b.id === state.activeBookId);
            if (!book) return;

            const currentUserObj = state.users[state.activeUserId];
            if (!currentUserObj) return;

            if (isCheckAll) {
                const allCh = Array.from({ length: book.chapters }, (_, i) => i + 1);
                currentUserObj.progress[book.id] = allCh;
            } else {
                currentUserObj.progress[book.id] = [];
            }

            saveStateToLocalStorage();
            renderChapterGrid();
            renderBibleBooksList();
            renderOverallProgress();
            renderTogetherProgressBoard();
            syncStateToCloud();
        }

        // Check Up To specific chapter range
        function checkUpToRange() {
            const book = bibleBooks.find(b => b.id === state.activeBookId);
            if (!book) return;

            const targetVal = parseInt(document.getElementById('bulkRangeValue').value);
            if (isNaN(targetVal) || targetVal < 1 || targetVal > book.chapters) {
                alertModal(`1장부터 ${book.chapters}장 사이에서 올바른 숫자를 입력해 주세요.`);
                return;
            }

            const currentUserObj = state.users[state.activeUserId];
            if (!currentUserObj) return;

            currentUserObj.progress[book.id] = Array.from({ length: targetVal }, (_, i) => i + 1);

            saveStateToLocalStorage();
            renderChapterGrid();
            renderBibleBooksList();
            renderOverallProgress();
            renderTogetherProgressBoard();
            syncStateToCloud();
        }

        // Calculates count of read chapters for a specific user object
        function getUserTotalCount(userObj) {
            let total = 0;
            let otTotal = 0;
            let ntTotal = 0;

            bibleBooks.forEach(book => {
                const readChapters = userObj.progress[book.id] || [];
                total += readChapters.length;
                if (book.category === "구약") {
                    otTotal += readChapters.length;
                } else {
                    ntTotal += readChapters.length;
                }
            });

            return { total, otTotal, ntTotal };
        }

        // Render Overall User Statistics & Progress Ring
        function renderOverallProgress() {
            const currentUserObj = state.users[state.activeUserId];
            if (!currentUserObj) return;

            const theme = colorClasses[currentUserObj.color || 'emerald'];
            const badgeColor = document.getElementById('userBadgeColor');
            badgeColor.className = `w-4 h-4 rounded-full ${theme.primary}`;
            document.getElementById('activeUserName').innerText = currentUserObj.name;

            const stats = getUserTotalCount(currentUserObj);
            const overallTotal = 1189;

            const percentage = Math.round((stats.total / overallTotal) * 100);

            // Update Statistics texts
            document.getElementById('totalCheckedChapters').innerText = stats.total.toLocaleString();
            document.getElementById('otProgressText').innerText = `${stats.otTotal} / 929`;
            document.getElementById('ntProgressText').innerText = `${stats.ntTotal} / 260`;
            document.getElementById('progressPercentage').innerText = `${percentage}%`;

            // Update Progress Ring SVG
            const circle = document.getElementById('progressRing');
            const radius = circle.r.baseVal.value;
            const circumference = 2 * Math.PI * radius;
            const strokeDashoffset = circumference - (percentage / 100) * circumference;
            circle.style.strokeDasharray = `${circumference} ${circumference}`;
            circle.style.strokeDashoffset = strokeDashoffset;
            circle.style.stroke = currentUserObj.color === 'emerald' ? '#10b981' :
                               currentUserObj.color === 'amber' ? '#f59e0b' :
                               currentUserObj.color === 'rose' ? '#f43f5e' : '#6366f1';

            // Estimated Completed date calculations
            calculateCompletionDate(stats.total);
        }

        // Render Comparison board "Together Board"
        function renderTogetherProgressBoard() {
            const board = document.getElementById('compareUsersContainer');
            board.innerHTML = '';

            const uids = Object.keys(state.users);
            uids.forEach(uid => {
                const user = state.users[uid];
                const stats = getUserTotalCount(user);
                const percent = Math.round((stats.total / 1189) * 100);
                const userTheme = colorClasses[user.color || 'emerald'];

                const userProgressRow = document.createElement('div');
                userProgressRow.className = "space-y-1.5 p-2 rounded-xl transition-all " + (uid === state.activeUserId ? 'bg-stone-50 border border-stone-200/40 shadow-sm' : '');
                
                userProgressRow.innerHTML = `
                    <div class="flex justify-between items-center text-xs">
                        <div class="flex items-center gap-2 font-semibold">
                            <span class="w-2.5 h-2.5 rounded-full ${userTheme.primary}"></span>
                            <span class="text-stone-700">${user.name}</span>
                            ${uid === state.activeUserId ? '<span class="text-[9px] bg-emerald-100 text-emerald-800 px-1 rounded font-bold">선택됨</span>' : ''}
                        </div>
                        <span class="font-bold text-stone-600">${percent}% <span class="text-[10px] text-stone-400 font-normal">(${stats.total}장)</span></span>
                    </div>
                    <div class="w-full h-3 bg-stone-100 rounded-full overflow-hidden relative cursor-pointer" onclick="switchActiveUser('${uid}')" title="${user.name} 프로필로 진도 기록하기">
                        <div class="h-full ${userTheme.primary} rounded-full transition-all duration-500" style="width: ${percent}%"></div>
                    </div>
                `;
                board.appendChild(userProgressRow);
            });
        }

        // Update Daily Goal to calculate completion timeline
        function updateDailyGoal() {
            const val = parseInt(document.getElementById('dailyGoalInput').value);
            if (isNaN(val) || val < 1) {
                state.dailyGoal = 3;
            } else {
                state.dailyGoal = val;
            }
            saveStateToLocalStorage();
            
            const currentUserObj = state.users[state.activeUserId];
            if (currentUserObj) {
                const stats = getUserTotalCount(currentUserObj);
                calculateCompletionDate(stats.total);
            }
        }

        // Completion days calculation helper
        function calculateCompletionDate(totalRead) {
            const totalRemaining = 1189 - totalRead;
            const daysRemaining = Math.ceil(totalRemaining / state.dailyGoal);
            
            document.getElementById('remainingDaysDisplay').innerText = `약 ${daysRemaining}일 남음`;

            // Calculate expected completed date
            if (totalRemaining <= 0) {
                document.getElementById('bibleCompleteDateEstimation').innerText = "🎉 성경 완독 완료!";
                return;
            }

            const today = new Date();
            today.setDate(today.getDate() + daysRemaining);
            const options = { year: 'numeric', month: 'long', day: 'numeric' };
            const formattedDate = today.toLocaleDateString('ko-KR', options);

            document.getElementById('bibleCompleteDateEstimation').innerText = `완독 예정일: ${formattedDate}`;
        }

        // Bible Verse Motivation Slider alternative
        let lastQuoteIndex = -1;
        function getNewVerse() {
            let nextIndex = Math.floor(Math.random() * versesList.length);
            while(nextIndex === lastQuoteIndex) {
                nextIndex = Math.floor(Math.random() * versesList.length);
            }
            lastQuoteIndex = nextIndex;
            document.getElementById('motivationalVerse').innerText = versesList[nextIndex];
        }

        // Data sharing modal & export encoding
        function openShareModal() {
            const rawJson = JSON.stringify(state);
            const base64Code = btoa(encodeURIComponent(rawJson));
            document.getElementById('shareCodeTextarea').value = base64Code;
            document.getElementById('importCodeInput').value = '';
            document.getElementById('copySuccessMsg').classList.add('hidden');
            document.getElementById('shareModal').classList.remove('hidden');
        }

        function closeShareModal() {
            document.getElementById('shareModal').classList.add('hidden');
        }

        // Use clipboard copy with compatibility fallback for iframe environments
        function copyShareCode() {
            const txt = document.getElementById('shareCodeTextarea');
            txt.select();
            txt.setSelectionRange(0, 99999);
            
            try {
                const successful = document.execCommand('copy');
                if (successful) {
                    const msg = document.getElementById('copySuccessMsg');
                    msg.classList.remove('hidden');
                    setTimeout(() => {
                        msg.classList.add('hidden');
                    }, 3000);
                }
            } catch (err) {
                alertModal("복사에 실패했습니다. 공유 코드 텍스트 영역을 직접 꾹 누르고 복사해 주세요.");
            }
        }

        function importShareCode() {
            const rawInput = document.getElementById('importCodeInput').value.trim();
            if (!rawInput) {
                alertModal("공유된 코드를 입력 상자에 채워 넣어주세요.");
                return;
            }

            try {
                const decodedJson = decodeURIComponent(atob(rawInput));
                const parsedState = JSON.parse(decodedJson);

                if (parsedState && parsedState.users && typeof parsedState.users === 'object') {
                    if (confirmModal("읽기 진도 데이터를 가져오시겠습니까? 현재 기기에 저장된 기존 데이터는 완전히 대체됩니다.")) {
                        state = parsedState;
                        saveStateToLocalStorage();
                        closeShareModal();
                        
                        renderUsersDropdown();
                        renderBibleBooksList();
                        renderChapterGrid();
                        renderOverallProgress();
                        renderTogetherProgressBoard();
                        alertModal("성공적으로 데이터를 불러왔습니다!");
                    }
                } else {
                    alertModal("코드가 올바르지 않거나 손상되었습니다. 다시 확인해 주세요.");
                }
            } catch (err) {
                alertModal("코드를 해석할 수 없습니다. 올바른 텍스트를 복사하셨는지 확인해 주세요.");
            }
        }

        // CUSTOM MODALS TO REPLACE BROWSER DEFAULT DIALOGS
        function alertModal(message) {
            const div = document.createElement('div');
            div.className = "fixed inset-0 bg-stone-900/60 backdrop-blur-xs flex items-center justify-center z-[100] p-4";
            div.innerHTML = `
                <div class="bg-white p-5 rounded-2xl max-w-sm w-full shadow-2xl animate-scale-up border border-stone-100 text-center">
                    <p class="text-sm text-stone-700 font-medium leading-relaxed mb-4">${message}</p>
                    <button id="alertCloseBtn" class="bg-emerald-800 hover:bg-emerald-700 text-white font-bold px-5 py-1.5 rounded-xl text-xs transition-all">확인</button>
                </div>
            `;
            document.body.appendChild(div);
            document.getElementById('alertCloseBtn').onclick = () => {
                document.body.removeChild(div);
            };
        }

        function confirmModal(message) {
            return confirm(message);
        }

        // Global Variable Mapping for compatibility with legacy HTML inline onclick events (Canvas requirement)
        window.toggleUserDropdown = toggleUserDropdown;
        window.openAddUserModal = openAddUserModal;
        window.closeAddUserModal = closeAddUserModal;
        window.selectColorBadge = selectColorBadge;
        window.submitNewUser = submitNewUser;
        window.filterBibleCategory = filterBibleCategory;
        window.searchBibleBook = searchBibleBook;
        window.selectBibleBook = selectBibleBook;
        window.bulkCheckActiveBook = bulkCheckActiveBook;
        window.toggleChapter = toggleChapter;
        window.checkUpToRange = checkUpToRange;
        window.updateDailyGoal = updateDailyGoal;
        window.getNewVerse = getNewVerse;
        window.openShareModal = openShareModal;
        window.closeShareModal = closeShareModal;
        window.copyShareCode = copyShareCode;
        window.importShareCode = importShareCode;
        window.switchActiveUser = switchActiveUser;
        
        // Cloud handlers
        window.connectCloudRoom = connectCloudRoom;
        window.leaveCloudRoom = leaveCloudRoom;
    </script>
</body>
</html>