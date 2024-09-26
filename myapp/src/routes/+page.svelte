<!-- <script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script> -->
<!-- main page -->
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

<a href="home"><button class="bg-gray-200">(only for running)click me to navigate to home page for now</button></a>
<a href="land_page"><button class="bg-gray-200">(only for running)click me to navigate to landing page for now</button></a>
    <!-- Sign Up Link -->
    <p class="text-center text-gray-600 mt-4">Already have an account? <a href="signup" class="text-blue-500 hover:underline">Sign Up</a></p>


</body>
</html>
