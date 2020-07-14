<template>
  <div class="single-post">
    <section class="post-details">
      <h1 class="post-title">This is single post title</h1>
      <div class="post-details">
        <div class="post-detail">last updated on</div>
        <div class="post-detail">written by name</div>
      </div>
      <p class="post-content">Content of the post</p>
    </section>
    <section class="post-feedback">
      <p>let me know what you thincc, send nude to <a href="mailto:idk@idk.com">idk mail</a></p>
    </section>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped> 
.single-post {
  padding: 30px;
  text-align: center;
  box-sizing: border-box;
}

.post {
  width: 100%;
}

@media (min-width: 768px) {
  .post {
    width: 600px;
    margin: auto;
  }
}

.post-title {
  margin: 0;
}

.post-details {
  padding: 10px;
  box-sizing: border-box;
  border-bottom: 3px solid #ccc;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

@media (min-width: 768px) {
  .post-details {
    flex-direction: row;
  }
  .post-detail {
    color: rgb(88, 88, 88);
    margin: 0 10px;
  }
  .post-feedback a {
    color: red;
    text-decoration: none;
  }
  .post-feedback a:hover,
  .post-feedback a:active {
    color: salmon;
  }
}
</style>