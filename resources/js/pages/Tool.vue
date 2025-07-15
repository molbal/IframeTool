<template>
  <div>
    <Head title="Grafana charts" />

      <iframe id="iframe"
        src="/graphs/index?embed=true"
        width="100%"
        height="1000"
        frameborder="0"></iframe>


  </div>
</template>

<script>
export default {
  mounted() {
    //
  },
}
function resizeIFrameToFitContent( iFrame ) {
    iFrame.height = iFrame.contentWindow.document.body.scrollHeight;
}

window.addEventListener('DOMContentLoaded', function(e) {
    var iFrame = document.getElementById( 'iframe' );
    resizeIFrameToFitContent( iFrame );
} );
</script>

<style>
/* Scoped Styles */
</style>
