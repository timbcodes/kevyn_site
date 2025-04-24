<template>
  <div class="main-view">
    <div class="header">
      <img
        src="@/assets/images/Domino2013-3.jpg"
        alt="Main Banner Image"
        class="banner"
      />
      <div class="context-box">
        <img
          src="@/assets/images/qr1.png"
          alt="Logo"
          class="logo"
        />
        <img
          src="@/assets/images/DClogo1.jpg"
          alt="Logo"
          class="logo"
        />
        <div class="text">
          <span>For info on acquiring any of my books, contact me at:</span>
          <a href="mailto:klenagh@polarcomm.com" class="title">
            <span class="text">klenagh@polarcomm.com</span>
          </a>
        </div>
        <img
          src="@/assets/images/qr2.png"
          alt="Logo"
          class="logo"
        />
      </div>
    </div>

    <div class="body">
      <div class="content">
        <div class="grid">
          <div class="grid-item">
            <img
              src="@/assets/images/Domino Chance Cover 1.jpg"
              alt="Placeholder Image"
              class="placeholder-image"
            />
          </div>
          <div class="grid-item">
            <img
              src="@/assets/images/Domino Chance Cover 3.jpg"
              alt="Placeholder Image"
              class="placeholder-image"
            />
          </div>
          <div class="grid-item">
            <img
              src="@/assets/images/Domino Chance Cover 4.jpg"
              alt="Placeholder Image"
              class="placeholder-image"
            />
          </div>
          <div class="grid-item">
            <img
              src="@/assets/images/Domino Chance Cover 5.jpg"
              alt="Placeholder Image"
              class="placeholder-image"
            />
          </div>
          <div class="grid-item">
            <img
              src="@/assets/images/Domino Chance Cover 6.jpg"
              alt="Placeholder Image"
              class="placeholder-image"
            />
          </div>
          <div class="grid-item">
            <img
              src="@/assets/images/Domino Chance Cover 7.jpg"
              alt="Placeholder Image"
              class="placeholder-image"
            />
          </div>
          <div class="grid-item">
            <img
              src="@/assets/images/Domino Chance Cover 8.jpg"
              alt="Placeholder Image"
              class="placeholder-image"
            />
          </div>
          <div class="grid-item">
            <img
              src="@/assets/images/Domino Chance Cover 9.jpg"
              alt="Placeholder Image"
              class="placeholder-image"
            />
          </div>
          <div class="grid-item">
            <img
              src="@/assets/images/Domino Chance Cover 10.jpg"
              alt="Placeholder Image"
              class="placeholder-image"
            />
          </div>
          <div class="grid-item">
            <img
              src="@/assets/images/A_frontcover Domino11.jpg"
              alt="Placeholder Image"
              class="placeholder-image"
            />
          </div>
        </div>
      </div>

      <div class="main-comic">
        <img
          src="@/assets/images/newcomic.jpg"
          alt="Placeholder Image"
          class="comic-image"
        />
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
      flex-wrap: wrap;
      text-align: center;

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
          display: inline-block;

          &:hover {
            text-decoration: underline;
          }
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

    /* Use flex, allow wrapping, center items. */
    .grid {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      width: 100%;
      max-width: 1200px;
      gap: 20px;

      .grid-item {
        /* Keep each item at 200px wide so no horizontal scrolling. */
        width: 200px;
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
  }

  .main-comic {
    margin-top: 20px;
    width: 100%;
    max-width: 600px;
    display: flex;
    justify-content: center;

    .comic-image {
      width: 100%;
      height: auto;
      object-fit: cover;
    }
  }

  .footer {
    width: 100%;
    height: 50px;
    background-color: #f0f0f0;
    color: #333;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 14px;
  }
}

/* Responsive Design */
@media (max-width: 768px) {
  .context-box {
    flex-direction: column;
    text-align: center;
  }

  .context-box .logo {
    margin-bottom: 10px;
    margin-right: 0;
  }
}

@media (max-width: 480px) {
  .banner {
    max-height: 250px;
  }

  .title {
    font-size: 20px;
  }

  .footer {
    font-size: 12px;
  }
}
</style>
