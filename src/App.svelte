<script lang="ts">
  const infohref = () => {
    window.location.href = "https://thepuppet57.alwaysdata.net/info.php"
  }

  function tpsreal() {
    window.location.href = "https://thepuppet57.alwaysdata.net/tps"
  }
</script>

<main>
  <div id="some-bad-id-cuz-idk-what-to-name-these">
    <h1 class="bigboytext">Hey there! I'm puppet!</h1>
    <div class="button-container">
      <button class="booton" on:click={infohref}>Info</button>
      <button class="booton" on:click={tpsreal}>The puppet studios</button>
    </div>
  </div>
</main>

<style lang="scss">
  $purple: #370664;
  $purpletext: #420068;
  $lightgray: #b6b6b6;

  :global(body), :global(html) {
    overflow: hidden;
    height: 100%;
    margin: 0;
  }

  #some-bad-id-cuz-idk-what-to-name-these {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }

  .bigboytext {
    color: $purpletext;
    margin-bottom: 5px;
  }

  .button-container {
    display: flex;
    flex-direction: row;
    gap: 10px; /* Adds space between buttons */
  }

  .booton {
    color: $lightgray;
    background-color: $purple;
    width: 90px;
    height: 40px;
    border: none;
    border-radius: 10px;
    transition: 0.3s;
  }

  .booton:hover {
    transform: scale(1.1);
    background-color: darken($purple, 3%);
  }
</style>
