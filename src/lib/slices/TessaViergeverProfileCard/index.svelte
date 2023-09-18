<script>
  /** @type {import("@prismicio/client").Content.TessaViergeverProfileCardSlice} */
  export let slice;
  console.log(slice)
</script>

<section data-slice-type={slice.slice_type} data-slice-variation={slice.variation}
>
<p>{slice.primary.name}</p>
<img src={slice.primary.profile_picture.url} alt="dkdkf" width="300" height="300">


</section>


