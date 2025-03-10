<template>
  <div class="main-view">
    <div class="header">
      <img src="https://placehold.co/600x400" alt="Main Banner Image" class="banner">
      <div class="context-box">
        <img src="https://placehold.co/400x150" alt="Logo" class="logo">
        <div class="text">
          <!-- <h1 class="title"></h1> -->
           <!-- Mailto -->
          <span>For info on acquiring any of my books, contact me at:</span>
          <a href="mailto:klenagh@polarcomm.com" class="title">
              <span class="text">klenagh@polarcomm.com</span>
          </a>
        </div>
      </div>
    </div>
    <div class="body">
      <div class="content">
        <div class="grid">
          <div class="grid-item" v-for="i in 6" :key="i">
            <img src="https://placehold.co/200x150" alt="Placeholder Image" class="placeholder-image">
          </div>
        </div>
      </div>
      <div class="main-comic">
        <img src="https://placehold.co/600x400" alt="Main Comic Image" class="comic-image">
      </div>
    </div>
    <div class="footer"></div>
  </div>
</template>
<style lang="scss" scoped>
.main-view {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  min-height: 100vh;
  background-color: #fefefe;
  .header {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
    background-color: #fefefe;
    .banner {
      width: 100%;
      height: auto;
      max-height: 400px;
      object-fit: cover;
    }
    .context-box {
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 20px;
      .logo {
        width: 150px;
        height: auto;
        margin-right: 20px;
      }
      .text {
        max-width: 600px;
        text-align: center;
        span {
          display: block;
          font-size: 18px;
          color: #333;
        }
        .title {
          font-size: 24px;
          color: #333;
          text-decoration: none;
          margin-top: 10px;
          &:hover {
            text-decoration: underline;
          }
        }
        .text {
          font-size: 18px;
          color: #333;
          margin-top: 10px;
        }
      }
    }
  }
  .content {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
    padding: 20px;
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
      width: 100%;
      .grid-item {
        background-color: #fefefe;
        border-radius: 8px;
        overflow: hidden;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        .placeholder-image {
          width: 100%;
          height: auto;
          object-fit: cover;
        }
      }
    }
    .main-comic {
      margin-top: 20px;
      width: 100%;
      max-width: 600px;
      .comic-image {
        width: 100%;
        height: auto;
        object-fit: cover;
      }
    }
  }
  .footer {
    width: 100%;
    height: 50px;
    background-color: #f0f0f0;
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 14px;
  }
}
</style>