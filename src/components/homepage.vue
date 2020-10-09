<template>
  <div class="homepage">
    <div class="header__container">
      <div class="navbar">
        <nav>
          <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Reviews</a></li>
            <li><a href="#">Portfolio</a></li>
            <li><a href="#">Contact</a></li>
          </ul>
        </nav>
      </div>
      <div class="bg-video">
        <video class="bg-video__content" autoplay muted loop>
          <source src="../src/../assets/bg-vid-1.mp4" type="video/mp4" />
          <source src="img/video.webm" type="video/webm" />
          Your browser is not supported!
        </video>
      </div>
      <div class="header__container--herobox">
        <div class="header__container--heading">
          <h1>Discover your beauty</h1>
        </div>
        <div class="cta__container">
          <div class="cta">
            <!-- <a href="#">View Our Work</a> -->
          </div>
        </div>
      </div>
    </div>

    <div class="section--about">
      <div class="row">
        <div class="col-1-of-2">
          <img
            src="../src/../assets/insta/photo-2.jpg"
            alt="photo 1"
            class="composition__photo composition__photo--p1"
          />
        </div>
        <div class="col-1-of-2">
          <h3 class="heading-tertiary u-margin-bottom-small">
            Michelle & Bianca
          </h3>
          <p class="paragraph">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Beatae
            suscipit quidem veritatis dolores? Aperiam, natus? Nam corrupti,
            placeat ad nobis error earum ex tenetur quod beatae, aliquid tempore
            iste eos. Lorem ipsum dolor sit amet consectetur adipisicing elit.
            Minus blanditiis facilis repellat ullam nam et odit consectetur,
            dolor quasi quidem dolore quia animi atque facere numquam maxime,
            molestias amet at.
          </p>
          <p class="paragraph">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptate
            excepturi itaque inventore? Perspiciatis porro animi minima libero
            est totam et, quisquam impedit pariatur molestias eligendi! Ratione
            facilis voluptates autem quidem?. Lorem ipsum, dolor sit amet
            consectetur adipisicing elit. Error aperiam soluta sint. Illum
            dolorum, distinctio eaque aperiam aspernatur odit ea soluta labore
            quo reiciendis, assumenda, et cum. Illo, esse saepe.
          </p>
          <div class="cta">
            <a href="#">Our Work &rarr;</a>
          </div>
          <!-- <a href="#" class="btn-text">Our Work &rarr;</a> -->
        </div>
      </div>
    </div>

    <div class="section--offerings">
      <div class="row">
        <div class="col-1-of-3">
          <img
            src="../src/../assets/insta/photo-1.jpg"
            alt="photo 2"
            class="composition__photo composition__photo--p2"
          />
        </div>
        <div class="col-1-of-3">
          <img
            src="../src/../assets/insta/photo-1.jpg"
            alt="photo 3"
            class="composition__photo composition__photo--p3"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@import "../scss_global/_mixins.scss";
@import "../scss_global/_variables.scss";
@import "../scss_global/_grid.scss";
a {
  text-decoration: none;
  // color: white;
  display: inline-block;
  transition: 0.2s all;
  text-transform: uppercase;
  color: #355c7d;
  font-weight: 700;
}

p {
  text-transform: lowercase;
  letter-spacing: 1px;
}
h3 {
  text-transform: uppercase;
}

img {
  width: 100%;
  // box-shadow: 0 1.5rem 4rem rgba($color-black, 0.4);
  border-radius: 2px;
  // position: absolute;
  z-index: 10;
  transition: all 0.2s;
  outline-offset: 1rem;
  border: 1px solid #5c969e;
  outline: 1.5px solid #5c969e;
}

.bg-video {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  z-index: -1;
  opacity: 0.6;
  overflow: hidden;
  border-radius: inherit;

  &__content {
    height: 100%;
    width: 100%;
    object-fit: cover;
  }
}
.header__container {
  position: relative;
  height: 95vh;
  background-image: linear-gradient(to right bottom,
      rgba(#f67280, 0.3),
      rgba(#6c5b7b, 1));
  background-size: cover;
  background-position: top;
  border-radius: 0 0 0 3rem;
  border-bottom: 2px solid #355c7d;
  // background-position: bottom;

  &--herobox {
    position: absolute;
    // top: 40%;
    left: 0;
    bottom: 0;
    // left: 50%;
    // transform: translate(-50%, -50%);
    text-align: center;
    background-color: rgba($color: #000000, $alpha: 0.3);
    width: 65%;
    border-radius: 0 3rem 0 3rem;
    padding: 1rem;
    // box-shadow: 0 0.5rem 3rem rgba($color: #000000, $alpha: 0.5);
  }
  & h1 {
    font-family: "Oswald", cursive;
    letter-spacing: 8px;
    font-size: 3.5rem;
    text-transform: uppercase;
    color: white;
  }

  &--herobox a {
    border: 3px solid rgba(#5c969e, 0.5);
    background: rgba($color: #000000, $alpha: 0.3);
    text-transform: uppercase;
    padding: 1.5rem;
    border-radius: 4px;

    &:hover {
      transform: scale(1.1);
      background-color: rgba($color: #000000, $alpha: 0.5);
      color: #ffcbcb;
      border-color: white;
    }
  }
}

.navbar {
  text-align: right;
  padding: 1rem;
  // opacity: 0.9;
  // color: black;
  border-bottom: 2px solid #355c7d;
  background-color: white;

  & ul {
    margin: 0;
  }

  & li {
    list-style: none;
    display: inline-block;
    margin: 1rem;
    right: 0;
    transition: 0.2s all;
  }
  & li a:hover {
    transform: scale(1.2);
    color: #ffcbcb;
  }
}

.section--about {
  padding: 2rem;

  & img {
    width: 70%;
  }
}
</style>