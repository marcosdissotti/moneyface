<script setup lang="ts">
    import { ref } from "vue"
;    import fs from "fs";
    import pdfText from "pdf-text";
    const pdf = "/home/dissotti/workspace/ReleasedeResultados4T23.pdf";

    const chunksTest = ref(); 
    console.log(pdf)
    var buffer = fs.readFileSync(pdf)
    pdfText(buffer, function(err, chunks) {
      chunksTest.value = chunks;
    })
</script>

<template>
  {{ chunksTest }}
</template>
