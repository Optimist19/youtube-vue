<template>
  <div class="container">
    <div class="left-header">
      <div>
        <img class="ham-logo" src="../assets/hamburger-menu.svg" />
      </div>
      <div>
        <img class="youlogo" src="../assets/youtube-logo.svg" />
      </div>
    </div>

    <div class="middle-header">
      <input class="search-bar" type="text" placeholder="Search" />
      <div>
        <button class="search-button">
          <img class="search-icon" src="../assets/search.svg" />
        </button>
      </div>
      <div>
        <button class="voice-button">
          <img class="voice-icon" src="../assets/voice-search-icon.svg" alt="" />
        </button>
      </div>
    </div>

    <div class="right-header">
      <div>
        <img class="upload-icon" src="../assets/upload.svg" alt="" />
      </div>
      <div>
        <img class="you-app" src="../assets/youtube-apps.svg" />
      </div>
      <div class="not">
        <img class="not-icon" src="../assets/notifications.svg" />
        <div>7</div>
      </div>
      <div>
        <img class="user-icon" src="../assets/my-channel.jpeg" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeadYt"
};
</script>

<style>

.container{
	height: 75px;
	border-bottom: 1px solid gray;
	display: flex;
	justify-content: space-between;
	/* justify-content: center; */
	align-items: center;
	position: fixed;
	top: 0;
	left: 0;
	right: 0;
	background-color: white;
	z-index: 100;
}

			/* left-header
We have the hamburger and the youtube logo */

.left-header{
	display: flex;
}


.ham-logo{
	height: 30px;
	margin-left: 20px;
	cursor: pointer;
}


.youlogo{
	height: 30px;
	margin-left: 20px;
	cursor: pointer;
}

/* 				middle-header
We have anything that has to do with search-bar, the search and the voice icon  */

.middle-header{
	display: flex;
	flex: 0.5;
	margin-left: 50px;
	margin-right: 50px;
}


.search-bar{
	flex: 1;
	font-size: 16px;
	padding-top: 8px;
	padding-bottom: 8px;
	padding-left: 8px;
	width: 0;
}


.search-icon{
	height: 26px;
	margin-top: 3px;
}

.search-button{
	height: 38px;
	width: 60px;
	margin-left: -1px;
	cursor: pointer;
}


.voice-icon{
	height: 20px;
	margin-top: 3px;
}

.voice-button{
	height: 38px;
	width: 38px;
	border-radius: 19px;
	margin-left: 6px;
	border: none;
	cursor: pointer;
}

/* 				right-header
Here we have the upload icon, youtube-app icon, notification icon, and the user's profile picture */

.right-header{
	display: flex;
}


.upload-icon{
	height: 26px;
	margin-right: 20px;
	cursor: pointer;
}


.you-app{
	height: 26px;
	margin-right: 20px;
	cursor: pointer;
}


.not-icon{
	height: 26px;
	margin-right: 20px;
	cursor: pointer;
}

.not{
	position: relative;
	cursor: pointer;
}

.not div{
	position: absolute;
	left: 12px;
	top: 0;
	height: 12px;
	width: 12px;
	background-color: rgb(207, 1, 1);
	border: 1px solid white;
	border-radius: 50%;
	font-size: 10px;
	padding-top: 2px;
	padding-bottom: 2px;
	padding-left: 6px;
	color: white;
}

.user-icon{
	height: 34px;
	margin-right: 20px;
	cursor: pointer;
}

@media  only screen and (max-width: 375px){
	.ham-logo{
		display: none;
	}

	.youlogo{
		margin-left: 1vw;
	}

	.middle-header{
		flex: 0.2;
		margin-left: 2vw;
		margin-right: 2vw;
	}

	.voice-button{
		display: none
	}

	.upload-icon,
	.you-app,
	.not-icon,
	.user-icon{
		margin-right: 2vw;
	}
}
</style>
