# candytsai.github.io
<!DOCTYPE html>
<html lang="en"> 
<head>
    <title>Bootstrap Resume/CV Template for Developers</title>
    
    <!-- Meta -->
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Responsive Resume Template">
    <meta name="author" content="Xiaoying Riley at 3rd Wave Media">    
    <link rel="shortcut icon" href="favicon.ico"> 
    
    <!-- Google Font -->
    <link href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700,900" rel="stylesheet">
    
    <!-- FontAwesome JS-->
	<script defer src="assets/fontawesome/js/all.min.js"></script>
       
    <!-- Theme CSS -->  
    <style>
    /*! 
 * Template Name: Pillar - Bootstrap 5 Resume/CV Template for Developers
 * Version: Bootstrap 5 v3.0
 * Author: Xiaoying Riley
 * Copyright: 3rd Wave Media
 * Twitter: @3rdwave_themes
 * Website: https://themes.3rdwavemedia.com/
*/

// Define theme colour scheme
$theme-color-primary: #59578E;
$theme-text-color-primary: #434E5E;
$theme-text-color-secondary: lighten($theme-text-color-primary, 10%);
$theme-text-color-light: lighten($theme-text-color-primary, 40%);
$theme-border-color:  lighten($theme-text-color-primary, 10%);
$theme-divider-color: lighten($theme-text-color-primary, 10%);
$theme-bg-light: #F7F8FA;
$theme-bg-dark: $theme-text-color-primary;

// Create variables to override the default value for variables used in the Bootstrap SCSS files.
$theme-colors: (
  "primary":  $theme-color-primary, 
  "secondary":  $theme-text-color-secondary, 
);

//Import Bootstrap
@import "bootstrap/scss/bootstrap.scss";


/*************************** Pillar Styles ****************************/
body {
    font-family: 'Roboto', sans-serif;  
    background: $theme-bg-light;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: $theme-text-color-primary;
    overflow-x: hidden;
    
}

a {
	color: $theme-color-primary;
	
	&:hover {
		color: darken($theme-color-primary, 15%);
	}
	
	&.no-text-decoration {
		text-decoration: none;
	}
}

.theme-bg-primary {
	background-color: $theme-color-primary;
}

.theme-bg-primary-darken {
	background-color: darken($theme-color-primary, 20%);
}

a.theme-btn-on-bg, .theme-btn-on-bg {
	background: rgba(0, 0, 0, 0.2);
	color: #fff;
	border: none;
	&:hover, &:focus, &:active {
		background: rgba(0, 0, 0, 0.4);
		border-color: transparent;border: none;
	}
	
}

.progress {
	@include border-radius(2px);
}

.theme-progress-bar-dark {
	background-color: $theme-color-primary;
	
}

.resume-wrapper {
    padding-top: 30px;
    padding-bottom: 60px;
	
}

.resume-wrapper-inner {
	max-width: 1000px;
}

.resume-header {
	background: $theme-color-primary;
	color: rgba(256, 256, 256, 0.9);
	height: 220px;
	.picture {
		width: 220px;
	}
		
	.name {
		font-size: 2.25rem;
		letter-spacing: 0.175rem;	
		font-weight: 900;
	}
	.title {
		font-size: 1.5rem;
	}
	
	a {
		color: rgba(256, 256, 256, 0.6);
		&:hover {
			color: white;
		}
		
	}
	
	
}
.resume-social {
	font-size: 0.875rem;

	.fa-container {
		font-size: 1rem;
		display:inline-block;
		width: 24px;
		height: 24px;
		@include border-radius(0.125rem);
		background: white;
		color: $theme-color-primary;
	}

}

.resume-section-title {
	font-size: 1.25rem;
	position: relative;
	color: $theme-color-primary;
	
	&:after {
		content: "";
		position: absolute;
		left: 0;
		bottom: 0;
		width: 100%;
		height: 1.5px;
		background: lighten($theme-text-color-primary, 30%);
	}
}

.resume-section-content {
	color: $theme-text-color-secondary;
}


.resume-timeline {
	padding-left: 2rem;
	&:before {
		content: "";
		display: inline-block;
	    width: 3px;
	    height: 100%;
	    background: lighten($theme-color-primary, 40%);
	    left: 6px;
	    top: 4px;
	    position: absolute;
	}
}

.resume-timeline-item {
	&:before {
		content: "";
		display: inline-block;
		position: absolute;
		left: -32px;
		top: 3px;
		width: 15px;
		height: 15px;
		border: 4px solid lighten($theme-color-primary, 10%);
		background: white;
		@include border-radius(50%);
		
	}
}

.resume-progress {
	height: 0.6rem;
}

.resume-company-name {
	color: $theme-text-color-secondary;
	font-size: 0.875rem;
	font-weight: 500;
}

.resume-position-time {
	font-size: 0.875rem;
	color: $theme-text-color-light;
}

.resume-position-title {
	font-size: 1.125rem;
	color: $theme-text-color-primary;
}

.resume-timeline-item-desc-heading {
	font-size: 1rem;
}

.resume-skills-cat {
	font-size: 1rem;
	color: $theme-text-color-primary;
}

.resume-skill-name {
	font-size: 0.8125rem;
	color: $theme-text-color-primary;
}

.badge-light {
	color: $theme-text-color-secondary;
	background: $theme-bg-light;
}


.resume-degree {
	color: $theme-text-color-primary;
}
.resume-degree-org {
	font-size: 0.875rem;
}
.resume-degree-time {
	color: $theme-text-color-light;
	font-size: 0.875rem;
}

.resume-awards-list {

}

.resume-award-icon {
	left: 0;
	top: 4px;
	color: $theme-text-color-light;
}

.resume-award-name {
	font-weight:bold;
	color: $theme-text-color-primary;
}

.resume-award-desc {
	font-size: 0.875rem;
}

.resume-lang-name {
	color: $theme-text-color-primary;
}

.footer {

	.fa-heart {
		color: #fb866a;
	}
}

// Small devices (landscape phones, less than 768px)
@media (max-width: 767.98px) {
    .resume-wrapper {
	    padding-top: 0;
    }
	
	.resume-header {
		height: auto;
	}
	.resume-header .picture {
		width: 120px;
		@include border-radius(4px);
	}

	
}

    </style>


</head> 

<body>	

    <article class="resume-wrapper text-center position-relative">
	    <div class="resume-wrapper-inner mx-auto text-start bg-white shadow-lg">
		    <header class="resume-header pt-4 pt-md-0">
			    <div class="row">
				    <div class="col-block col-md-auto resume-picture-holder text-center text-md-start">
				        <img class="picture" src="assets/images/profile.jpg" alt="">
				    </div><!--//col-->
				    <div class="col">
					    <div class="row p-4 justify-content-center justify-content-md-between">
						    <div class="primary-info col-auto">
							    <h1 class="name mt-0 mb-1 text-white text-uppercase text-uppercase">蔡宜臻 I-Chen Tsai</h1>
							    <div class="title mb-3">CGU Biomedical Science Student</div>
							    <ul class="list-unstyled">
								    <li class="mb-2"><a class="text-link" href="#"><i class="far fa-envelope fa-fw me-2" data-fa-transform="grow-3"></i>B1009247@cgu.edu.tw</a></li>
								    <li><a class="text-link" href="#"><i class="fas fa-mobile-alt fa-fw me-2" data-fa-transform="grow-6"></i>0976128260</a></li>
							    </ul>
						    </div><!--//primary-info-->
						    <div class="secondary-info col-auto mt-2">
							    <ul class="resume-social list-unstyled">
							    </ul>
						    </div><!--//secondary-info-->
					    </div><!--//row-->
					    
				    </div><!--//col-->
			    </div><!--//row-->
		    </header>
		    <div class="resume-body p-5">
			    <section class="resume-section summary-section mb-5">
				    <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">Education Summary</h2>
				    <div class="resume-section-content">
					    <p class="mb-0">Education</p>
              <p>2021-2025 (Expected) <br>
                 B.S.,Department of Biomedical Science Chang Gung University <br>
                 Major: Biomedical Science Biomedical Research Program</p>
              <p class="mb-0">Scholarships</p>
              <p>Fall 2021-Spring 2024 Honor Program student (Silver Scholarship)</p>
              <p>Fall 2023 Academic Excellence Award </p>
              <p>Spring 2022 Academic Excellence Award </p>
              <p>Fall 2021 Academic Excellence Award </p>
				    </div>
			    </section><!--//summary-section-->
			    <div class="row">
				    <div class="col-lg-9">
					    <section class="resume-section experience-section mb-5">
						    <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">Education Timeline & Courses</h2>
						    <div class="resume-section-content">
							    <div class="resume-timeline position-relative">
								    <article class="resume-timeline-item position-relative pb-5">
									    
									    <div class="resume-timeline-item-header mb-2">
										    <div class="d-flex flex-column flex-md-row">
										        <h3 class="resume-position-title font-weight-bold mb-1">Freshman</h3>
										        <div class="resume-company-name ms-auto">CGU 110-1/110-2</div>
										    </div><!--//row-->
<!-- 										    <div class="resume-position-time">2023 - Present</div> -->
									    </div><!--//resume-timeline-item-header-->
									    <div class="resume-timeline-item-desc">
										    <li>General Biology (Ⅰ)(Ⅱ)</li>
                        <li>Biomathematics (Ⅰ)(Ⅱ)</li>
                        <li>General Chemistry </li>
                        <li>General Chemistry Laboratory</li>
                        <li>Physics with Lab </li>
                        <li>Organic Chemistry</li>                        
                        <li>Experimental Organic Chemistry</li>
                        <li>Introduction to Artificial Intelligence</li>
                        <li>Basic English(Ⅰ)</li>
                        <li>The English Honors Program </li>
                        <li>Research Orientation (1)</li>
                        <li>Basic programming language for biologists (Python)</li>
                        <li>Humanity & Social Aspect of Science</li>
                        <li>North American Novels, Domestic Arts, and Gender</li>
                        <li>Critical Thinking: Virtue and Happiness</li>
                        <li>Reflection of Life from First Aid cases</li>
                        
                       
                        
                        
                        
                        
                        
										    
									    </div><!--//resume-timeline-item-desc-->

								    </article><!--//resume-timeline-item-->
								    
								    <article class="resume-timeline-item position-relative pb-5">
									    
									    <div class="resume-timeline-item-header mb-2">
										    <div class="d-flex flex-column flex-md-row">
										        <h3 class="resume-position-title font-weight-bold mb-1">Sophomore</h3>
										        <div class="resume-company-name ms-auto">CGU 111-1/111-2</div>
										    </div><!--//row-->
									    </div><!--//resume-timeline-item-header-->
									    <div class="resume-timeline-item-desc">
										    <li>Biochemistry</li>
                        <li>Analytical Chemistry</li>
                        <li>Biochemistry Laboratory</li>
                        <li>Biostatistics</li>
                        <li>Physiology</li>
                        <li>Molecular Biology</li>
                        <li>Cell Biology</li>
                        <li>Molecular Biology Laboratory</li>  
                        <li>Molecular Cloning</li>
                        <li>Research Practice (1)(2)</li>                     
                        <li>Forum for young leaders</li>
                        <li>The English Honors Program </li>
                        <li>Environmental Studies Ecocide, Ecosystems, and the Fate of the Planet</li>
                        <li>Truth behind the Scenes, Exploring by Mathematics and Quantum Computing</li>               
                        <li>Transcultural, Health, and Medical Care</li>
                        <li>Introduction to Acupuncture and Moxibustion</li>
                        
                        
									    </div><!--//resume-timeline-item-desc-->

								    </article><!--//resume-timeline-item-->
								    
								    <article class="resume-timeline-item position-relative pb-5">
									    
									    <div class="resume-timeline-item-header mb-2">
										    <div class="d-flex flex-column flex-md-row">
										        <h3 class="resume-position-title font-weight-bold mb-1">Junior</h3>
                          <div class="resume-company-name ms-auto">CGU 112-1/112-2</div>
										    </div><!--//row-->
									    </div><!--//resume-timeline-item-header-->
									    <div class="resume-timeline-item-desc">
										    <li>Genetics</li>
                        <li>Immunobiology</li>
                        <li>Microbiology</li>
                        <li>Introduction to Omics</li>
                        <li>Biological Psychology</li>
                        <li>Introduction to Life Science Research</li>
                        <li>Bioinformatics</li>
                        <li>Big Data Analysis and Visualization</li>
                        <li>Introduction to English Scientific Writing and Presentation</li>
                        <li>Biotechnology English</li>
										    <li>Web Programming</li>
                        <li>Independent Study (Ⅰ)(Ⅱ)</li>
                        <li>Seminar (Ⅰ)(Ⅱ)</li>      
                        <li>Fables：A Multidimensional View of Classics</li>
                        <li>The English Honors Program</li>
                        <li>French (Ⅱ)</li>
                        
                        
                        
									    </div><!--//resume-timeline-item-desc-->

								    </article><!--//resume-timeline-item-->
								    
								    
								    
								    
							    </div><!--/resume-timeline-->
							    
							    
							    
							    
							    
							    
						    </div>
					    </section><!--//experience-section-->
				    </div>
				    <div class="col-lg-3">
					    <section class="resume-section skills-section mb-5">
						    <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">Skills &amp; Tools</h2>
						    <div class="resume-section-content">
						        <div class="resume-skill-item">
							        <h4 class="resume-skills-cat font-weight-bold">Frontend</h4>
							        <ul class="list-unstyled mb-4">
								        <li class="mb-2">
								            <div class="resume-skill-name">HTML</div>
								        </li>
								        <li class="mb-2">
								            <div class="resume-skill-name">CSS</div>

								        </li>
								        <li class="mb-2">
								            <div class="resume-skill-name">JavaScript</div>
								        </li>

							        </ul>
						        </div><!--//resume-skill-item-->
						        
						        <div class="resume-skill-item">
						            <h4 class="resume-skills-cat font-weight-bold">Backend</h4>
							        <ul class="list-unstyled">
								        <li class="mb-2">
								            <div class="resume-skill-name">Python</div>
								        </li>
								        </li>
								        <li class="mb-2">
								            <div class="resume-skill-name">PHP</div>
								        </li>
                      
							        </ul>
						        </div><!--//resume-skill-item-->
						    </div><!--resume-section-content-->
					    </section><!--//skills-section-->
					    <section class="resume-section education-section mb-5">
						    <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">Education</h2>
						    <div class="resume-section-content">
							    <ul class="list-unstyled">
								    <li class="mb-2">
								        <div class="resume-degree font-weight-bold">B.S.,Department of Biomedical Science</div>
								        <div class="resume-degree-org">Chang Gung University</div>
								        <div class="resume-degree-time">2021-2025 (Expected)</div>
								    </li>
							    </ul>
						    </div>
					    </section>
					    <section class="resume-section language-section mb-5">
						    <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">Language</h2>
						    <div class="resume-section-content">
							    <ul class="list-unstyled resume-lang-list">
								    <li class="mb-2"><span class="resume-lang-name font-weight-bold">Chinese</span> <small class="text-muted font-weight-normal">(Native)</small></li>
								    <li class="mb-2 align-middle"><span class="resume-lang-name font-weight-bold">English</span></li>
						    </div>
					    </section>
					    <section class="resume-section interests-section mb-5">
						    <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">Interests</h2>
						    <div class="resume-section-content">
							    <ul class="list-unstyled">
                    <li class="mb-1">Reading </li>
								    <li class="mb-1">Travelling</li>
								    <li class="mb-1">Going to movies</li>
								    
							    </ul>
						    </div>
					    </section><!--//interests-section-->
					    
				    </div>
			    </div><!--//row-->
		    </div><!--//resume-body-->
		    
		    
	    </div>
    </article> 

    
    <footer class="footer text-center pt-2 pb-5">
	    <!--/* This template is free as long as you keep the footer attribution link. If you'd like to use the template without the attribution link, you can buy the commercial license via our website: themes.3rdwavemedia.com Thank you for your support. :) */-->
        <small class="copyright">Designed with <span class="sr-only">love</span><i class="fas fa-heart"></i> by <a href="http://themes.3rdwavemedia.com" target="_blank">Xiaoying Riley</a> for developers</small>
    </footer>

    

</body>
</html> 

