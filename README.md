@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;400;500;900&display=swap');

:root {
    --primary: #48CAE4;
    --normal: #ffffff;
    --black: #13131a;
    --bg: #0c1013;
    --danger: #f75842;
    --border: 0.1rem solid rgba(255, 255, 255, 0.3);


    --container-width-lg: 80%;
    --container-width-md: 90%;
    --container-width-sm: 94%;
}

/* Universal selector  */
* {
    font-family: 'Roboto', sans-serif;
    margin: 0;
    padding: 0;
    outline-offset: none;
    border: none;
    box-sizing: border-box;
    text-decoration: none;
    list-style: none;
    transition: all 0.5s linear;
    scroll-behavior: smooth;
}

/* Custom Scroll bar */
::-webkit-scrollbar {
    width: 10px;
}

::-webkit-scrollbar-track {
    background: var(--normal);
}

::-webkit-scrollbar-thumb {
    background: var(--black);
}

::-webkit-scrollbar-thumb:hover {
    background: var(--danger);
}

body {
    line-height: 1.7;
    color: var(--normal);
    background-color: var(--bg);
}

.container {
    width: var(--container-width-lg);
    margin: 0 auto;
}

section {
    padding: 6rem 0;
}

section h2 {
    text-align: center;
    margin-bottom: 4rem;
}

h1,
h2,
h3,
h4 {
    line-height: 1.2;
}

h1 {
    font-size: 2.4rem;
}

h2 {
    font-size: 2rem;
}

h3 {
    font-size: 1.6rem;
}

h4 {
    font-size: 1.3rem;
}

a {
    color: var(--normal);
}

img {
    width: 100%;
    display: block;
    object-fit: cover;
}

.btn {
    display: inline-block;
    background-color: var(--primary);
    color: var(--black);
    padding: 0.5rem 2rem;
    border: 1px solid transparent;
    border-radius: 0.3rem;
    font-weight: 500;
}

.btn:hover {
    color: var(--primary);
    background-color: transparent;
    border-color: var(--primary);
}

.border_bottom {
    text-align: center;
    display: inline-block;
    border-bottom: 2px solid var(--primary);
    color: var(--primary);
    margin-bottom: 2.5rem;
}

nav {
    background-color: var(--black);
    width: 100vw;
    height: 5rem;
    position: fixed;
    top: 0;
    z-index: 1000;
}

.window-scroll{
    background-color:#0c1013f1;
}

.nav_container {
    display: flex;
    height: 100%;
    justify-content: space-between;
    align-items: center;
}

.nav_container span {
    color: var(--primary);
}

.nav_container h4 {
    font-size: 1.8rem;
}

.nav_container h4::first-letter {
    font-size: 2rem;
}

.nav_container h4:hover {
    color: var(--primary);
    transform: rotateX(360deg);
    transition-duration: 1.2s;
}

nav button {
    display: none;
}

.nav_menu {
    display: flex;
    align-items: center;
    gap: 3rem;
}

.nav_menu a {
    font-size: 1rem;
}

.nav_menu a:hover {
    color: var(--primary);
    border-bottom: 3px solid var(--primary);
    padding-bottom: 0.8rem;
    background-color: var(--black);
}

/* ======HEADER======= */

header {
    position: relative;
    top: 5rem;
    overflow: hidden;
    margin-bottom: 2rem;
    background-color: var(--black);
}

.header_container {
    display: flex;
    align-items: center;
    position: relative;
}

.header_left {
    flex: 1;
}

.header_right {
    flex: 1;
}

.header_left_img {
   width: 75%;
   border: 1px solid rgba(0, 0, 0, 0.5);
   border-radius: 50%;
}


.header_right .text-1 {
    font-size: 1.8rem;
    margin-bottom: 0.3rem;
}

.header_right .text-2 {
    font-size: 3.6rem;
    font-weight: 550;
}

.header_right .text-3 {
    font-size: 2.5rem;
    margin: 0.3rem 0;
}

.header_left_img img {
    border-radius: 50%;
}

/* header::before {
    content: "";
    position: absolute;
    background-color: var(--bg);
    width: 100%;
    height: 5rem;
    bottom: 0;
    margin-bottom: -3.1rem;
    z-index: 99;
    transform: skewY(-2deg);
    transform-origin: left;
} */

.header_right .typing {
    color: var(--primary);
    font-weight: 500;
}

/* ======ABOUT ME======= */

.about {
    text-align: center;
}

.about_container {
    display: flex;
    margin: auto;
    align-items: center;
    justify-content: center;
    position: relative;
    margin-bottom: 2.5rem;
}

.about_container .about-img {
    border: 1px solid var(--primary);
    border-radius: 50%;
    overflow: hidden;
    max-width: 12.5rem;
    max-height: 12.5rem;
    margin-right: 2rem;
    position: relative;
    align-items: center;
    margin-bottom: 2rem;
}

.about_container .about-text {
    max-width: 70%;
    text-align: justify;
    line-height: 1.5rem;
    letter-spacing: 0.5px;
    padding-bottom: 2.5rem;
}

.about_container .about-text p {
    margin-bottom: 0.8rem;
}

.about_container .about-text .text {
    margin-bottom: 1rem;
}

.about_container .about-text .text span {
    color: var(--primary);
    font-weight: 500;
}

/* ======SERVICES======= */
.services {
    text-align: center;
    margin-top: -5rem;
}

.services_container .cards {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    justify-content: space-between;
    align-items: center;
    margin-bottom: 3rem;
}

.services_container .cards .card {
    background-color: var(--primary);
    padding: 1.5rem 1rem;
    margin: 0 1.5rem;
    cursor: pointer;
    position: relative;
}

.sbox i {
    font-size: 2rem;
    width: 4rem;
    height: 4rem;
    color: var(--bg);
    border: 1px solid rgba(0, 0, 0, 0.5);
    border-radius: 50%;
    padding: 14px;
    transition: all 1s;
}

.sbox h3 {
    font-size: 1.2rem;
    color: var(--black);
}

.sbox p {
    margin: 1.2rem 0;
    color: var(--bg);
}

.sbox a {
    color: var(--normal);
    font-size: 1.2rem;
    font-weight: 500;
    padding: 0.3rem 1rem;
    background-color: var(--bg);
    border-radius: 1rem;
}

.sbox a:hover {
    background-color: var(--normal);
    color: var(--bg);
    border: 1px solid var(--bg);
}

.services_container .cards .card:hover .sbox i {
    background-color: var(--bg);
    color: var(--normal);
}

.services_container .cards .card::after {
    content: "";
    height: 100%;
    width: 100%;
    background-color: var(--normal);
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1;
    transition: all 0.5s;
}

.services_container .cards .card:hover::after {
    transform: rotate(13deg);
}

/* ======SKILLS======= */
.skills .new {
    text-align: center;
}

.skills_container {
    display: flex;
    margin: auto;
    position: relative;
    flex-direction: column;
    padding: 1.6rem 1.8rem;
    max-width: 40rem;
    background-color: var(--black);
    border-radius: 0.7rem;
    box-shadow: 0.3rem 0.3rem 1.2rem rgba(0, 0, 0, 0.2);
}

.skills_container .bar {
    margin: 1.2rem 0;
}

.skills_container .bar:first-child {
    margin-top: 0rem;
}

.skills_container .bar .info {
    margin-bottom: 0.3rem;
}

.skills_container .bar .info span {
    font-weight: 500;
    font-size: 1rem;
    opacity: 0;
    animation: showText 0.5s 1s linear forwards;
}

@keyframes showText {
    100% {
        opacity: 1;
    }
}

.skills_container .bar .progress-line {
    height: 10px;
    width: 100%;
    background-color: var(--normal);
    position: relative;
    transform: scaleX(0);
    transform-origin: left;
    border-radius: 0.7rem;
    box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05), 0 1px rgba(255, 255, 255, 0.8);
    animation: animate 1s cubic-bezier(1, 0, 0.5, 1) forwards;
}

@keyframes animate {
    100% {
        transform: scaleX(1);
    }
}

.bar .progress-line span {
    height: 100%;
    position: absolute;
    border-radius: 0.7rem;
    transform: scaleX(0);
    transform-origin: left;
    background-color: var(--primary);
    animation: animate 1s 3s cubic-bezier(1, 0, 0.5, 1) forwards;
}

.bar .progress-line.html span {
    width: 90%;
}

.bar .progress-line.python span {
    width: 90%;
}

.bar .progress-line.mysql span {
    width: 60%;
}

.progress-line span::before {
    position: absolute;
    content: "";
    top: -0.7rem;
    right: 0;
    height: 0;
    width: 0;
    border: 0.5rem solid transparent;
    border-bottom-width: 0rem;
    border-right-width: 0rem;
    border-top-color: var(--bg);
    opacity: 0;
    animation: showText2 0.5s 1s linear forwards;
}

.progress-line span::after {
    position: absolute;
    top: -1.8rem;
    right: 0;
    font-weight: 500;
    background: #000;
    color: #fff;
    padding: 1px 0.5rem;
    font-size: 0.7rem;
    border-radius: 0.2rem;
    opacity: 0;
    animation: showText2 0.5s 1s linear forwards;
}


@keyframes showText2 {
    100% {
        opacity: 1;
    }
}

.progress-line.html span::after {
    content: "90%";
}

.progress-line.python span::after {
    content: "90%";
}

.progress-line.mysql span::after {
    content: "60%";
}

/* =======PORTFOLIO======= */

.portfolio_container {
    text-align: center;
    margin-top: 3rem;
}

.gallery {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    margin: 0 auto;
    margin-bottom: 3rem;
    background-color: var(--black);
    border-radius: 2rem;
}

.gallery a {
    height: 15rem;
    width: 20rem;
    margin: 1.2rem;
    border-radius: 0.3rem;
    overflow: hidden;
    box-shadow: 0 3px 5px var(--primary);
}

.gallery a img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.gallery a img:hover {
    transform: scale(1.4);
}

/* ======COURSES======= */
.courses {
    text-align: center;
    margin-top: 3rem;
}

.courses_container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
}

.course {
    background-color: var(--black);
    text-align: center;
    border: 1px solid transparent;
}

.course:hover {
    border-color: var(--primary);
    background: transparent;
}

.course_info {
    padding: 2rem;
}

.course_info p {
    margin: 1.2rem 0 2rem;
    font-size: 0.9rem;
}

/* ======FAQs SECTION======= */
.faqs {
    text-align: center;
    margin-top: 2rem;
}

.faqs_container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
    background-color: var(--black);
    box-shadow: inset 0 0 3rem rgba(0, 0, 0, 0.5);
}

.faq {
    padding: 2rem;
    margin: 1rem;
    display: flex;
    align-items: center;
    gap: 1.4rem;
    height: fit-content;
    background-color: var(--primary);
    color: var(--bg);
    text-align: justify;
    cursor: pointer;
    border-radius: 1rem;
}

.faq h4 {
    font-size: 1rem;
    line-height: 2.23;
}

.faq_icon {
    align-self: flex-start;
    font-size: 1.3rem;
}

.faq p {
    margin-top: 0.8rem;
    display: none;
}

/* for showing ans on click */
.faq.open p {
    display: block;
}

/* ======Footer SECTION======= */
footer {
    padding-top: 5rem;
    background-color: var(--black);
    font-size: 0.9rem;
}

.footer_container {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 5rem;
}

.footer_container>div h4 {
    margin-bottom: 1.2rem;
}

.footer_1 p {
    margin: 0 0 2rem;
}

footer ul li {
    margin-bottom: 0.7rem;
}

footer ul li a:hover {
    text-decoration: underline;
    color: var(--primary);
}

.footer_4 .mail {
    text-transform: lowercase;
}

.footer_social {
    display: flex;
    gap: 1rem;
    font-size: 1.2rem;
    margin-top: 2rem;
}

.footer_copyright {
    text-align: center;
    margin-top: 4rem;
    padding: 1.2rem 0;
    border-top: 1px solid var(--normal);
}

/* ======MEDIA QUERIES (TABLETS)======= */

@media screen and (max-width:1024px) {
    .container {
        width: var(--container-width-md);
    }

    h1 {
        font-size: 2.2rem;
    }

    h2 {
        font-size: 1.7rem;
    }

    h3 {
        font-size: 1.4rem;
    }

    h4 {
        font-size: 1.2rem;
    }

    .header_right .text-1 {
        font-size: 1.2rem;
    }

    .header_right .text-2 {
        font-size: 2rem;
    }

    .header_right .text-3 {
        font-size: 1.5rem;
    }

    .header_right .typing {
        font-weight: 450;
    }

    .btn {
        padding: 0.3rem 1.2rem;
    }

    /* ======NAVBAR OPEN======= */
    nav button {
        display: inline-block;
        background: transparent;
        font-size: 1.8rem;
        color: var(--normal);
        cursor: pointer;
    }

    nav button#close-menu-btn {
        display: none;
    }

    .nav_menu {
        position: fixed;
        top: 5rem;
        right: 5%;
        gap: 0;
        height: fit-content;
        width: 18rem;
        flex-direction: column;
        display: none;
        /* we will display with js  */
    }

    .nav_menu li{
        width: 100%;
        height: 3rem;
        animation: animateNavItems 0.2s linear forwards;
        transform-origin: top right;
        opacity: 0;
    }
    .nav_menu li a{
        background-color: var(--primary);
        box-shadow: -4rem 6rem 10rem rgba(0,0,0,0.6);
        width: 100%;
        height: 100%;
        display: grid;
        color: var(--bg);
        place-items: center;
    }

    .nav_menu li:nth-child(2){
        animation-delay: 0.2s;
    }
    .nav_menu li:nth-child(3){
        animation-delay: 0.4s;
    }
    .nav_menu li:nth-child(4){
        animation-delay: 0.6s;
    }
    .nav_menu li:nth-child(5){
        animation-delay: 0.8s;
    }
    .nav_menu li:nth-child(6){
        animation-delay: 1s;
    }
    .nav_menu li:nth-child(7){
        animation-delay: 1.2s;
    }
    
    @keyframes animateNavItems {
        0%{
            transform: rotateZ(-90deg);
        }
        100%{
            transform: rotateZ(0);
            opacity: 1;
        }
    }

    .services_container .cards {
        row-gap: 1rem;
        grid-template-columns: repeat(2, 1fr);
    }
    
    .services_container .cards .card {
       padding: 2rem 0.3rem;
       margin: 0 0.5rem;
    }
    .services_container .cards .card:hover::after {
        transform: rotate(5deg);
    }
    .gallery a {
        height: 14rem;
        width: 18rem;
        margin: 1.2rem;
        border-radius: 0.3rem;
        overflow: hidden;
        box-shadow: 0 3px 5px var(--primary);
    }

    .gallery video {
        height: 14rem;
        width: 18rem;
        margin: 1.2rem;
        border-radius: 0.3rem;
        overflow: hidden;
        box-shadow: 0 3px 5px var(--primary);
    }

    .courses_container{
        grid-template-columns: repeat(2,1fr);
    }
    
    .faqs_container{
        grid-template-columns: 1fr;
    }
    .faq{
        padding: 1.5rem;
    }
    .footer_container{
        grid-template-columns: repeat(2,1fr);
    }
}

/* ========MEDIA QUERIES (MOBILE)======== */
@media screen and (max-width:600px) {
    .container{
        width: var(--container-width-sm);
    }    
    .nav_menu{
        right: 3%;
    }

    .about_container .about-img {
        margin-right: 0rem;
    }

    .header_right .text-1 {
        font-size: 1rem;
    }

    .header_right .text-2 {
        font-size: 1.2rem;
    }

    .header_right .text-3 {
        font-size: 1.2rem;
    }
    .header_right a{
        margin-bottom: 0.3rem;
    }

    .btn {
        padding: 0.3rem 1rem;
    }

    .about_container{
        flex-direction: column;
    }
    .services_container .cards {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-bottom: 3rem;
    }
    
    .services_container .cards .card {
       padding: 3rem 1rem;
       margin: 1rem 1rem;
    }
    .services_container .cards .card:hover::after {
        transform: rotate(5deg);
    }

    .gallery a{
        width: 25rem;
    }

    .courses_container{
        grid-template-columns: 1fr;
        width: 80%;
    }

    .courses_container .course{
        margin-bottom: 1rem;
    }

    .footer_container{
        grid-template-columns: 1fr;
        text-align: center;
        gap: 2rem;
    }

    .footer_social{
        justify-content: center;
    }
}
