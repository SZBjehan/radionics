<template>
    <div class="Featured" id="Featured">
        <div class="intro-size">
            <div class="carousel">
                <div class="carousel-inner">
                    <input
                        class="carousel-open"
                        type="radio"
                        id="carousel-1"
                        name="carousel"
                        aria-hidden="true"
                        hidden=""
                        checked="checked"
                    />
                    <div class="carousel-item">
                        <a href=""
                            ><img class="ass" src="/images/landing1.jpg"
                        /></a>
                    </div>
                    <input
                        class="carousel-open"
                        type="radio"
                        id="carousel-2"
                        name="carousel"
                        aria-hidden="true"
                        hidden=""
                    />
                    <div class="carousel-item">
                        <a href=""
                            ><img class="ass" src="/images/landing2.jpg"
                        /></a>
                    </div>
                    <input
                        class="carousel-open"
                        type="radio"
                        id="carousel-3"
                        name="carousel"
                        aria-hidden="true"
                        hidden=""
                    />
                    <div class="carousel-item">
                        <a href=""
                            ><img class="ass" src="/images/landing3.png"
                        /></a>
                    </div>
                    <input
                        class="carousel-open"
                        type="radio"
                        id="carousel-4"
                        name="carousel"
                        aria-hidden="true"
                        hidden=""
                        checked="checked"
                    />
                    <div class="carousel-item">
                        <a href=""
                            ><img class="ass" src="/images/landingPage1.jpg"
                        /></a>
                    </div>
                    <input
                        class="carousel-open"
                        type="radio"
                        id="carousel-5"
                        name="carousel"
                        aria-hidden="true"
                        hidden=""
                        checked="checked"
                    />
                    <div class="carousel-item">
                        <a href=""
                            ><img class="ass" src="/images/landingPage3.jpg"
                        /></a>
                    </div>

                    <label
                        for="carousel-5"
                        class="carousel-control prev control-1"
                        >‹</label
                    >
                    <label
                        for="carousel-2"
                        class="carousel-control next control-1"
                        >›</label
                    >
                    <label
                        for="carousel-1"
                        class="carousel-control prev control-2"
                        >‹</label
                    >
                    <label
                        for="carousel-3"
                        class="carousel-control next control-2"
                        >›</label
                    >
                    <label
                        for="carousel-2"
                        class="carousel-control prev control-3"
                        >‹</label
                    >
                    <label
                        for="carousel-4"
                        class="carousel-control next control-3"
                        >›</label
                    >
                    <label
                        for="carousel-3"
                        class="carousel-control prev control-4"
                        >‹</label
                    >
                    <label
                        for="carousel-5"
                        class="carousel-control next control-4"
                        >›</label
                    >
                    <label
                        for="carousel-4"
                        class="carousel-control prev control-5"
                        >‹</label
                    >
                    <label
                        for="carousel-1"
                        class="carousel-control next control-5"
                        >›</label
                    >

                    <ol class="carousel-indicators">
                        <li>
                            <label for="carousel-1" class="carousel-bullet"
                                >•</label
                            >
                        </li>
                        <li>
                            <label for="carousel-2" class="carousel-bullet"
                                >•</label
                            >
                        </li>
                        <li>
                            <label for="carousel-3" class="carousel-bullet"
                                >•</label
                            >
                        </li>
                        <li>
                            <label for="carousel-4" class="carousel-bullet"
                                >•</label
                            >
                        </li>
                        <li>
                            <label for="carousel-5" class="carousel-bullet"
                                >•</label
                            >
                        </li>
                    </ol>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Intro"
};
</script>

<style>
.intro {
    overflow: hidden;
}
.intro-size {
    min-width: fit-content;
    max-height: 50%;
}

html,
body {
    margin: 0px;
    padding: 0px;
}

.carousel {
    position: relative;
    box-shadow: 0px 1px 6px rgba(0, 0, 0, 0.64);
    margin-top: 0.5px;
}

.carousel-inner {
    position: relative;
    overflow: hidden;
    width: 100%;
}

.carousel-open:checked + .carousel-item {
    position: static;
    opacity: 100;
}

.carousel-item {
    position: absolute;
    opacity: 0;
    -webkit-transition: opacity 0.6s ease-out;
    transition: opacity 0.6s ease-out;
    max-height: 400px;
}

.carousel-item img {
    display: block;
    height: auto;
    max-width: 100%;
}

.carousel-control {
    background: rgba(0, 0, 0, 0.28);
    border-radius: 50%;
    color: #fff;
    cursor: pointer;
    display: none;
    font-size: 40px;
    height: 40px;
    line-height: 35px;
    position: absolute;
    top: 50%;
    -webkit-transform: translate(0, -50%);
    cursor: pointer;
    -ms-transform: translate(0, -50%);
    transform: translate(0, -50%);
    text-align: center;
    width: 40px;
    z-index: 1;
}

.carousel-control.prev {
    left: 2%;
}

.carousel-control.next {
    right: 2%;
}

.carousel-control:hover {
    background: rgba(0, 0, 0, 0.8);
    color: #aaaaaa;
}

#carousel-1:checked ~ .control-1,
#carousel-2:checked ~ .control-2,
#carousel-3:checked ~ .control-3,
#carousel-4:checked ~ .control-4,
#carousel-5:checked ~ .control-5 {
    display: block;
}

.carousel-indicators {
    list-style: none;
    margin: 0;
    padding: 0;
    position: absolute;
    bottom: 2%;
    left: 0;
    right: 0;
    text-align: center;
    z-index: 1;
}

.carousel-indicators li {
    display: inline-block;
    margin: 0 5px;
}

.carousel-bullet {
    color: #fff;
    cursor: pointer;
    display: block;
    font-size: 35px;
}

.carousel-bullet:hover {
    color: #aaaaaa;
}

#carousel-1:checked
    ~ .control-1
    ~ .carousel-indicators
    li:nth-child(1)
    .carousel-bullet,
#carousel-2:checked
    ~ .control-2
    ~ .carousel-indicators
    li:nth-child(2)
    .carousel-bullet,
#carousel-3:checked
    ~ .control-3
    ~ .carousel-indicators
    li:nth-child(3)
    .carousel-bullet,
#carousel-4:checked
    ~ .control-4
    ~ .carousel-indicators
    li:nth-child(4)
    .carousel-bullet,
#carousel-5:checked
    ~ .control-5
    ~ .carousel-indicators
    li:nth-child(5)
    .carousel-bullet {
    color: #428bca;
}

#title {
    width: 100%;
    position: absolute;
    padding: 0px;
    margin: 0px auto;
    text-align: center;
    font-size: 27px;
    color: rgba(255, 255, 255, 1);
    font-family: "Open Sans", sans-serif;
    z-index: 9999;
    text-shadow: 0px 1px 2px rgba(0, 0, 0, 0.33),
        -1px 0px 2px rgba(255, 255, 255, 0);
}
</style>
