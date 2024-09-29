
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">
    <style>
        body {
          font-family: 'Poppins', sans-serif;
        }
      </style>  
</head>
<body class="">
    <div class="fixed top-0 left-0  h-screen  bg-neutral-700 text-white transition-width duration-300 ease-in-out w-60 " id="sidebar">
       
        <div class="flex items-center p-3  w-40">
            <div class="flex items-center p-3  ">
                <button id="btn">   <div class=""><i class="fa-solid fa-bars text-6 text-white  hover:text-black hover:bg-white p-3 rounded-full "></i></div> </button>
                
                <div class=" w-28  overflow-hidden ml-9 rounded-md  "><img id="logo_img" src="\icon\About.png" alt="Logo"></div>
                <!-- <p id="name" class="text-3xl font-serif text-white ml-2 transition duration-500 ease-in-o">Gradsy</p> -->
                
            </div>
            </div>
            <div> 
        <!-- <div class="flex flex-row items-center h-12">
            <div><button id="btn"><i class="fas fa-bars text-white cursor-pointer absolute top-5 left-1/2 transform -translate-x-1/2"></i></button></div>
            <div class="flex items-center">
                <img src="gcoen_logo.png" alt="Logo" class="w-8 h-8 rounded-full mr-3">
                <p class="text-lg">Gradsy</p>
            </div>
           
        </div> -->
        <div class="options">
            <ul class="mx-4">
                <li>
                   <div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white hover:text-gray-900">
                    <a href="home" >
                        <i class="fas fa-home mr-3"></i>
                        <span class="ml-3 itemm ">Home</span>
                    </a>
                    <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900  text-blue-500 py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Home</span>
               
                   </div> </li>
                   <li>
                    <div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white hover:text-gray-900">       <a href="home" >
                       <i class="far fa-folder mr-3"></i>
                       <span class="ml-3 itemm">Alumni </span>
                   </a>
                   <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Alumni Directory</span>
            </div>   </li>
                <li>
                   <div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white hover:text-gray-900"> <a href="home" >
                    <i class="fas fa-plus p-[2px] mr-3"></i>
                    <span class="ml-3 itemm">Explore</span>
                </a>
                <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Add Post</span>
           </div> </li>
                <li>
                  <div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white hover:text-gray-900">  <a href="home" >
                    <i class="far fa-message mr-3"></i>
                    <span class="ml-3 itemm">Campaigns</span>
                </a>
                <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Message</span>
          </div>  </li>
                <!-- <li>
                  <div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white hover:text-gray-900">  <a href="home" >
                    <i class="fas fa-video mr-3"></i>
                    <span class="ml-3 itemm">Job</span>
                </a>
                <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Quick Meet</span>
         </div>   </li> -->
                
                <li>
              <div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white hover:text-gray-900">
                <a href="home" >
                    <i class="fas fa-user-doctor mr-3"></i>
                    <span class="ml-3 itemm">Jobs</span>
                </a>
                <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Job Portal</span>
           
              </div> </li>
                <li>
                  <div class="flex items-center w-full py-5 px-3 rounded-md hover:bg-white hover:text-gray-900">
                    <a href="home" >
                        <i class="fas fa-trophy pl-[3px] mr-2"></i>
                        <span class="ml-3 itemm ">Notification</span>
                    </a>
                    <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Achievement</span>
               
                  </div> </li>
            </ul>
        </div>
    </div>
</div>


    <div class="feed ml-20">
       
    </div>

    <script>
      let button = document.querySelector('#btn');
let sidebar = document.querySelector('#sidebar');
let items = document.querySelectorAll('.itemm');
let tooltip = document.querySelector('.tooltip');
// let name = document.querySelector('#name');
let isCollapsed = false;

button.onclick = () => {
    isCollapsed = !isCollapsed;

    sidebar.classList.toggle('w-20');
    tooltip.classList.toggle('opacity-1');
    // if (name) {
    //     name.classList.toggle('text-black');
    // }

    if(isCollapsed==false) {
        setTimeout(() => {
            items.forEach((item) => {
        item.classList.toggle('hidden');
    });
        },200);
    }
    else{
        items.forEach((item) => {
        item.classList.toggle('hidden');
    });
    }
}

  //       let button = document.querySelector('#btn');
  //       let sidebar = document.querySelector('#sidebar');
  //       let item = document.querySelectorAll('.itemm');
  //       let tooltip = document.querySelector('.tooltip');
  //       let name = document.querySelector('#name');
  //       let clickCount=0;
  //       button.onclick = () => { clickCount++;
  // sidebar.classList.toggle('w-20');
  // tooltip.classList.toggle('opacity-1');
  // name.classList.toggle('text-black');

  // if (clickCount % 2 === 0) { // every second time
  //   setTimeout(function() {
  //     item.forEach((item) => {
  //       item.classList.remove('hidden'); 
  //     });
  //   }, 0); // 1 second delay
  // } else {
  //   // item.forEach((item) => {
  //   //   item.classList.add('hidden');
  //   // });
  //   setTimeout(function() {
  //     item.forEach((item) => {
  //       item.classList.add('hidden'); 
  //     });
  //   }, 0); // 1 second delay
  // }}
    </script>
</body>
</html>
