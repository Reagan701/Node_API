<template>
  <article>
    <div class="container">
      <div class="row">
        <div
          class="col-md-4 col-lg-4 col-12"
          v-for="item in FoodArray"
          :key="item.id"
        >
          <section class="card-content">
            <div class="card-content">
              <div class="card">
                <div class="layer"></div>
                <div class="content">
                    <img :src="item.icon" alt="avatar" id="food-img" class="img-fluid image"/>
                  <br />
                  <div class="details">
                    <span>{{ item.title }}</span>
                    <br />
                    <a
                      id="live"
                      target="_blank"
                      class="text-primary bi bi-github mx-2 fs-1"
                      :href="item.link1"
                    ></a>
                    <a
                      id="live"
                      target="_blank"
                      class="text-primary bi bi-link-45deg mx-2 fs-1"
                      :href="item.link2"
                    ></a>
                  </div>
                </div>
              </div>
            </div>
          </section>
        </div>
      </div>
    </div>
  </article>
</template>

<script scoped>
export default {
  data() {
    return {
      FoodArray: [
        {
          id: 1,
          icon: "https://i.postimg.cc/RZCK8KBX/Milk.webp",
          title: "Milk",
        },
        {
          id: 2,
          icon: "https://i.postimg.cc/d1GhDVFh/cereal.webp",
          title: "Cereal",
        },
      ],
    };
  },
};
</script>

<style scoped>
#food-img {
  object-fit: cover;
}
.card-content {
  margin: 50px auto 50px;
  display: grid;
  grid-gap: 20px;
}

.card-content .card {
  position: relative;
  margin: 0 auto;
  width: 285px !important;
  width: fit-content;
  background: white;
  color: #00a5ff;
  padding: 20px;
  box-sizing: border-box;
  text-align: center;
  box-shadow: 0 10px 40px rgba(0, 0, 0, 0.5);
  overflow: hidden;
  border-radius: 30px;
}
.card-content .card .layer {
  position: absolute;
  top: calc(100% - 2px);
  left: 0;
  height: 100%;
  width: 100%;
  background: linear-gradient(#00a5ff, #0004ff);
  z-index: 1;
  transition: 0.5s;
}
.card-content .card:hover .layer {
  top: 0;
}
.card-content .card .content {
  position: relative;
  z-index: 2;
}
.card-content .card .content p {
  font-size: 18px;
  line-height: 24px;
}
.card-content .card .content .image {
  width: 100%;
  height: 180px;
  margin: 0 auto;
  overflow: hidden;
  overflow: hidden;
  border: 5px solid navy;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}
.card-content .card .content .details h2 {
  font-size: 18px;
}
.card-content .card .content .details span {
  color: #03a9f4;
  font-size: 14px;
  transition: 0.5s;
}
.card-content .card:hover .content .details span {
  color: #fff;
}
.card-content .card:hover .content p {
  color: white;
}
</style>