# My-first-project
<section class="services">
    <div class="ser-txt">
        <h2>Services we offer</h2>
        <p>We offer a wide range of specialized services designed to meet your goals.</p>
    </div>
    <div class="ser-list">
        <ul>
            <li><a href="#service1">IT Services</a></li>
            <li><a href="#service2">Network Services</a></li>
            <li><a href="#service3">Technical Security</a></li>
            <li><a href="#service4">Digital Marketing</a></li>
            <li><a href="#service5">Cloud Services</a></li>
            <li><a href="#service6">Collaboration System</a></li>
            <li><a href="#service7">Certified Training</a></li>
        </ul>
    </div>

    <!-- Divs for each service content -->
    <div class="service-content" id="service1">
        <img src="path-to-your-image1.jpg" alt="IT Services">
        <div class="text">
            <p>Details about IT services...</p>
            <button>Learn More</button>
        </div>
    </div>
    <div class="service-content" id="service2">
        <img src="path-to-your-image2.jpg" alt="Network Services">
        <div class="text">
            <p>Details about Network services...</p>
            <button>Learn More</button>
        </div>
    </div>
    <div class="service-content" id="service3">
        <img src="path-to-your-image3.jpg" alt="Technical Security">
        <div class="text">
            <p>Details about Technical Security...</p>
            <button>Learn More</button>
        </div>
    </div>
    <!-- Add similar divs for other services -->
</section>


.css section
.services {
    display: flex;
    padding: 50px 15px;
    justify-content: space-between;
    align-items: flex-start;
}

.ser-list {
    flex: 1;
    display: flex;
    flex-direction: column;
    gap: 10px;
}

.ser-list ul {
    list-style-type: none;
    padding: 0;
}

.ser-list ul li {
    cursor: pointer;
    padding: 10px;
    background-color: #fff;
    border: 2px solid #ff1493;
    border-radius: 5px;
    transition: all 0.3s ease;
}

.ser-list ul li:hover {
    background-color: #ff1493;
    color: white;
}

.service-content {
    display: none; /* Hide by default */
    flex: 1;
    max-width: 500px;
    padding: 20px;
    background-color: #f4f4f4;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    transition: all 0.3s ease;
}

.service-content img {
    width: 100%;
    border-radius: 10px;
    object-fit: cover;
    max-height: 300px;
}

.service-content .text {
    margin-top: 20px;
}

.service-content button {
    background-color: #ff1493;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: all 0.3s ease;
}

.service-content button:hover {
    background-color: red;
}

/* Show the corresponding div when it's targeted */
.service-content:target {
    display: block;
}

/* Adjust for larger screens */
@media (min-width: 768px) {
    .services {
        flex-direction: row;
    }
}
