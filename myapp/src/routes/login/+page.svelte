<!-- <script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script> -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gradsy Login</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css" />
  
  <!-- Import Poppins Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap" rel="stylesheet">
  
  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  
  <!-- Apply Poppins font in Tailwind -->
  <style>
    body {    
      font-family: 'Poppins', sans-serif;
    }
  </style>
</head>
<body class="bg-gray-100 flex items-center justify-center min-h-screen">

  <!-- Container -->
  <div class="min-w-96 max-w-102 bg-[#fffefe] h-auto px-auto rounded-lg p-8 md:w-102 text-sm">
    <!-- Logo -->
    <div class="flex justify-center mb-2">
      <img src="/icon/About.png" alt="Gradsy Logo" class="h-16">
    </div>

    <!-- Email and Password Form -->
    <form action="#" method="POST">
      <!-- Email -->
      <div class="mb-4">
        <label for="email" class="block text-gray-700">Email</label>
        <input type="email" id="email" name="email" placeholder="Enter Your Email" class="w-full p-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-400">
      </div>

      <!-- Password -->
      <div class="mb-4 relative ">
        <label for="password" class="block text-gray-700">Password</label>
        <input type="password" id="password" name="password" placeholder="Enter Your Password" class="w-full p-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-400">
		<span class="absolute right-3 top-8	 cursor-pointer " id="password-toggle">
			<i  class="fas fa-eye opacity-50  " id="password-eye"></i>
		  </span>
      </div>

      <!-- Forgot Password -->
      <div class="flex justify-between items-center mb-4 ">
        <a href="#" class="text-sm text-gray-600 hover:text-blue-500">Forgot Password?</a>
      </div>

      <!-- Sign In Button -->
      <button type="submit" class="w-full bg-[#49b6c5] text-white p-2 rounded-lg hover:bg-[#3aa7b2]">LOG IN</button>
    </form>

    <!-- Sign Up Link -->
    <p class="text-center text-gray-600 mt-4">Don't have an account? <a href="signup" class="text-blue-500 hover:underline">Sign Up</a></p>

    <!-- OR Sign In With -->
    <div class="flex items-center justify-between mt-6">
      <div class="border-t flex-grow mr-3"></div>
      <span class="text-gray-500">Or Sign In With</span>
      <div class="border-t flex-grow ml-3"></div>
    </div>

    <!-- Social Buttons -->
    <div class="flex justify-center mt-4 space-x-4">
      <a href="#" class="bg-white border p-2 rounded-lg hover:bg-gray-100 flex items-center">
        <img src="/icon/google.png" alt="Google" class="h-6 w-6">
      </a>
      <a href="#" class="bg-white border p-2 rounded-lg hover:bg-gray-100 flex items-center">
        <img src="/icon/github.png" alt="GitHub" class="h-6 w-6">
      </a>
      <a href="#" class="bg-white border p-2 rounded-lg hover:bg-gray-100 flex items-center">
        <img src="/icon/linkedin.png" alt="LinkedIn" class="h-6 w-6">
      </a>
    </div>
  </div>
<script>
	let passwordInput = document.getElementById('password');
let passwordToggle = document.getElementById('password-toggle');
let passwordEye = document.getElementById('password-eye');

passwordToggle.addEventListener('click', () => {
  if (passwordInput.type === 'password') {
    passwordInput.type = 'text';
    passwordEye.classList.add('fa-eye-slash');
  } else {
    passwordInput.type = 'password';
    passwordEye.classList.remove('fa-eye-slash');
  }
});
</script>
</body>
</html>
