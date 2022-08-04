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
                      class="text-primary fa-solid fa-eye fs-1"
                      :href="item.link1"
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
          link1: "https://github.com/Tempestfury11/Age2Days",
        },
        {
          id: 2,
          icon: "https://i.postimg.cc/d1GhDVFh/cereal.webp",
          title: "Cereal",
          link1: "https://github.com/Tempestfury11/Age2Days",
        },
        {
          id: 3,
          icon: "https://i.postimg.cc/rmKSjYbS/bread.webp",
          title: "Bread",
          link1: "https://github.com/Tempestfury11/Age2Days",
        },
        {
          id: 4,
          icon: "https://i.postimg.cc/YSg4SKJD/cheese.jpg",
          title: "Cheese",
          link1: "https://github.com/Tempestfury11/Age2Days",
        },
        {
          id: 5,
          icon: "https://i.postimg.cc/s2ScCLKs/tomato.jpg",
          title: "Tomato",
          link1: "https://github.com/Tempestfury11/Age2Days",
        },
        {
          id: 6,
          icon: "https://i.postimg.cc/LXxvx1N1/brussell.jpg",
          title: "Brussel",
          link1: "https://github.com/Tempestfury11/Age2Days",
        },
        {
          id: 7,
          icon: "https://i.postimg.cc/kGZ0hZfK/beef.jpg",
          title: "Beef",
          link1: "https://github.com/Tempestfury11/Age2Days",
        },
        {
          id: 8,
          icon: "https://i.postimg.cc/QCgJPYgV/drumstick.jpg",
          title: "Chicken",
          link1: "https://github.com/Tempestfury11/Age2Days",
        },
        {
          id: 9,
          icon: "https://i.postimg.cc/zfRX8syt/coffee.webp",
          title: "Coffee",
          link1: "https://github.com/Tempestfury11/Age2Days",
        },
      ],
    };
  },
};
</script>

<style scoped>
#food-img {
  object-fit: cover;
  border-radius: 30px;
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
  color: navy;
  padding: 20px;
  box-sizing: border-box;
  text-align: center;
  box-shadow: 0 10px 40px rgba(0, 0, 0, 0.5);
  overflow: hidden;
  border-radius: 30px;
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
  border: 5px solid red;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}
.card-content .card .content .details h2 {
  font-size: 18px;
}
.card-content .card .content .details span {
  color: navy;
  font-size: 14px;
  transition: 0.5s;
}
</style>