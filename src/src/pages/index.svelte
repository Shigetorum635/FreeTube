<script>
    let Youtube = "";
    let IsActive = false;
    let Output = "";
    let getTheExt = async (B) => {
        let b = B.split('/watch?v=');
        Output = "https://www.youtube-nocookie.com/embed/"+b[1]
        
    }

    

</script>
<link href="https://unpkg.com/tailwindcss@^2/dist/tailwind.min.css" rel="stylesheet">


<div class="bg-blue-800 w-screen h-screen">
    <div class="text-black font-bold text-center text-5xl shadow-lg bg-blue-400 p-5">Youtube Sin Restricciones.</div>
    <div class="text-black font-bold text-center text-2xl shadow-lg bg-blue-400 "> Sin Historial</div>
    <div class="text-black font-bold text-center text-2xl shadow-lg bg-blue-400 "> Sin Cookies</div>


    <input bind:value={Youtube} class="bg-gray-300 p-3 mx-auto w-screen text-center font-bold" placeholder="Entra tu URL Aqui" />
    <button class="bg-red-600 text-white p-5 w-screen transition-all duration-700 hover:bg-yellow-500" on:click="{getTheExt(Youtube)}">DESBLOQUEAR</button>
    <iframe class="w-144 h-72 justify-center mx-auto bg-blue-800 shadow-2xl" title="Lmaooo" width="600" height="300" src={Output }></iframe>
  </div>
  

