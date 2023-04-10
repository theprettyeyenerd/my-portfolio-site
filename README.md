# my-portfolio-site
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vie' </title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <div id="header">
        <div class="container">
            <nav>
                <img src="img/yvette-sign.png" class=" dp">
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Services</a></li>
                    <li><a href="#">Portfolio</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </nav>
            <div class="header-text">
                <P>Bsc Computer Science</P>
                <h1> Hi, I'm<span> Yvette Moore</span><br> from Ghana</h1>
            </div>
            <!----------about--------->
            <div id="about">
                <div class="container">
                    <div class="row">
                        <div class="about-col-1">
                            <img src="img me.jpg"></div>
                        <div class="about-col-2">
                            <h1 class=" sub-title">About Me </h1>
                            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quos, doloremque, nesciunt dolorem quis tempore laborum obcaecati asperiores odit accusamus ad quibusdam iure velit consequuntur ut perspiciatis odio ipsam explicabo
                                laudantium?
                            </p>
                            <div class="tab-titles">
                                <p class=" tab-links active-link" onclick="opentab('skills')">Skills</p>
                                <p class=" tab-links" onclick="opentab('experience')">Experience</p>
                                <p class=" tab-links " onclick="opentab('education')">Education</p>
                            </div>
                            <div class="tab-contents active-tab" id="skills">
                                <ul>
                                    <li><span>UI/UX</span><br>Designing Web/App interfaces</li>
                                    <li><span>Web Development</span><br>web app development</li>
                                    <li><span>App Development</span><br>Building Andriod/iOs apps</li>
                                </ul>
                            </div>
                            <div>
                            </div>
                            <div class="tab-contents" id="experience">
                                <ul>
                                    <li><span>2018-2021</span><br>Robotics club</li>
                                    <li><span>2020</span><br> Final Cut Pro Video Editing</li>
                                    <li><span>2021-present</span><br>Bsc Computer Science</li>
                                </ul>
                            </div>
                            <div class="tab-contents" id="education">
                                <ul>
                                    <li><span>2018-2021</span><br>Mfantsiman Girls High School</li>
                                    <li><span>2021-present</span><br>Bsc Computer Science</li>
                                    <li><span>2023-present</span><br>Frontend Development</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <!--------services-------->
                    <div id="services">
                        <div class="container">
                            <h1 class="sub-title">My Services</h1>
                            <div class="services-list">
                                <div>
                                    <h2>Web Design</h2>
                                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Minima impedit unde dolores accusamus illo placeat hic, repellat nemo autem saepe, voluptatibus veniam eius nam amet necessitatibus excepturi repellendus nobis
                                        voluptate.
                                    </p>
                                    <a href="#">learn more</a>


                                </div>
                                <div>
                                    <h2>Video Editing</h2>
                                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Minima impedit unde dolores accusamus illo placeat hic, repellat nemo autem saepe, voluptatibus veniam eius nam amet necessitatibus excepturi repellendus nobis
                                        voluptate.
                                    </p>
                                    <a href="#">learn more</a>


                                </div>
                                <div>
                                    <h2>Content Creation</h2>
                                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Minima impedit unde dolores accusamus illo placeat hic, repellat nemo autem saepe, voluptatibus veniam eius nam amet necessitatibus excepturi repellendus nobis
                                        voluptate.
                                    </p>
                                    <a href="#">learn more</a>


                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <!--------------portfolio---------->
                <div class="portfolio">
                    <div class="container">
                        <h1 class="sub-title">My Work</h1>
                        <div class="worklist">
                            <div class="work">
                                <img src="img/imgweb.jpg">
                                <div class="layer">
                                    <h3> Web Design</h3>
                                    <p> A website created to suit your brand image.</p>
                                </div>
                            </div>
                            <div class="work">
                                <img src="img/img vid.jpg">
                                <div class="layer">
                                    <h3>Video Editing </h3>
                                    <p> Video shots are manipulated and arranged to perfection.</p>
                                </div>
                            </div>
                            <div class="work">
                                <img src="img/img content.jpg">
                                <div class="layer">
                                    <h3> Content Creation</h3>
                                    <p> Picture or video content is created for your brand for website display.</p>
                                </div>
                            </div>
                        </div>
                        <a href="#" class="btn">See more</a>

                    </div>
                </div>
                <!------------contact-------->
                <div class="contact">
                    <div class="container">
                        <div class="row">
                            <div class="contact-left">
                                <h1 class="sub-title">Contact Me</h1>
                                <p>sayadjoa@gmail.com</p>
                                <p>0555365903</p>
                            </div>
                            <div class="contact-right"></div>
                            <form>
                                <input type="text" name="Name" placeholder="Your Name" required>
                                <input type="email" name="email" placeholder="Your email" required>
                                <textarea name="Message" rows="6" placeholder="your message"></textarea>
                                <button type="submit" class="btn btn2">Submit</button>
                            </form>
                        </div>
                    </div>
                </div>
                <script>
                    var tablinks = document.getElementsByClassName("tab-links");
                    var tabcontents = document.getElementsByClassName("tab-contents");

                    function opentab(tabname) {
                        for (tablink of tablinks) {
                            tablink.classList.remove("active-link");

                        }
                        for (tabcontent of tabcontents) {
                            tabcontent.classList.remove("active-tab");
                        }
                        event.currentTarget.classList.add("active-link");
                        document.getElementById(tabname).classList.add("active-tab");
                    }
                </script>

</body>

</html>
