<template>
  <div class="wrapper">
    <header class="header">
      <h1 class="title"><strong>Pure</strong> {{ name }}</h1>
    </header>

    <section>
      <!-- First example -->
      <div class="example-wrapper">
        <h2 class="example-title">Title</h2>
        <p class="example-description">Text</p>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: `Pure${this.name}`,
  data() {
    return {
      name: "Rating"
    };
  }
};
</script>

<style>
.wrapper {
  width: 80%;
  max-width: 1000px;
  margin-left: auto;
  margin-right: auto;
}

.header {
  display: flex;
  align-items: center;
}

.title {
  font: bold 32px "Roboto";
  margin-bottom: 8px;
}
.title strong {
  color: #41b883
}

.example-wrapper {
  margin-top: 40px;
}

.example-wrapper:not(:last-of-type) {
  margin-bottom: 60px;
}

.example-title {
  margin: 0;
}

.example-description {
  margin-top: 10px;
  margin-bottom: 20px;
  color: gray;
}

@media (min-width: 769px) {
  .example-title {
    font: bold 26px "Roboto";
  }
  .example-description {
    font: normal 22px "Roboto";
  }
}

@media (max-width: 768px) {
  .example-title {
    font: bold 22px "Roboto";
  }
  .example-description {
    font: normal 16px "Roboto";
  }
}
</style>
