<!DOCTYPE html>
<html>
<head>
	<title>TailwindCSS</title>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0,">
	<title>{% block title %}Django Boards{% endblock %}</title>
	<link href="https://cdn.jsdelivr.net/npm/tailwindcss/dist/tailwind.min.css" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss/dist/preflight.min.css" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss/dist/utilities.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.css">
</head>
<body>

    <!-- Awal Navigasi Bagia Atas, Search Box contohnya -->
	<nav class="flex items-center justify-between flex-wrap bg-green-lighter p-2">
         <div class="flex items-center flex-no-shrink text-black pl-4 mr-6">
             <svg class="fill-current h-8 w-8 mr-2" width="54" height="54" viewBox="0 0 54 54" xmlns="http://www.w3.org/2000/svg">
                 <path d="M13.5 22.1c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05zM0 38.3c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05z"/>
             </svg>
             <span class="line-through font-semibold text-xl tracking-tight">Soedarhana</span>
         </div>

        <!-- Bagian Awal Button Doc,Exam, Blog -->
        <div class="w-full block flex-grow lg:flex lg:items-center lg:w-auto">
            <div class="text-sm lg:flex-grow">
              <a href="#responsive-header" class="no-underline bg-transparent hover:bg-blue text-blue-dark font-semibold hover:text-white m-4 py-2 px-4 border border-blue hover:border-transparent rounded">
                Docs
              </a>
              <a href="#responsive-header" class="no-underline bg-transparent hover:bg-blue text-blue-dark font-semibold hover:text-white m-4 py-2 px-4 border border-blue hover:border-transparent rounded">
                Examples
              </a>
              <a href="#responsive-header" class="no-underline bg-transparent hover:bg-blue text-blue-dark font-semibold hover:text-white m-4 py-2 px-4 border border-blue hover:border-transparent rounded">
                Blog
              </a>
            </div>


            <!-- Awal Search Box -->
            <div class="relative mr-6 my-2">
              <input type="search" class="text-green-darker sm:text-blue-darker lg:text-green-dark tracking-wide bg-purple-white shadow rounded border-0 p-3" placeholder="Search...">
              <div class="absolute pin-r pin-t mt-3 mr-4 text-purple-lighter">
                <svg version="1.1" class="h-4 text-dark" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
                 viewBox="0 0 52.966 52.966" style="enable-background:new 0 0 52.966 52.966;" xml:space="preserve">
                    <path d="M51.704,51.273L36.845,35.82c3.79-3.801,6.138-9.041,6.138-14.82c0-11.58-9.42-21-21-21s-21,9.42-21,21s9.42,21,21,21
                    c5.083,0,9.748-1.817,13.384-4.832l14.895,15.491c0.196,0.205,0.458,0.307,0.721,0.307c0.25,0,0.499-0.093,0.693-0.279
                    C52.074,52.304,52.086,51.671,51.704,51.273z M21.983,40c-10.477,0-19-8.523-19-19s8.523-19,19-19s19,8.523,19,19
                    S32.459,40,21.983,40z"/>

                </svg>
              </div>
            </div>
            <!-- Akhir Search Box -->


            <!-- Bagian Login / Daftar -->
            <div class="hover:text-blue">
                <form class="w-full max-w-sm">
                    <button class="bg-blue text-white font-bold py-2 px-4 border-b-4 hover:border-b-2 hover:border-t-2 border-blue-dark hover:border-blue rounded" type="button">
                      Sign Up
                    </button>
                    <button class="bg-blue text-white font-bold py-2 px-4 border-b-4 hover:border-b-2 hover:border-t-2 border-blue-dark hover:border-blue rounded" type="button">
                      Login
                    </button>
                  </div>
                </form>
            </div>
            <!-- Akhir Login / Daftar -->

        </div>
        <!-- Akhir Button -->

    </nav>
    <!-- Akhir Navigasi Atas -->

    <!-- Awal Isi bagian Body -->
    <div id="wrapper" class="flex h-screen bg-grey-lightest sm:flex-col md:flex-row font-light w-full pr-5 mt-1">
       <div id="sidebar" class="bg-orange-darker md:w-64 sm:w-screen">
            <header class="flex justify-between items-center border-b border-orange-darkest pt-8 pb-8 pl-6 pr-6">
                <div id="logo" class="no-underline text-white md:text-2xl sm:text-4xl font-bold">
                    <img src="https://files.slack.com/files-pri/T5Q1A6MC6-FC164U14N/logo_whizkids_baru_kemeja.png" width="50" alt="">
                        DevSubang
                </div>
                <div id="collapse" class="text-white border border-white p-2 h-8 rounded">
                    <i class="fa fa-bars" aria-hidden="true"></i>
                </div>
            </header>
            <div id="profile" class="flex items-center border-b border-orange-darkest px-8 py-6">
                <div id="img" class="w-1/4">
                    <img src="https://avatars3.githubusercontent.com/u/40782378?s=400&u=ef41e525045df98a415de30a041a7362f9213222&v=4" width="55" alt="" class="rounded-full">
                </div>
                <div id="welcome" class="text-white w-2/4 sm:ml-1 md:ml-4">
                    <p class="text-xs">Welcome,</p>
                    <span class="text-lg">Soedarhana</span>
                </div>
            </div>
            <ul id="menu" class="flex flex-col list-reset sm:hidden md:block">
                <li class="block">
                    <a href="#" class="no-underline text-white block h-full w-full border-b border-orange-darkest px-8 py-4 hover:text-orange">
                        <i class="fa fa-tachometer mr-2" aria-hidden="true"></i>
                        Dashboard
                    </a>
                </li>
                <li class="flex justify-between block">
                    <a href="#" class="no-underline text-white block h-full w-full border-b border-orange-darkest px-8 py-4 hover:text-orange">
                        <i class="fa fa-user mr-2" aria-hidden="true"></i>
                        Account
                        <i class="fa fa-angle-right float-right" aria-hidden="true"></i>
                    </a>
                </li>
                <li class="block">
                    <a href="#" class="no-underline text-white block h-full w-full border-b border-orange-darkest px-8 py-4 hover:text-orange">
                        <i class="fa fa-envelope mr-2" aria-hidden="true"></i>
                        MailBox
                        <i class="fa fa-angle-down float-right" aria-hidden="true"></i>
                    </a>
                    <ul class="flex flex-col list-reset bg-orange-darkest block">
                        <li class="flex block border-b border-orange-darker">
                            <a href="#" class="no-underline text-white block h-full w-full ml-4 hover:text-orange px-8 py-4">
                                <i class="fa fa-envelope-o mr-2" aria-hidden="true"></i>
                                Inbox
                            </a>
                        </li>
                        <li class="flex block border-b border-orange-darker">
                            <a href="#" class="no-underline text-white block h-full w-full ml-4 hover:text-orange px-8 py-4">
                                <i class="fa fa-envelope-o mr-2" aria-hidden="true"></i>
                                Categories
                                <i class="fa fa-angle-down float-right" aria-hidden="true"></i>
                            </a>
                        </li>
                        <ul class="flex flex-col list-reset bg-orange-darkest block">
                            <li class="flex block border-b border-orange-darker">
                                <a href="#" class="no-underline text-white block h-full w-full ml-8 hover:text-orange px-8 py-4">
                                    <i class="fa fa-envelope-o mr-2" aria-hidden="true"></i>
                                    Social
                                </a>
                            </li>
                            <li class="flex block border-b border-orange-darker">
                                <a href="#" class="no-underline text-white block h-full w-full ml-8 hover:text-orange px-8 py-4">
                                    <i class="fa fa-envelope-o mr-2" aria-hidden="true"></i>
                                    Notifications
                                </a>
                            </li>
                        </ul>
                    </ul>
                </li>
            </ul>
        </div>

        <div id="content" class="px-8 bg-transparent flex-grow flex-shrink flex-auto">
            <div id="info" class="border-b border-grey-light h-24">
                <div class="flex justify-between flex-grow items-center border-b h-24">
                    <div class="flex">
                        <ul class="flex list-reset text-black">
                            <li class="py-4 px-4">
                                <i class="fa fa-exclamation-triangle" aria-hidden="true">
                                    <svg class="stroke-current text-purple inline-block h-8 w-8" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" fill="none" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <circle cx="8" cy="21" r="2"></circle>
                                        <circle cx="20" cy="21" r="2"></circle>
                                        <path d="M5.67 6H23l-1.68 8.39a2 2 0 0 1-2 1.61H8.75a2 2 0 0 1-2-1.74L5.23 2.74A2 2 0 0 0 3.25 1H1"></path>
                                    </svg>
                                </i>
                            </li>
                        </ul>
                    </div>

                    <!-- Awal Chat & Ask Free -->
                    <div class="flex">
                        <ul class="flex list-reset text-black">
                            <li class="px-4">
                                <span class="text-sm">
                                    <i class="fa fa-comments" aria-hidden="true"></i>
                                    Chat
                                </span>
                            </li>
                            <li class="border-l px-4">
                                <span class="text-sm">
                                    Ask Free
                                    <i class="fa fa-sign-out" aria-hidden="true"></i>
                                </span>
                            </li>
                        </ul>
                    </div>
                    <!-- Akhir Chat & Ask Free -->

                </div>
            </div>

            <!-- Konten atau isi web -->
            <div class="absolute pin-y  pt-2 pb-5 mb-5 mt-20 bg-grey-lightest mr-10 w-auto bg-grey h-screen overflow-y-scroll">
                <h1 class="font-serif pb-2">Tentang Kita : Terelie</h1>
                <p>SVG dibuat menggunakan XML, sehingga itu adalah gratis dan open. (tidak ada badan/perusahaan yang "memiliki" format SVG).
                    Anda dapat membuat gambar SVG dengan menggunakan editor text biasa seperti Notepad. Dengan statement diatas,
                    maka kita bisa menemukan gambar-gambar SVG digunakan dalam komunitas "open source". Untuk contoh, semua logo dan
                    diagram di Wikipedia menggunakan SVG.
                </p> <br>

                <p>
                    SVG dibuat menggunakan XML, sehingga itu adalah gratis dan open. (tidak ada badan/perusahaan yang "memiliki" format SVG).
                    Anda dapat membuat gambar SVG dengan menggunakan editor text biasa seperti Notepad. Dengan statement diatas,
                    maka kita bisa menemukan gambar-gambar SVG digunakan dalam komunitas "open source". Untuk contoh, semua logo dan
                    diagram di Wikipedia menggunakan SVG.
                </p> <br>

                <p>
                    SVG dibuat menggunakan XML, sehingga itu adalah gratis dan open. (tidak ada badan/perusahaan yang "memiliki" format SVG).
                    Anda dapat membuat gambar SVG dengan menggunakan editor text biasa seperti Notepad. Dengan statement diatas,
                    maka kita bisa menemukan gambar-gambar SVG digunakan dalam komunitas "open source". Untuk contoh, semua logo dan
                    diagram di Wikipedia menggunakan SVG.
                </p> <br>

                <h2 class="font-sans pb-2">Subang Maju</h2>
                <p>
                    SUBANG adalah sebuah kecamatan yang juga merupakan pusat pemerintahan (ibu kota) Kabupaten Subang, Provinsi Jawa Barat, Indonesia.
                    Tofograpi Subang pedataran sampai bergelombang 70%, bergelombang sampai berbukit 20%, berbukit sampai bergunung 10% dengan
                    ketinggian 144 meter di atas permukaan laut.
                </p> <br>

                <p>
                    Letak Lokasi Kabupaten Subang berdasarkan informasi yang didapat dari web resmi pemerintah Kabupaten Subang
                    sebagai salah satu kabupaten di kawasan utara Provinsi Jawa Barat meliputi wilayah seluas 205.176,95 ha atau 6,34 % dari
                    luas Provinsi Jawa Barat. Wilayah ini terletak di antara 107º 31′ sampai dengan 107º 54′ Bujur Timur dan 6º 11′
                    sampai dengan 6º 49′ Lintang Selatan.
                </p> <br>

                <p>
                    Secara administratif, Kabupaten Subang terbagi atas 253 desa dan kelurahan yang tergabung dalam 22 kecamatan.
                    Berdasarkan Peraturan Daerah Kabupaten Subang Nomor 3 Tahun 2007 tentang Pembentukan Wilayah Kerja Camat,
                    jumlah kecamatan bertambah menjadi 30 kecamatan.
                </p> <br>

                <p>
                    Prasejarah Bukti adanya kelompok masyarakat pada masa prasejarah di wilayah Kabupaten Subang adalah
                    ditemukannya kapak batu di daerah Bojongkeding (Binong), Pagaden, Kalijati dan Dayeuhkolot (Sagalaherang).
                    Temuan benda-benda prasejarah bercorak neolitikum ini menandakan bahwa saat itu di wilayah Kabupaten Subang
                    sekarang sudah ada kelompok masyarakat yang hidup dari sektor pertanian dengan pola sangat sederhana.
                    Selain itu, dalam periode prasejarah juga berkembang pula pola kebudayaan perunggu yang ditandai
                    dengan penemuan situs di Kampung Engkel, Sagalaherang.
                </p> <br>

                <h2 class="font-serif pb-2 uppercase">Sejarah Subang</h2>
                <p>
                    Hindu Pada saat berkembangnya corak kebudayaan Hindu, wilayah Kabupaten Subang menjadi bagian dari 3 kerajaan,
                    yakni Tarumanagara, Galuh, dan Pajajaran. Selama berkuasanya 3 kerajaan tersebut, dari wilayah Kabupaten Subang
                    diperkirakan sudah ada kontak-kontek dengan beberapa kerajaan maritim hingga di luar kawasan Nusantara.
                    Peninggalan berupa pecahan-pecahan keramik asal Cina di Patenggeng (Kalijati) membuktikan bahwa selama abad ke-7
                    hingga abad ke-15 sudah terjalin kontak perdagangan dengan wilayah yang jauh. Sumber lain menyebutkan
                    bahwa pada masa tersebut, wilayah Subang berada di bawah kekuasaan Kerajaan Sunda. Kesaksian Tome’
                    Pires seorang Portugis yang mengadakan perjalanan keliling Nusantara menyebutkan bahwa saat menelusuri pantai utara Jawa,
                    kawasan sebelah timur Sungai Cimanuk hingga Banten adalah wilayah kerajaan Sunda.
                </p> <br>
            </div>
            <!-- Akhir konten -->
        </div>
    </div>
    <!-- Akhir Isi bagian Body -->


    <!-- Footer, Feedback Aboutme DLL -->
    <section class="no-underline relative pin-x pin-b bg-black py-5 w-full mt-1">
        <div class="container mx-auto px-8">
            <div class="table w-full">
                <div class="block sm:table-cell">
                    <p class="uppercase text-white text-sm sm:mb-6">Links</p>
                    <ul class="list-reset text-xs mb-6">
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="no-underline text-white hover:text-grey-light">FAQ</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="no-underline text-white hover:text-grey-light">Help</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="no-underline text-white hover:text-grey-light">Support</a>
                        </li>
                    </ul>
                </div>
                <div class="block sm:table-cell">
                    <p class="uppercase text-white text-sm sm:mb-6">Legal</p>
                    <ul class="list-reset text-xs mb-6">
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="no-underline text-white hover:text-grey-light">Terms</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="no-underline text-white hover:text-grey-light">Privacy</a>
                        </li>
                    </ul>
                </div>
                <div class="block sm:table-cell">
                    <p class="uppercase text-white text-sm sm:mb-6">Social</p>
                    <ul class="list-reset text-xs mb-6">
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="no-underline text-white hover:text-grey-light">Facebook</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="no-underline text-white hover:text-grey-light">Linkedin</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="no-underline text-white hover:text-grey-light">Twitter</a>
                        </li>
                    </ul>
                </div>
                <div class="block sm:table-cell">
                    <p class="uppercase text-white text-sm sm:mb-6">Company</p>
                    <ul class="list-reset text-xs mb-6">
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="no-underline text-white hover:text-grey-light">Official Blog</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="no-underline text-white hover:text-grey-light">About Us</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="no-underline text-white hover:text-grey-light">Contact</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
    <!-- Akhir Footer -->

</body>
</html>
