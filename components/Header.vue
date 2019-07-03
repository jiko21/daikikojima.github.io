<template>
  <ul >
    <li>
      <a href="/">Home</a>
    </li>
    <li>
      <a href="/about">About me</a>
    </li>
    <li>
      <a href="/Works">Works</a>
    </li>
  </ul>
</template>
<style lang="scss" scoped>
  ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: #333;
    li {
      border-right: 1px solid #ccc;
      float: left;
      & > a {
        display: block;
        color: white;
        text-align: center;
        padding: 14px 16px;
        text-decoration: none;
        &:hover {
          background: #111;
        }
      }
    }
  }
</style>