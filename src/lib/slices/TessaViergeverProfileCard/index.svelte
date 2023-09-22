<script>
  /** @type {import("@prismicio/client").Content.TessaViergeverProfileCardSlice} */
  export let slice;
  console.log(slice)
</script>

<body>
  <main>
    <section data-slice-type={slice.slice_type} data-slice-variation={slice.variation}>
      <p>{slice.primary.name}</p>
    
      <img src={slice.primary.profile_picture.url} alt="placeholder" width="250" height="auto">
  
      <p>{slice.primary.hobbies[0].text}</p>
      <p>{slice.primary.age}</p>
      <a href="{slice.primary.instagram.url}">Instagram</a>
      <a href="{slice.primary.linkedin.url}">LinkedIn</a>
      <a href="{slice.primary.github}">Github</a>
    </section>
  </main>
</body>

<style>

  * {
    margin: 0;
    box-sizing: border-box;
    font-family: 'Source Sans Pro', sans-serif;
  }

  /*  🥕 ROOT */
  :root {

    /* custom properties : colors */    
    --color-primary: rgba(248, 247, 255, 1);         /*  */  
    --color-secundary: rgba(255, 238, 221, 1);       /* coral*/  
    --color-tertiary: rgba(255, 216, 190, 1);        /* coral*/ 
    --color-highlights: rgba(184, 184, 255, 1);       /* lila */ 

     /* custom properties : text */ 
    --color-text: rgba(147, 129, 255, 1);             /* paars*/ 



  }

  body {
    background-color: rgba(240, 230, 140, 0.455);
    display: flex;
    justify-content: space-around;
  }

  section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    background-color: khaki;
    margin-top: 4rem;
    box-shadow: 0 0 50px rgba(30, 50, 49, 1)
    
  }

  img {
    border-radius: 5px;
    border: 5px solid rgb(194, 143, 139);
    box-shadow: 0 0 20px rgba(76, 76, 76, 0.221);
    padding: 1rem;
    margin: 1rem;
  }
  
</style>

