<script>
    let Youtube = "";
    let IsActive = false;
    let Output = "";
    let getTheExt = async (B) => {
        let b = B.split('/watch?v=');
        Output = "https://www.youtube-nocookie.com/embed/"+b[1]
        
    }

    

</script>



  
    <div class=" absolute bg-gradient-to-t from-red-600 to-indigo-700 w-screen h-screen">
      <iframe class=" my-3 w-11/12 h-96 justify-center mx-auto bg-blue-800 shadow-2xl" title="Lmaooo" src="{Output}"></iframe>
      <div class="mx-auto text-center "><input bind:value={Youtube}  class="w-3/4 p-1 rounded my-2 focus:outline-none shadow  bg-clip-text text-transparent bg-gradient-to-br font-bold ring-black ring-1 from-black to-indigo-800 " placeholder="Pon tu URL Aqui." type="text" /></div>
      <div class="mx-auto text-center bg-black cursor-pointer w-max px-2 py-1 rounded-sm text-white" on:click="{getTheExt(Youtube)}">Desbloquear</div>
    </div>
  

  

