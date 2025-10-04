<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <link rel="stylesheet" href="css/bootstrap.min.css">
  <link rel="stylesheet" href="css/index.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />
  <link rel="stylesheet" href="css/all.css">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.13.1/font/bootstrap-icons.min.css">
  <style>
   /* Common Styles */
.head {
  border: 1px solid #ddd;
  height: 80px;
  width: 100%;
  position: relative;
  align-items: center;
  justify-content: space-between;
}

.search-container {
  display: flex;
  align-items: center;
  border: 1px solid #ddd;
  border-radius: 50px;
  padding: 5px 15px;
  height: 40px;
  width: 260px;
  margin-left: 90px;
}

.search-container input {
  border: none;
  outline: none;
  font-size: 16px;
  padding: 8px;
  border-radius: 50px;
  width: 100%;
  height: 30px;
  border: 1px solid white;
}

.search-icon {
  margin-right: 10px;
  color: #ddd;
  font-size: 16px;
}

.mag {
  margin-left: 232px;
  font-size: 18px;
}

.fa-twitter {
  margin-left: 280px;
  cursor: pointer;
}

.fa-facebook, .fa-instagram {
  margin-left: 20px;
  cursor: pointer;
}

.sidebar {
  height: 100vh;
  width: 250px;
  background-color: white;
  position: fixed;
  top: 0;
  right: -250px;
  transition: right 0.3s ease;
  padding-top: 60px;
  z-index: 1000;
}

.sidebar .active {
  color: #F79918;
}

.sidebar.active {
  right: 0;
}

.sidebar a {
  padding: 4px 20px;
  text-decoration: none;
  display: block;
  color: black;
  font-size: 14px;
}

.sidebar a:hover {
  color: #f89b1c;
}

.cancel-icon {
  position: absolute;
  top: 10px;
  right: 15px;
  font-size: 25px;
  color: black;
  cursor: pointer;
}

.hamburger {
  font-size: 28px;
  margin-left: auto;
  cursor: pointer;
  color: black;
  display: block;
}

.subscribe-section {
  padding: 50px;
}

.subscribe-box {
  background-color: #f9fafb;
  padding: 40px;
  border-radius: 10px;
}

.subscribe-btn {
  background-color: #f89b1c;
  border: none;
  color: white;
  font-weight: bold;
  font-size: 11px;
  border-radius: 30px;
  padding: 12px 40px;
  transition: box-shadow 0.3s ease;
}

.subscribe-btn:hover {
  background-color: white;
  color: #f89b1c;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
}

.form-control {
  border-radius: 8px;
  padding: 12px;
}

.social-icon {
  background-color: #d1d1d1;
  width: 40px;
  height: 40px;
  border-radius: 16px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 5px;
  color: black;
  transition: all 0.3s ease;
}

.social-icon:hover {
  background-color: #F79918;
}

.social-icon:hover i {
  color: white;
}

.footer-links a {
  margin: 0 10px;
  text-decoration: none;
  color: gray;
  font-weight: 500;
}

.footer-links a:hover {
  color: black;
}

.footerr {
  text-align: center;
  padding: 40px 0;
  font-size: 14px;
  background-color: #fff;
}

/* Responsive Styles */

/* ≤1200px */
@media (max-width: 1200px) {
  .mag {
    margin-left: 40px !important;
  }

  .fa-twitter {
    margin-left: 80px !important;
  }
  .mostpop
  {
    width: auto;
  }
}

@media (max-width: 576px) {
  .image2,.image3,.image4,.image5,.image6,.image7
  {
    max-width: 100%;
    height: auto;
  }
  img, svg {
    vertical-align: middle;
}
  .img-fluid {
    max-width: 100%;
    height: auto;
}
  
}

/* ≤992px */
@media (max-width: 992px) {
  .d-flex.mt-5 {
    flex-direction: column !important;
    gap: 40px;
  }
  .search-container {
    width: 80% !important;
    max-width: 35%;
    margin-left: 0 !important;
    
  }

  .col-md-4,
  .col-md-5,
  .col-md-6,
  .col-md-7 {
    width: 100% !important;
    margin-left: 0 !important;
  }

  .mag {
    margin-left: 20px !important;
    text-align: center;
  }

  #row {
    display: block;
    text-align: left;
    order: 1;
  }

  #row i {
    margin-right: 10px;
  }

  .hamburger {
    position: absolute;
    top: 20px;
    right: 40px;
  }

  .head {
    flex-wrap: wrap;
    justify-content: center !important;
  }
   .img-fluid {
    max-width: 100%;
    height: auto !important;
}
  
}




/* ≤576px */
@media (max-width: 576px) {
  .head {
    flex-direction: column;
    height: auto;
    padding: 10px 10px !important;
    text-align: center;
  }
   .img2,.img3,.img4,.img5,.img6
  {
    max-width: 100%;
    height: auto !important;
  }
  .mostpop
  {
    width: auto;
  }
  

  .search-container {
    width: 80% !important;
    max-width: 100%;
    margin-left: 0 !important;
    justify-content: center;
    order: 3;
  }

  .search-container input {
    font-size: 14px;
  }

  .mag {
    font-size: 20px;
    margin: 0 !important;
    text-align: center;
    order: 1;
  }

  #row {
    width: 80%;
  }

  .fa-twitter,
  .fa-facebook,
  .fa-instagram {
    margin-left: 0 !important;
  }

  .hamburger {
    position: absolute;
    top: 50px;
    right: 40px;
  }

  .subscribe-section {
    padding: 5px;
  }
  
   .subscribe-section .d-flex {
     flex-direction: column !important;
     gap: 15px;
   }

   .subscribe-btn {
     width: 100% !important;
     padding: 12px 20px;
   }

  .footerr {
    font-size: 13px;
  }

  .footerr .d-flex.justify-content-center.mb-2 {
    flex-direction: column !important;
    align-items: center;
    gap: 10px;
  }

  .footer-links {
    display: flex;
    flex-direction: column;
    gap: 6px;
  }

  .footer-links a {
    margin: 0;
    text-align: center;
  }

  img {
    max-width: 100%;
    height: auto !important;
  }
}

/* ≤768px */
@media (max-width: 768px) {
  .head {
    flex-direction: column;
    height: auto;
    padding: 30px 10px !important;
    text-align: center;
  }
  .hamburger {
    position: absolute;
    top: 50px;
    right: 40px;
  }
    .mostpop
  {
    width: auto !important;
  }

   .img2,.img3,.img4,.img5,.img6,.img7
  {
    max-width: 100%;
    height: auto !important;
  }
  .search-container {
    width: 80% !important;
    max-width: 100%;
    margin-left: 0 !important;
    justify-content: center;
    order: 5;
    
  }

  .search-container input {
    font-size: 14px;
  }

  .mag {
    font-size: 20px;
    margin: 0 !important;
    text-align: center;
    order: 1;
  }
 #row {
    width: 80%;
  }

  .fa-twitter,
  .fa-facebook,
  .fa-instagram {
    margin-left: 0 !important;
    margin-bottom: 20 !important
  }

  .subscribe-section .d-flex {
    flex-direction: column !important;
    gap: 15px;
  }

  .form-control,
  .subscribe-btn {
    width: 100% !important;
  }

  .d-flex.mt-5,
  .d-flex.gap-3.mb-3 {
    flex-direction: column !important;
  }

  .footer-links a {
    display: block;
    margin: 8px 0;
  }
    .img-fluid {
    max-width: 100%;
    height: auto !important;
}
}


  </style>
</head>

<body>


  <!-- header Start -->
  <header class="head   d-flex px-5 py-3">
    <div class="search-container mt-1">
      <i class="fas fa-search search-icon"></i>
      <input type="text" placeholder="Search..." />
    </div>
    <h4 class="mag mt-3 fw-bold">MAGDESIGN</h4>
    <span id="row">
      <i class="fa-brands fa-twitter mt-2"></i>
      <i class="fa-brands fa-facebook mt-2"></i>
      <i class="fa-brands fa-instagram mt-2"></i>
    </span>

    <!-- Hamburger Icon -->
    <div class="hamburger" onclick="toggleSidebar()">&#9776;</div>

    <!-- Sidebar -->
    <div class="sidebar shadow" id="sidebar">
      <div class="cancel-icon" onclick="toggleSidebar()">&#10006;</div>
      <a href="#" class="home fw-bold active">Home</a>
      <a href="#" class="fw-bold">Categories</a>
      <a href="#" class="fw-bold">Travel</a>
      <a href="#" class="fw-bold">Food</a>
      <a href="#" class="fw-bold">Technology</a>
      <a href="#" class="fw-bold">Bussiness</a>
    </div>
    <script>
      function toggleSidebar() {
        const sidebar = document.getElementById("sidebar");
        sidebar.classList.toggle("active");
      }
    </script>
  </header>
  <!-- header End -->

  <!-- main -->
  <div class="container py-1">
    <h1 class="my-5 fw-bold text-center">Trending</h1>
    <div class="row">
      <div class="col-md-5">
        <img src="image/post_lg_1.jpg.webp" alt="" class="d-block w-100" style="height: 390px;border-radius:10px">
      </div>
      <div class="col-md-7 mt-4">
        <p class="fw-bold ms-3">Bussiness, Travel - July 2,2020 </p>
        <p class="h1 fw-bold ms-3">Your most unhappy <br>customers are your greatest source of learning.</p>
        <p class="ms-3 fw-bold" style="color:#949494;">Far far away, behind the word mountains, far from the countries
          Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast
          of the Semantics, a large language ocean.</p>
        <div class="d-flex author-info align-items-center">
          <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
            class="ms-3 flex-shrink-0">
          <span>
            <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
            <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
          </span>
        </div>
      </div>
    </div>

    <!-- main end -->


    <!-- 3 boxes -->

    <div class="d-flex mt-5">

      <div class="col-md-4">
        <div class="top"><img src="image/img_2.jpg.webp" alt="" style="height: 230px;border-radius: 10px;" class="img-fluid"></div>
        <div class="bottom">
          <p class="fw-bold mt-4 ms-1">Bussiness, Travel - July 2, 2020</p>
          <p class="fw-bold h5 ms-1">Your most unhappy customers are <br>your greatest source of learning.</p>
          <p class="ms-1" style="font-size: 14px;color: #949494;">Far far away, behind the word mountains, far <br>from
            the countries Vokalia and Consonantia, <br>there live the blind texts.</p>
          <div class="d-flex author-info align-items-center">
            <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
              class="flex-shrink-0">
            <span>
              <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
              <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
            </span>
          </div>
        </div>
      </div>

      <div class="col-md-4 ms-4">
        <div class="top"><img src="image/img_3.jpg.webp" alt="" style="height: 230px;border-radius: 10px;" class="img-fluid"></div>
        <div class="bottom">
          <p class="fw-bold mt-4 ms-1">Bussiness, Travel - July 2, 2020</p>
          <p class="fw-bold h5 ms-1">Your most unhappy customers are <br>your greatest source of learning.</p>
          <p class="ms-1" style="font-size: 14px;color: #949494;">Far far away, behind the word mountains, far <br>from
            the countries Vokalia and Consonantia, <br>there live the blind texts.</p>
          <div class="d-flex author-info align-items-center">
            <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
              class="flex-shrink-0">
            <span>
              <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
              <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
            </span>
          </div>
        </div>
      </div>


      <div class="col-md-4 ms-4">
        <div class="top"><img src="image/img_4.jpg.webp" alt="" style="height: 230px;border-radius: 10px;" class="img-fluid"></div>
        <div class="bottom">
          <p class="fw-bold mt-4 ms-1">Bussiness, Travel - July 2, 2020</p>
          <p class="fw-bold h5 ms-1">Your most unhappy customers are <br>your greatest source of learning.</p>
          <p class="ms-1" style="font-size: 14px;color: #949494;">Far far away, behind the word mountains, far <br>from
            the countries Vokalia and Consonantia, <br>there live the blind texts.</p>
          <div class="d-flex author-info align-items-center">
            <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
              class="flex-shrink-0">
            <span>
              <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
              <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
            </span>
          </div>
        </div>
      </div>

    </div>
    <!-- 3 boxes End -->


    <!-- 3 boxes -->
    <div class="d-flex mt-5">

      <div class="col-md-4 mb-5">
        <div class="top"><img src="image/img_4.jpg.webp" alt="" style="height: 230px;border-radius: 10px;" class="img-fluid"></div>
        <div class="bottom">
          <p class="fw-bold mt-4 ms-1">Bussiness, Travel - July 2, 2020</p>
          <p class="fw-bold h5 ms-1">Your most unhappy customers are <br>your greatest source of learning.</p>
          <p class="ms-1" style="font-size: 14px;color: #949494;">Far far away, behind the word mountains, far <br>from
            the countries Vokalia and Consonantia, <br>there live the blind texts.</p>
          <div class="d-flex author-info align-items-center">
            <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
              class="flex-shrink-0">
            <span>
              <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
              <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
            </span>
          </div>
        </div>
      </div>

      <div class="col-md-4 mb-5 ms-4">
        <div class="top"><img src="image/img_5.jpg.webp" alt="" style="height: 230px;border-radius: 10px;" class="img-fluid"></div>
        <div class="bottom">
          <p class="fw-bold mt-4 ms-1">Bussiness, Travel - July 2, 2020</p>
          <p class="fw-bold h5 ms-1">Your most unhappy customers are <br>your greatest source of learning.</p>
          <p class="ms-1" style="font-size: 14px;color: #949494;">Far far away, behind the word mountains, far <br>from
            the countries Vokalia and Consonantia, <br>there live the blind texts.</p>
          <div class="d-flex author-info align-items-center">
            <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
              class="flex-shrink-0">
            <span>
              <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
              <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
            </span>
          </div>
        </div>
      </div>

      <div class="col-md-4 mb-5 ms-4">
        <div class="top"><img src="image/img_6.jpg.webp" alt="" style="height: 230px;border-radius: 10px;" class="img-fluid"></div>
        <div class="bottom">
          <p class="fw-bold mt-4 ms-1">Bussiness, Travel - July 2, 2020</p>
          <p class="fw-bold h5 ms-1">Your most unhappy customers are <br>your greatest source of learning.</p>
          <p class="ms-1" style="font-size: 14px;color: #949494;">Far far away, behind the word mountains, far <br>from
            the countries Vokalia and Consonantia, <br>there live the blind texts.</p>
          <div class="d-flex author-info align-items-center">
            <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
              class="flex-shrink-0">
            <span>
              <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
              <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
            </span>
          </div>
        </div>
      </div>

    </div>
    <!-- 3 boxes end -->


    <!-- Most Popular Posts -->

    <div class="container py-5">
      <div class="mx-auto w-75">
        <h1 class="fw-bold text-center mt-5">Most Popular Posts</h1>
        <img src="image/img_7.jpg.webp" alt="" class="mostpop mt-5 w-100 rounded img-fluid">
        <div>
          <div class="bottom">
            <p class="fw-bold mt-3">Bussiness, Travel - July 2, 2020</p>
            <p class="fw-bold h5 gap-0">Your most unhappy customers are your greatest source of
              learning.</p>
            <p style="font-size: 14px;color: #949494;">Far far away, behind the word mountains, far
              from the countries Vokalia and Consonantia, there live the <br>blind texts.</p>
            <div class="d-flex author-info align-items-center">
              <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
                class="flex-shrink-0">
              <span>
                <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
                <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
              </span>
            </div>
          </div>
        </div>
      </div>

      <!-- Most Popular Posts End -->


      <!-- Sports -->
      <div class="container">
        <div class="row">
          <div class="col-md-6">
            <div class="left">
              <h3 class="mt-5 fw-bold">Sports</h3>
              <div class="d-flex gap-3 mb-3">
                <img src="image/img_2.jpg.webp" alt="" style="height: 100px;border-radius: 7px;" class="img2">
                <div>
                  <p class="fw-bold mb-1">Bussiness, Travel - July 2, 2020</p>
                  <p class="fw-bold h5 mb-2">Your most unhappy customers are
                    <br>your greatest source of learning.
                  </p>
                  <div class="d-flex author-info align-items-center">
                    <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
                      class="flex-shrink-0">
                    <span>
                      <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
                      <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
                    </span>
                  </div>
                </div>
              </div>
              <div class="d-flex gap-3 mb-3">
                <img src="image/img_3.jpg.webp" alt="" style="height: 100px;border-radius: 7px;" class="img3">
                <div>
                  <p class="fw-bold mb-1">Bussiness, Travel - July 2, 2020</p>
                  <p class="fw-bold h5 mb-2">Your most unhappy customers are
                    <br>your greatest source of learning.
                  </p>
                  <div class="d-flex author-info align-items-center">
                    <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
                      class=" flex-shrink-0">
                    <span>
                      <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
                      <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
                    </span>
                  </div>
                </div>
              </div>
              <div class="d-flex gap-3 mb-3">
                <img src="image/img_4.jpg.webp" alt="" style="height: 100px;border-radius: 7px;" class="img4">
                <div>
                  <p class="fw-bold mb-1">Bussiness, Travel - July 2, 2020</p>
                  <p class="fw-bold h5 mb-2">Your most unhappy customers are
                    <br>your greatest source of learning.
                  </p>
                  <div class="d-flex author-info align-items-center">
                    <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
                      class=" flex-shrink-0">
                    <span>
                      <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
                      <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
                    </span>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <!-- Sport End -->

          <!-- Bussiness -->

          <div class="col-md-6">
            <h3 class="mt-5 fw-bold">Bussiness</h3>
            <div class="d-flex gap-3 mb-3">
              <img src="image/img_2.jpg.webp" alt="" style="height: 100px;border-radius: 7px;" class="img5">
              <div>
                <p class="fw-bold mb-1">Bussiness, Travel - July 2, 2020</p>
                <p class="fw-bold h5 mb-2">Your most unhappy customers are
                  <br>your greatest source of learning.
                </p>
                <div class="d-flex author-info align-items-center">
                  <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
                    class=" flex-shrink-0">
                  <span>
                    <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
                    <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
                  </span>
                </div>
              </div>
            </div>

            <div class="d-flex gap-3 mb-3">
              <img src="image/img_3.jpg.webp" alt="" style="height: 100px;border-radius: 7px;" class="img6">
              <div>
                <p class="fw-bold mb-1">Bussiness, Travel - July 2, 2020</p>
                <p class="fw-bold h5 mb-2">Your most unhappy customers are
                  <br>your greatest source of learning.
                </p>
                <div class="d-flex author-info align-items-center">
                  <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
                    class=" flex-shrink-0">
                  <span>
                    <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
                    <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
                  </span>
                </div>
              </div>
            </div>

            <div class="d-flex gap-3 mb-3">
              <img src="image/img_4.jpg.webp" alt="" style="height: 100px;border-radius: 7px;" class="img7">
              <div>
                <p class="fw-bold mb-1">Bussiness, Travel - July 2, 2020</p>
                <p class="fw-bold h5 mb-2">Your most unhappy customers are
                  <br>your greatest source of learning.
                </p>
                <div class="d-flex author-info align-items-center">
                  <img src="image/person_1.jpg.webp" alt="" style="height: 45px;border-radius: 20px;width: 45px;"
                    class=" flex-shrink-0">
                  <span>
                    <p class="fw-bold mb-0 ms-2">Sergy Campbell</p>
                    <p style="font-size: 14px;color: #949494;" class="ms-2 mb-0">Author, 26 published post</p>
                  </span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div>
      </div>
      <!-- Bussiness End -->


      <!-- footer -->
      <section class="subscribe-section">
        <div class="container subscribe-box">
          <h5 class="fw-bold mb-3 text-center">Subscribe to newsletter</h5>
          <div class="d-flex flex-column">
            <input type="email" class="form-control me-3 mb-4" placeholder="Enter your email">
            <button class="subscribe-btn mx-auto w-25">SUBSCRIBE</button>
          </div>
        </div>
      </section>

      <!-- footer end -->

      <!-- last -->

      <footer class="footerr mt-3">
        <!-- Social Icons -->
        <div class="row justify-content-center mb-2">
          <a href="#" class="social-icon"><i class="bi bi-facebook"></i></a>
          <a href="#" class="social-icon"><i class="bi bi-twitter"></i></a>
          <a href="#" class="social-icon"><i class="bi bi-linkedin"></i></a>
          <a href="#" class="social-icon"><i class="bi bi-youtube"></i></a>
        </div>

        <!-- Copyright -->
        <p class="text-muted mt-4">
          Copyright ©2025 All rights reserved | This template is made with
          <span style="color: red;">❤</span> by
          <a href="https://colorlib.com" class="text-decoration-underline text-muted">Colorlib</a>
        </p>

        <!-- Terms & Conditions and Privacy Policy -->
        <div class="footer-links mt-4">
          <a href="#">Terms & Conditions</a> /
          <a href="#">Privacy Policy</a>
        </div>
      </footer>



    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
