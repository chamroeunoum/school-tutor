<template >
    <div class="w-full h-12 leading-10 font-muol text-lg border-b border-gray-200" >សង្ខេបព័ត៌មាន</div>
    <div class="flex flex-wrap justify-center p-8">
        <!-- <div @click="$router.push('/orgchart')" class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class=" m-auto mb-4 h-12" >
                <ParentChild />
            </Icon>
            <div class="m-auto mb-2 ">តារាងរចនាសម្ព័ន្ធ</div>
            <div class="m-auto mb-2 font-bold text-lg text-blue-600 " ></div>
        </div> -->
        <!-- <div @click="$router.push('/regulator')" class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class="text-red-700 m-auto mb-4 h-12" >
                <DocumentPdf24Regular />
            </Icon>
            <div class="m-auto mb-2 ">ឯកសារគតិយុត្ត</div>
            <div class="m-auto mb-2 font-bold text-lg text-blue-600 " v-html="totalRegulators" ></div>
        </div> -->
        <div @click="$router.push('/user')" class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class=" m-auto mb-4 h-12" >
                <PersonCircleOutline />
            </Icon>
            <div class="m-auto mb-2 text-lg">គណនី</div>
            <div class="m-auto mb-2 font-bold text-lg " v-html="totalAccounts" ></div>
        </div>
        <div @click="$router.push('/store')" class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class=" m-auto mb-4 h-12 " >
                <StorefrontOutline />
            </Icon>
            <div class="m-auto mb-2 text-lg">ហាង</div>
            <div class="m-auto mb-2 font-bold text-lg  " v-html="totalStores" ></div>
        </div>
        <div @click="$router.push('/client')" class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class=" m-auto mb-4 h-12 " >
                <UserMultiple />
            </Icon>
            <div class="m-auto mb-2 text-lg">អតិថិជន</div>
            <div class="m-auto mb-2 font-bold text-lg  " v-html="totalClients" ></div>
        </div>
        <div @click="$router.push('/loan')" class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class=" m-auto mb-4 h-12 " >
                <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 20 20"><g fill="none"><path d="M4.5 2A1.5 1.5 0 0 0 3 3.5v13A1.5 1.5 0 0 0 4.5 18h7a1.5 1.5 0 0 0 1.5-1.5V15a.5.5 0 0 0-.5-.5c-.413 0-.677-.102-.856-.236c-.183-.137-.322-.342-.424-.623c-.214-.588-.22-1.367-.22-2.141a.5.5 0 0 0-.147-.354l-.286-.287l-1.213-1.213c-.467-.467-.604-.78-.63-.955c-.02-.14.022-.234.122-.33c.214-.205.367-.344.54-.386c.103-.026.338-.044.76.378l3 3a.5.5 0 0 0 .708-.707L13 9.793V6.707l2.56 2.56a1.5 1.5 0 0 1 .44 1.061V17.5a.5.5 0 0 0 1 0v-7.172a2.5 2.5 0 0 0-.732-1.767L13 5.293V3.5A1.5 1.5 0 0 0 11.5 2h-7zM12 5.5v3.293l-1.146-1.147c-.579-.578-1.154-.777-1.705-.643a1.517 1.517 0 0 0-.313.115A3.001 3.001 0 0 0 5 10a3 3 0 0 0 5.007 2.23c.017.578.075 1.21.273 1.753c.148.407.384.796.764 1.08l.006.006A1.5 1.5 0 0 0 10 16.5v.5H6v-.5A1.5 1.5 0 0 0 4.5 15H4V5h.5A1.5 1.5 0 0 0 6 3.5V3h4v.5A1.5 1.5 0 0 0 11.5 5h.5v.5zm0 11v.009a.5.5 0 0 1-.5.491H11v-.5a.5.5 0 0 1 .5-.5h.5v.5zM6 10a2 2 0 0 1 1.874-1.996c-.124.23-.187.51-.139.833c.071.482.378.983.911 1.516l.907.907A2 2 0 0 1 6 10zM5 3v.5a.5.5 0 0 1-.5.5H4v-.5a.5.5 0 0 1 .5-.5H5zM4 16h.5a.5.5 0 0 1 .5.5v.5h-.5a.5.5 0 0 1-.5-.5V16zm8-12h-.5a.5.5 0 0 1-.5-.5V3h.5a.5.5 0 0 1 .5.5V4z" fill="currentColor"></path></g></svg>
            </Icon>
            <div class="m-auto mb-2 text-lg">កម្ចី</div>
            <div class="m-auto mb-2 font-bold text-lg  " v-html="totalLoans" ></div>
        </div>
        <div @click="$router.push('/product')" class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class=" m-auto mb-4 h-12 " >
                <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 24 24"><g fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M10 16V8h2.5a2.5 2.5 0 1 1 0 5H10"></path><circle cx="12" cy="12" r="9"></circle></g></svg>
            </Icon>
            <div class="m-auto mb-2 text-lg">ផលិតផល</div>
            <div class="m-auto mb-2 font-bold text-lg  " v-html="totalProducts" ></div>
        </div>
        <div @click="$router.push('/stock')" class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class=" m-auto mb-4 h-12 " >
                <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 24 24"><g fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 21V8l9-4l9 4v13"></path><path d="M13 13h4v8H7v-6h6"></path><path d="M13 21v-9a1 1 0 0 0-1-1h-2a1 1 0 0 0-1 1v3"></path></g></svg>
            </Icon>
            <div class="m-auto mb-2 text-lg">ឃ្លាំង</div>
            <div class="m-auto mb-2 font-bold text-lg  " v-html="totalProducts" ></div>
        </div>
        <div class=" my-8 border-b border-gray-300 bg-gray-100 w-full p-2 rounded-full font-muol" >ព័ត៌មានកម្ចី</div>
        <!-- Total loans principle -->
        <div class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class=" m-auto mb-4 h-12 " >
                <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 20 20"><g fill="none"><path d="M4.5 2A1.5 1.5 0 0 0 3 3.5v13A1.5 1.5 0 0 0 4.5 18h7a1.5 1.5 0 0 0 1.5-1.5V15a.5.5 0 0 0-.5-.5c-.413 0-.677-.102-.856-.236c-.183-.137-.322-.342-.424-.623c-.214-.588-.22-1.367-.22-2.141a.5.5 0 0 0-.147-.354l-.286-.287l-1.213-1.213c-.467-.467-.604-.78-.63-.955c-.02-.14.022-.234.122-.33c.214-.205.367-.344.54-.386c.103-.026.338-.044.76.378l3 3a.5.5 0 0 0 .708-.707L13 9.793V6.707l2.56 2.56a1.5 1.5 0 0 1 .44 1.061V17.5a.5.5 0 0 0 1 0v-7.172a2.5 2.5 0 0 0-.732-1.767L13 5.293V3.5A1.5 1.5 0 0 0 11.5 2h-7zM12 5.5v3.293l-1.146-1.147c-.579-.578-1.154-.777-1.705-.643a1.517 1.517 0 0 0-.313.115A3.001 3.001 0 0 0 5 10a3 3 0 0 0 5.007 2.23c.017.578.075 1.21.273 1.753c.148.407.384.796.764 1.08l.006.006A1.5 1.5 0 0 0 10 16.5v.5H6v-.5A1.5 1.5 0 0 0 4.5 15H4V5h.5A1.5 1.5 0 0 0 6 3.5V3h4v.5A1.5 1.5 0 0 0 11.5 5h.5v.5zm0 11v.009a.5.5 0 0 1-.5.491H11v-.5a.5.5 0 0 1 .5-.5h.5v.5zM6 10a2 2 0 0 1 1.874-1.996c-.124.23-.187.51-.139.833c.071.482.378.983.911 1.516l.907.907A2 2 0 0 1 6 10zM5 3v.5a.5.5 0 0 1-.5.5H4v-.5a.5.5 0 0 1 .5-.5H5zM4 16h.5a.5.5 0 0 1 .5.5v.5h-.5a.5.5 0 0 1-.5-.5V16zm8-12h-.5a.5.5 0 0 1-.5-.5V3h.5a.5.5 0 0 1 .5.5V4z" fill="currentColor"></path></g></svg>
            </Icon>
            <div class="m-auto mb-2 text-lg">សរុបប្រាក់កម្ចី</div>
            <div class="m-auto mb-2 font-bold text-lg text-blue-600 " v-html="totalBalances.toFixed(2) + ' $'" ></div>
        </div>
        <!-- Total loans payback -->
        <div class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class=" m-auto mb-4 h-12 " >
                <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 20 20"><g fill="none"><path d="M4.5 2A1.5 1.5 0 0 0 3 3.5v13A1.5 1.5 0 0 0 4.5 18h7a1.5 1.5 0 0 0 1.5-1.5V15a.5.5 0 0 0-.5-.5c-.413 0-.677-.102-.856-.236c-.183-.137-.322-.342-.424-.623c-.214-.588-.22-1.367-.22-2.141a.5.5 0 0 0-.147-.354l-.286-.287l-1.213-1.213c-.467-.467-.604-.78-.63-.955c-.02-.14.022-.234.122-.33c.214-.205.367-.344.54-.386c.103-.026.338-.044.76.378l3 3a.5.5 0 0 0 .708-.707L13 9.793V6.707l2.56 2.56a1.5 1.5 0 0 1 .44 1.061V17.5a.5.5 0 0 0 1 0v-7.172a2.5 2.5 0 0 0-.732-1.767L13 5.293V3.5A1.5 1.5 0 0 0 11.5 2h-7zM12 5.5v3.293l-1.146-1.147c-.579-.578-1.154-.777-1.705-.643a1.517 1.517 0 0 0-.313.115A3.001 3.001 0 0 0 5 10a3 3 0 0 0 5.007 2.23c.017.578.075 1.21.273 1.753c.148.407.384.796.764 1.08l.006.006A1.5 1.5 0 0 0 10 16.5v.5H6v-.5A1.5 1.5 0 0 0 4.5 15H4V5h.5A1.5 1.5 0 0 0 6 3.5V3h4v.5A1.5 1.5 0 0 0 11.5 5h.5v.5zm0 11v.009a.5.5 0 0 1-.5.491H11v-.5a.5.5 0 0 1 .5-.5h.5v.5zM6 10a2 2 0 0 1 1.874-1.996c-.124.23-.187.51-.139.833c.071.482.378.983.911 1.516l.907.907A2 2 0 0 1 6 10zM5 3v.5a.5.5 0 0 1-.5.5H4v-.5a.5.5 0 0 1 .5-.5H5zM4 16h.5a.5.5 0 0 1 .5.5v.5h-.5a.5.5 0 0 1-.5-.5V16zm8-12h-.5a.5.5 0 0 1-.5-.5V3h.5a.5.5 0 0 1 .5.5V4z" fill="currentColor"></path></g></svg>
            </Icon>
            <div class="m-auto mb-2 text-lg">សរុបប្រាក់ដើមបានបង់</div>
            <div class="m-auto mb-2 font-bold text-lg text-yellow-600 " v-html="totalPrinciples.toFixed(2) + ' $'" ></div>
        </div>
        <!-- Total loans balance : ( principle - repayback ) -->
        <div class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class=" m-auto mb-4 h-12 " >
                <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 20 20"><g fill="none"><path d="M4.5 2A1.5 1.5 0 0 0 3 3.5v13A1.5 1.5 0 0 0 4.5 18h7a1.5 1.5 0 0 0 1.5-1.5V15a.5.5 0 0 0-.5-.5c-.413 0-.677-.102-.856-.236c-.183-.137-.322-.342-.424-.623c-.214-.588-.22-1.367-.22-2.141a.5.5 0 0 0-.147-.354l-.286-.287l-1.213-1.213c-.467-.467-.604-.78-.63-.955c-.02-.14.022-.234.122-.33c.214-.205.367-.344.54-.386c.103-.026.338-.044.76.378l3 3a.5.5 0 0 0 .708-.707L13 9.793V6.707l2.56 2.56a1.5 1.5 0 0 1 .44 1.061V17.5a.5.5 0 0 0 1 0v-7.172a2.5 2.5 0 0 0-.732-1.767L13 5.293V3.5A1.5 1.5 0 0 0 11.5 2h-7zM12 5.5v3.293l-1.146-1.147c-.579-.578-1.154-.777-1.705-.643a1.517 1.517 0 0 0-.313.115A3.001 3.001 0 0 0 5 10a3 3 0 0 0 5.007 2.23c.017.578.075 1.21.273 1.753c.148.407.384.796.764 1.08l.006.006A1.5 1.5 0 0 0 10 16.5v.5H6v-.5A1.5 1.5 0 0 0 4.5 15H4V5h.5A1.5 1.5 0 0 0 6 3.5V3h4v.5A1.5 1.5 0 0 0 11.5 5h.5v.5zm0 11v.009a.5.5 0 0 1-.5.491H11v-.5a.5.5 0 0 1 .5-.5h.5v.5zM6 10a2 2 0 0 1 1.874-1.996c-.124.23-.187.51-.139.833c.071.482.378.983.911 1.516l.907.907A2 2 0 0 1 6 10zM5 3v.5a.5.5 0 0 1-.5.5H4v-.5a.5.5 0 0 1 .5-.5H5zM4 16h.5a.5.5 0 0 1 .5.5v.5h-.5a.5.5 0 0 1-.5-.5V16zm8-12h-.5a.5.5 0 0 1-.5-.5V3h.5a.5.5 0 0 1 .5.5V4z" fill="currentColor"></path></g></svg>
            </Icon>
            <div class="m-auto mb-2 text-lg">សរុបប្រាក់ដើមនៅសល់</div>
            <div class="m-auto mb-2 font-bold text-lg text-blue-600 " v-html="(totalBalances - totalPrinciples ).toFixed(2) + ' $'" ></div>
        </div>
        <!-- Total loans interest -->
        <div class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class=" m-auto mb-4 h-12 " >
                <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 20 20"><g fill="none"><path d="M4.5 2A1.5 1.5 0 0 0 3 3.5v13A1.5 1.5 0 0 0 4.5 18h7a1.5 1.5 0 0 0 1.5-1.5V15a.5.5 0 0 0-.5-.5c-.413 0-.677-.102-.856-.236c-.183-.137-.322-.342-.424-.623c-.214-.588-.22-1.367-.22-2.141a.5.5 0 0 0-.147-.354l-.286-.287l-1.213-1.213c-.467-.467-.604-.78-.63-.955c-.02-.14.022-.234.122-.33c.214-.205.367-.344.54-.386c.103-.026.338-.044.76.378l3 3a.5.5 0 0 0 .708-.707L13 9.793V6.707l2.56 2.56a1.5 1.5 0 0 1 .44 1.061V17.5a.5.5 0 0 0 1 0v-7.172a2.5 2.5 0 0 0-.732-1.767L13 5.293V3.5A1.5 1.5 0 0 0 11.5 2h-7zM12 5.5v3.293l-1.146-1.147c-.579-.578-1.154-.777-1.705-.643a1.517 1.517 0 0 0-.313.115A3.001 3.001 0 0 0 5 10a3 3 0 0 0 5.007 2.23c.017.578.075 1.21.273 1.753c.148.407.384.796.764 1.08l.006.006A1.5 1.5 0 0 0 10 16.5v.5H6v-.5A1.5 1.5 0 0 0 4.5 15H4V5h.5A1.5 1.5 0 0 0 6 3.5V3h4v.5A1.5 1.5 0 0 0 11.5 5h.5v.5zm0 11v.009a.5.5 0 0 1-.5.491H11v-.5a.5.5 0 0 1 .5-.5h.5v.5zM6 10a2 2 0 0 1 1.874-1.996c-.124.23-.187.51-.139.833c.071.482.378.983.911 1.516l.907.907A2 2 0 0 1 6 10zM5 3v.5a.5.5 0 0 1-.5.5H4v-.5a.5.5 0 0 1 .5-.5H5zM4 16h.5a.5.5 0 0 1 .5.5v.5h-.5a.5.5 0 0 1-.5-.5V16zm8-12h-.5a.5.5 0 0 1-.5-.5V3h.5a.5.5 0 0 1 .5.5V4z" fill="currentColor"></path></g></svg>
            </Icon>
            <div class="m-auto mb-2 text-lg">សរុបប្រាក់ការបានបង់</div>
            <div class="m-auto mb-2 font-bold text-lg text-green-600 " v-html="totalInterests.toFixed(2) + ' $'" ></div>
        </div>
        <!-- Total loans interest owned -->
        <div class="bg-gray-200 rounded border border-gray-100 hover:border-gray-200 hover:bg-gray-100 duration-300 p-8 m-8 cursor-pointer min-w-200">
            <Icon size="60" class=" m-auto mb-4 h-12 " >
                <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 20 20"><g fill="none"><path d="M4.5 2A1.5 1.5 0 0 0 3 3.5v13A1.5 1.5 0 0 0 4.5 18h7a1.5 1.5 0 0 0 1.5-1.5V15a.5.5 0 0 0-.5-.5c-.413 0-.677-.102-.856-.236c-.183-.137-.322-.342-.424-.623c-.214-.588-.22-1.367-.22-2.141a.5.5 0 0 0-.147-.354l-.286-.287l-1.213-1.213c-.467-.467-.604-.78-.63-.955c-.02-.14.022-.234.122-.33c.214-.205.367-.344.54-.386c.103-.026.338-.044.76.378l3 3a.5.5 0 0 0 .708-.707L13 9.793V6.707l2.56 2.56a1.5 1.5 0 0 1 .44 1.061V17.5a.5.5 0 0 0 1 0v-7.172a2.5 2.5 0 0 0-.732-1.767L13 5.293V3.5A1.5 1.5 0 0 0 11.5 2h-7zM12 5.5v3.293l-1.146-1.147c-.579-.578-1.154-.777-1.705-.643a1.517 1.517 0 0 0-.313.115A3.001 3.001 0 0 0 5 10a3 3 0 0 0 5.007 2.23c.017.578.075 1.21.273 1.753c.148.407.384.796.764 1.08l.006.006A1.5 1.5 0 0 0 10 16.5v.5H6v-.5A1.5 1.5 0 0 0 4.5 15H4V5h.5A1.5 1.5 0 0 0 6 3.5V3h4v.5A1.5 1.5 0 0 0 11.5 5h.5v.5zm0 11v.009a.5.5 0 0 1-.5.491H11v-.5a.5.5 0 0 1 .5-.5h.5v.5zM6 10a2 2 0 0 1 1.874-1.996c-.124.23-.187.51-.139.833c.071.482.378.983.911 1.516l.907.907A2 2 0 0 1 6 10zM5 3v.5a.5.5 0 0 1-.5.5H4v-.5a.5.5 0 0 1 .5-.5H5zM4 16h.5a.5.5 0 0 1 .5.5v.5h-.5a.5.5 0 0 1-.5-.5V16zm8-12h-.5a.5.5 0 0 1-.5-.5V3h.5a.5.5 0 0 1 .5.5V4z" fill="currentColor"></path></g></svg>
            </Icon>
            <div class="m-auto mb-2 text-lg">សរុបប្រាក់ការ ជំពាក់</div>
            <div class="m-auto mb-2 font-bold text-lg text-red-600 " v-html="totalOwnedInterests.toFixed(2) + ' $'" ></div>
        </div>
        
    </div>
</template>
<script >
import { Icon } from '@vicons/utils'
import { useDialog, useMessage, useNotification } from 'naive-ui'
import { DocumentPdf24Regular } from '@vicons/fluent'
import { PersonCircleOutline, StorefrontOutline } from '@vicons/ionicons5'
import { UserMultiple, ParentChild } from '@vicons/carbon'
import { ref , reactive, computed } from 'vue'
import { useStore } from 'vuex'
import { useRouter } from 'vue-router'


export default {
    name: 'Dashboard',
    components: {
        Icon ,
        /**
         * fluent
         */
        DocumentPdf24Regular ,
        PersonCircleOutline ,
        ParentChild ,
        UserMultiple ,
        StorefrontOutline
    },
    name: 'dashboard' ,
    setup() {
        const router = useRouter()
        const store = useStore()
        const dialog = useDialog()
        const message = useMessage()
        const notify = useNotification()

        

        /**
         * Total balances
         */
        const totalBalances = ref(0)
        const totalPrinciples = ref(0)
        const totalInterests = ref(0)
        const totalOwnedInterests = ref(0)
        function getBPIW(){
            store.dispatch('loan/totalBPIW',{}).then( res => {
                if( res.data.ok ){
                    totalBalances.value = parseFloat( res.data.balance > 0 ? res.data.balance : 0 )
                    totalPrinciples.value = parseFloat( res.data.principle > 0 ? res.data.principle : 0 )
                    totalInterests.value = parseFloat( res.data.interest > 0 ? res.data.interest : 0 )
                    totalOwnedInterests.value = parseFloat( res.data.owned_interest > 0 ? res.data.owned_interest : 0 )
                }else{
                    totalBalances.value = 0
                    totalPrinciples.value = 0
                    totalInterests.value = 0
                    totalOwnedInterests.value = 0
                }
            }).catch( err => {
                console.log( err )
            })
        }

        /**
         * Account
         */
        const accountResponse = ref(null)
        const totalAccounts = computed(() => {
            return accountResponse.value !== null ? accountResponse.value.pagination.totalRecords : 0 
        })
        function getAccounts(){
            store.dispatch('user/list',{
                search: '' ,
                perPage: 10 ,
                page: 1
            }).then( res => {
                if( res.data.ok ){
                    accountResponse.value = res.data
                }else{
                    accountResponse.value = null
                }
            }).catch( err => {
                console.log( err )
                notify.error({
                    title: "អានបញ្ជីគណនី" ,
                    content: "មានបញ្ហាពេលអានបញ្ជីគណនី។" ,
                    duration: 3000 ,
                    background: true
                })
            })
        }

        /**
         * Clients
         */
        const clientResponse = ref(null)
        const totalClients = computed(() => {
            return clientResponse.value !== null ? clientResponse.value.records.length : 0 
        })
        function getClients(){
            store.dispatch('client/compact',{
                search: '' ,
                perPage: 10 ,
                page: 1
            }).then( res => {
                if( res.data.ok ){
                    clientResponse.value = res.data
                }else{
                    clientResponse.value = null
                }
            }).catch( err => {
                console.log( err )
                notify.error({
                    title: "អានអតិថិជន" ,
                    content: "មានបញ្ហាពេលអានអតិថិជន។" ,
                    duration: 3000 ,
                    background: true
                })
            })
        }

        /**
         * Loans
         */
        const loanResponse = ref(null)
        const totalLoans = computed(() => {
            return loanResponse.value !== null ? loanResponse.value.pagination.totalRecords : 0 
        })
        function getLoans(){
            store.dispatch('loan/list',{
                search: '' ,
                perPage: 10 ,
                page: 1
            }).then( res => {
                if( res.data.ok ){
                    loanResponse.value = res.data
                }else{
                    loanResponse.value = null
                }
            }).catch( err => {
                console.log( err )
                notify.error({
                    title: "អានកម្ចី" ,
                    content: "មានបញ្ហាពេលអានកម្ចី។" ,
                    duration: 3000 ,
                    background: true
                })
            })
        }

        /**
         * Products
         */
        const productResponse = ref(null)
        const totalProducts = computed(() => {
            return productResponse.value !== null ? productResponse.value.pagination.totalRecords : 0 
        })
        function getProducts(){
            store.dispatch('product/list',{
                search: '' ,
                perPage: 10 ,
                page: 1
            }).then( res => {
                if( res.data.ok ){
                    productResponse.value = res.data
                }else{
                    productResponse.value = null
                }
            }).catch( err => {
                console.log( err )
                notify.error({
                    title: "អានផលិតផល" ,
                    content: "មានបញ្ហាពេលអានផលិតផល។" ,
                    duration: 3000 ,
                    background: true
                })
            })
        }

        /**
         * Products
         */
         const storeResponse = ref(null)
        const totalStores = computed(() => {
            return storeResponse.value !== null ? storeResponse.value.pagination.totalRecords : 0 
        })
        function getStores(){
            store.dispatch('store/list',{
                search: '' ,
                perPage: 10 ,
                page: 1
            }).then( res => {
                if( res.data.ok ){
                    storeResponse.value = res.data
                }else{
                    storeResponse.value = null
                }
            }).catch( err => {
                console.log( err )
                notify.error({
                    title: "អានផលិតផល" ,
                    content: "មានបញ្ហាពេលអានផលិតផល។" ,
                    duration: 3000 ,
                    background: true
                })
            })
        }

        /**
         * Initial
         */
        getBPIW()
        getLoans()
        getClients()
        getAccounts()
        getStores()
        getProducts()

        return {
            totalBalances,
            totalPrinciples,
            totalInterests,
            totalOwnedInterests,
            totalLoans ,
            totalClients ,
            totalAccounts ,
            totalProducts ,
            totalStores
        }
    }
}
</script>
<style scoped>
    
</style>