<template>
  <div class="nav-side">
    <div class="img-para">
      <div>
        <img class="nav-img" src="../assets/home.svg" />
      </div>
      <p>Home</p>
    </div>
    <div class="img-para">
      <div>
        <img class="nav-img" src="../assets/explore.svg" />
      </div>
      <p>Explore</p>
    </div>
    <div class="img-para">
      <div>
        <img class="nav-img" src="../assets/subscriptions.svg" />
      </div>
      <p>Subscriptions</p>
    </div>
    <div class="img-para">
      <div>
        <img class="nav-img" src="../assets/originals.svg" />
      </div>
      <p>Originals</p>
    </div>
    <div class="img-para">
      <div>
        <img class="nav-img" src="../assets/youtube-music.svg" />
      </div>
      <p>Youtube Music</p>
    </div>
    <div class="img-para">
      <div>
        <img class="nav-img" src="../assets/library.svg" />
      </div>
      <p>Library</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "SideBar"
};
</script>

<style>
.nav-side{
	width: 80px;
	height: 100%;
	background-color: white;
	position: fixed;
	left: 0;
	top: 65px;
	z-index: 200;
}

	/* The img-para means nav image + paragraph */

.img-para{
	height: 90px;
	margin-top: 1px;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	cursor: pointer;
}

.img-para:hover{
	background-color: bisque;
}

/* The nav-img is the Home, Explore image etc */

.nav-img{
	width: 38px;
}

.img-para p{
	font-size: 12px;
	margin-top: 3px;
	margin-bottom: 3px;
}


@media  only screen and (max-width: 375px){
  .nav-side{
    width: 100%;
    height: 10vh;
    background-color: rgb(86, 49, 248);
    position: fixed;
    left: 0;
    top: 91%;
    /* bottom: 10%; */
    z-index: 200;
    display: flex;
    justify-content: space-around;
    align-items: center;
  }	
}
</style>
