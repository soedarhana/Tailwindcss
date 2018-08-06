<!DOCTYPE html>
<html>
<head>
	<title>TailwindCSS</title>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0,">
	<title>{% block title %}Django Boards{% endblock %}</title>
	<link href="https://cdn.jsdelivr.net/npm/tailwindcss/dist/tailwind.min.css" rel="stylesheet">
</head>
<body class="bg-grey-lightest ml-20 mr-20 mt-5">

	<nav class="flex items-center justify-between flex-wrap bg-green-lighter p-2">
         <div class="flex items-center flex-no-shrink text-black mr-6">
             <svg class="fill-current h-8 w-8 mr-2" width="54" height="54" viewBox="0 0 54 54" xmlns="http://www.w3.org/2000/svg">
                 <path d="M13.5 22.1c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05zM0 38.3c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05z"/>
             </svg>
             <span class="line-through font-semibold text-xl tracking-tight">Soedarhana</span>
         </div>

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


            <div class="relative mr-6 my-2">
              <input type="search" class="text-green-darker sm:text-blue-darker lg:text-green-dark text-center tracking-wide bg-purple-white shadow rounded border-0 p-3" placeholder="Search by name...">
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

        </div>

    </nav>


    <div class="container leading-normal my-4 mx-auto px-4">
        <div class="body">
            <div class="#">
                <h1 class="md:font-sans lg:font-serif text-3xl md:text-5xl text-green-darker sm:text-blue-darker lg:text-green-dark text-center tracking-wide uppercase">Hello , And Welcome To <a class="no-underline text-green-darker hover:text-green-dark" href="http://bekassekolah.blogspot.com/">my WEB</a></h1>
                <p>
                    What is Lorem Ipsum?
                Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.
                </p> <br>

                <h2 class="md:font-sans lg:font-serif text-2xl md:text-3xl text-green-light sm:text-blue-darker lg:text-green-lighter tracking-wide"><a class="no-underline text-green-darker hover:underline hover:text-green-dark" href="#">Find Me In YouTube</a></h2>
                <p>
                    What is Lorem Ipsum?
                Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
                </p> <br>

                <h2 class="md:font-sans lg:font-serif text-pink-light text-2xl md:text-3xl sm:text-blue-darker lg:text-pink-lighter tracking-wide"><a class="no-underline" href="https://www.facebook.com/soedarhana.gambayana">My Facebook</a></h2>
                <p>
                    What is Lorem Ipsum?
                Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
                </p> <br>
            </div>


            <div class="#">
                Ieu Isi kr di Kanan
            </div>
        </div>
    </div>

    <section class="bg-grey-dark py-6 w-full">
        <div class="container mx-auto px-8">
            <div class="table w-full">
                <div class="block sm:table-cell">
                    <p class="uppercase text-white text-sm sm:mb-6">Links</p>
                    <ul class="list-reset text-xs mb-6">
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="text-white hover:text-grey-light">FAQ</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="text-white hover:text-grey-light">Help</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="text-white hover:text-grey-light">Support</a>
                        </li>
                    </ul>
                </div>
                <div class="block sm:table-cell">
                    <p class="uppercase text-white text-sm sm:mb-6">Legal</p>
                    <ul class="list-reset text-xs mb-6">
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="text-white hover:text-grey-light">Terms</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="text-white hover:text-grey-light">Privacy</a>
                        </li>
                    </ul>
                </div>
                <div class="block sm:table-cell">
                    <p class="uppercase text-white text-sm sm:mb-6">Social</p>
                    <ul class="list-reset text-xs mb-6">
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="text-white hover:text-grey-light">Facebook</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="text-white hover:text-grey-light">Linkedin</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="text-white hover:text-grey-light">Twitter</a>
                        </li>
                    </ul>
                </div>
                <div class="block sm:table-cell">
                    <p class="uppercase text-white text-sm sm:mb-6">Company</p>
                    <ul class="list-reset text-xs mb-6">
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="text-white hover:text-grey-light">Official Blog</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="text-white hover:text-grey-light">About Us</a>
                        </li>
                        <li class="mt-2 inline-block mr-2 sm:block sm:mr-0">
                            <a href="#" class="text-white hover:text-grey-light">Contact</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

</body>
</html>
