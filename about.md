---
layout: page
title: About
comments: true
---


<script>
.pb-100 {
	padding-bottom: 100px;
}
.pt-100 {
	padding-top: 100px;
}
.section-title {
	margin-bottom: 110px;
	position: relative;
}
.section-title h3 {
	text-transform: uppercase;
	font-weight: 800;
	font-size: 30px;
}

.section-title:before {
	position: absolute;
	content: "";
	width: 110px;
	height: 1px;
	background-color: #635CDB;
	left: 50%;
	-webkit-transform: translate(-50%, -50%) rotate(90deg);
	        transform: translate(-50%, -50%) rotate(90deg);
	top: 50%;
}
.section-title:after {
	position: absolute;
	content: "";
	width: 80px;
	height: 1px;
	background-color: #635CDB;
	left: 50%;
	-webkit-transform: translateX(-50%);
	        transform: translateX(-50%);
	bottom: -20px;
}
.section-title h3 span {
	display: block;
	font-size: 15px;
	text-transform: lowercase;
	font-weight: 400;
	margin-bottom: 10px;
}
.section-title p {
	margin-top: 5px;
}
.team-hover {
	text-align: center;
	position: absolute;
	left: 0;
	top: 0;
	width: 100%;
	height: 100%;
	z-index: 2;
	color: #fff;
	visibility: hidden;
	opacity: 0;
	-ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=0)";
	-webkit-transition: .5s;
	transition: .5s
}

.single-team img {
	width: 100%;
}

.team-hover h4 {
	text-transform: capitalize;
	font-size: 20px;
	font-weight: 600;
}

.team-hover h4 span {
	display: block;
	font-size: 13px;
	font-weight: 400;
	margin-top: 5px;
}

.team-hover ul {
	list-style: none;
	margin: 0;
	padding: 0;
	margin-top: 15px;
}

.team-hover ul li {
	display: inline-block;
}

.team-hover ul li {
	background-color: #333;
	width: 25px;
	height: 25px;
	line-height: 25px;
	border-radius: 50%;
	margin: 0 2px;
	text-align: center
}

.team-hover ul li a {
	color: #fff;
	font-size: 13px;
	display: block;
}
.single-team {
	position: relative;
	z-index: 2;
}

.team-content {
	position: absolute;
	left: 50%;
	top: 50%;
	-webkit-transform: translate(-50%, -50%);
	        transform: translate(-50%, -50%);
}

.team-hover:before {
	position: absolute;
	content: "";
	width: 100%;
	height: 100%;
	left: 0;
	top: 0;
	background-color: #333;
	z-index: -1;
	opacity: .85;
	-ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=85)";
}

.single-team:hover .team-hover {
	visibility: visible;
	opacity: 1;
	-ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
}
</script>


<body>
    <section class="team-area pb-100 pt-100" id="team">
         <div class="container">
            <div class="row section-title">
               <div class="col-md-6 text-right">
                  <h3><span>who we are?</span> creative team</h3>
               </div>
               <div class="col-md-6">
                  <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry typesetting industry.d </p>
               </div>
            </div>
            <div class="row">
               <div class="col-md-4">
                  <div class="single-team">
                     <img src="http://infinityflamesoft.com/html/halim-preview/assets/img/team/1.jpg" alt="">
                     <div class="team-hover">
                        <div class="team-content">
                           <h4>john doe <span>web developer</span></h4>
                           <ul>
                              <li><a href="#"><i class="fa fa-facebook"></i></a></li>
                              <li><a href="#"><i class="fa fa-twitter"></i></a></li>
                              <li><a href="#"><i class="fa fa-linkedin"></i></a></li>
                              <li><a href="#"><i class="fa fa-google-plus"></i></a></li>
                           </ul>
                        </div>
                     </div>
                  </div>
               </div>
               <div class="col-md-4">
                  <div class="single-team">
                     <img src="http://infinityflamesoft.com/html/halim-preview/assets/img/team/2.jpg" alt="">
                     <div class="team-hover">
                        <div class="team-content">
                           <h4>john doe <span>web developer</span></h4>
                           <ul>
                              <li><a href="#"><i class="fa fa-facebook"></i></a></li>
                              <li><a href="#"><i class="fa fa-twitter"></i></a></li>
                              <li><a href="#"><i class="fa fa-linkedin"></i></a></li>
                              <li><a href="#"><i class="fa fa-google-plus"></i></a></li>
                           </ul>
                        </div>
                     </div>
                  </div>
               </div>
               <div class="col-md-4">
                  <div class="single-team">
                     <img src="http://infinityflamesoft.com/html/halim-preview/assets/img/team/3.jpg" alt="">
                     <div class="team-hover">
                        <div class="team-content">
                           <h4>john doe <span>web developer</span></h4>
                           <ul>
                              <li><a href="#"><i class="fa fa-facebook"></i></a></li>
                              <li><a href="#"><i class="fa fa-twitter"></i></a></li>
                              <li><a href="#"><i class="fa fa-linkedin"></i></a></li>
                              <li><a href="#"><i class="fa fa-google-plus"></i></a></li>
                           </ul>
                        </div>
                     </div>
                  </div>
               </div>
            </div>
         </div>
      </section>
</body>
