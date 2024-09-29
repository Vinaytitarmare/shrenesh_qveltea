<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css"
    />
    <style>
      body {
        font-family: 'Poppins', sans-serif;
      }
    </style>
  </head>
  <body class=" bg-[url('icon/opacity_graduate.png')] bg-no-repeat bg-cover ">
    <!-- w-[full] h-[100vh] -->
    <div
      class="h-14  flex flex-row justify-between mt-0 pt-2 pl-2 fixed top-0 left-0 w-full z-10  bg-[#f6fbfe] shadow-b-md"
    >
      <img src="icon/About.png" alt="" class="mt-1" />
      <div class="flex flex-row justify-around space-x-6 items-center">
        <div><a href="home">Home</a></div>
        <div><a href="download">Download</a></div>
        <div><a href="">Support</a></div>
        <div><a href="">Jobs</a></div>
        <div><a href="">Campaigns</a></div>
        <div>
          <button class="bg-[#49b6c5] text-white rounded-2xl mr-3 px-4 py-1"
            ><a href="login">Login</a></button
          >
        </div>
      </div>
    </div>
    <!-- main downloading part here boyy -->
    <div class="flex flex-col mt-[12vh] justify-around">
      <div class="flex flex-wrap items-center justify-around mx-auto">
        <img src="icon/About.png" alt="" />
        <div class="text-2xl font-bold mb-4">
          <pre><b class="">     For a more seamless experience,</b></pre>
          <pre><b>  Download Gradsy on your device now !</b></pre>
        </div>
      </div>

      <!-- <div class="flex    "> -->
        <div class="flex flex-wrap justify-center gap-10 ">
          <div class="flex flex-col w-[20rem] h-[22rem] gap-6 justify-center items-center text-2xl font-bold rounded-2xl bg-gray-200"  style="box-shadow: 10px 10px 20px gray;">
            <div><img src="icon/window.png" class="h-[9rem]  rounded-lg mx-auto" alt="" /></div>
            <div><p >Download for Windows</p></div>
            <div>
              <button  
                class="px-8 py-2 rounded-2xl border-2  bg-[#49b6c5] text-white"
                >Download</button
              >
            </div>
          </div>
          <div style="box-shadow: 10px 10px 20px gray;" class="flex flex-col w-[20rem] h-[22rem] gap-6 justify-center items-center text-white text-2xl font-bold rounded-2xl bg-[#2E2E30]">
            <div><img src="icon/playstore.png" class=" h-[9rem] mx-auto" alt="" /></div>
            <div><p>Download for Android</p></div>
            <div>
              <button
                class="px-8 py-2 rounded-2xl border-2 text-[#49b6c5] bg-white"
                >Download</button
              >
            </div>
          </div>
          <div style="box-shadow: 10px 10px 20px gray;" class="flex flex-col w-[20rem] h-[22rem] gap-6 justify-center items-center rounded-2xl text-2xl font-bold bg-gray-200">
            <div><img src="icon/apple.png" alt="" class="h-[9rem] mx-auto" /></div>
            <div><p>Download for IOS</p></div>
            <div>
              <button
                class="px-8 py-2 rounded-2xl border-2 bg-[#49b6c5] text-white"
                >Download</button
              >
            </div>
          </div>
        </div>
      </div>
      <img src="icon/msg.png" class="fixed bottom-0 right-2" alt="" />
      <script>
      </script>
  </body
  >
</html>
