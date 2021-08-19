<template>

<div class="button_cont" align="center">

<a class="example_f" href="add-website-here" target="_blank" rel="nofollow">
<span>Pesan Sekarang</a>
</div>
	
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {
	props: ['showTitle']
}
</script>

<style lang="scss">
example_f {
   border-radius: 4px;
   background: linear-gradient(to right, #67b26b, #4ca2cb);
   border: none;
   color: #09eb2e;
   text-align: center;
   text-transform: uppercase;
   font-size: 22px;
   padding: 20px;
   width: 200px;
   transition: all 0.4s;
   cursor: pointer;
   margin: 5px;
 }
 .example_f span {
   cursor: pointer;
   display: inline-block;
   position: relative;
   transition: 0.4s;
 }
 .example_f span:after {
   content: '\00bb';
   position: absolute;
   opacity: 0;
   top: 0;
   right: -20px;
   transition: 0.5s;
 }
 .example_f:hover span {
   padding-right: 25px;
 }
 .example_f:hover span:after {
   opacity: 1;
   right: 0;
 }
</style>
