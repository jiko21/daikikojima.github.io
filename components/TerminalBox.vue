<template>
  <div class="terminal-box">
    <div class="app-bar">
      <div class="bar-button red-circle"/>
      <div class="bar-button yellow-circle"/>
      <div class="bar-button green-circle"/>
    </div>
    <div class="content">
      <slot/>
    </div>
  </div>
</template>

<script>
  export default {
    name: "TerminalBox"
  }
</script>

<style lang="scss" scoped>
  $width: 90%;
  .terminal-box {
    margin: 5% 0;
  }
  .app-bar {
    width: $width;
    box-sizing: border-box;

    display: table;
    height: 25px;
    background-color: #bbb;
    margin: 0 auto;
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
    .bar-button {
      height: 10px;
      width: 10px;
      float: left;
      margin: 5px 3px;
      vertical-align: middle;
      border-radius: 50%;
      border: 1px solid #000;
      background-color: #ff3b47;
      border-color: #9d252b;
      display: table-cell;
    }

    .yellow-circle{
      background-color: #ffc100;
      border-color: #9d802c;
    }
    .green-circle {
      background-color: #00d742;
      border-color: #049931;
    }
  }
  .content {
    background-color: #002536;
    box-sizing: border-box;
    font-family: monospace;
    width: $width;
    margin: 0 auto;
    padding: 20px;
    border-bottom-left-radius: 5px;
    border-bottom-right-radius: 5px;
    color: white;
    text-align: left;
  }
</style>
