<!DOCTYPE html>

<html>
<head>
<title>	Webserie	</title>
<link type="text/css" rel="stylesheet" href="stilark.css"/>
<meta charset="UTF-8">
	
</head>

<body>






	<video   autoplay loop  id="video" >
    <source src="klipp1.mp4" type="video/mp4">
    <source src="klipp2.mp4" type="video/mp4">

  </video>




<script>
video_count =1;
videoPlayer = document.getElementById("video");

function run(){
        video_count++;
        if (video_count == 16) video_count = 1;
        var nextVideo = "klipp"+video_count+".mp4";
        videoPlayer.src = nextVideo;
        videoPlayer.play();
   };

   var el = document.getElementById("video");
  if (el.addEventListener) {
      el.addEventListener("click", yourNextFunction, false);
  } else {
      el.attachEvent('onclick', yourNextFunction);
  }  

  var video_count =1,
    videoPlayer = document.getElementById("video");

function yourNextFunction (){
      video_count++;
      if (video_count == 16) video_count = 1;
      var nextVideo = "klipp"+video_count+".mp4";
      videoPlayer.src = nextVideo;
      videoPlayer.play();
}
   </script>

	


</body>

</html>
