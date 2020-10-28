<template>
  <div>
    <div class="container-fluid">
      <div class="row">
        <nav id="sidebarMenu" class="col-md-3 col-lg-2 d-md-block bg-light sidebar collapse">
          <div class="sidebar-sticky pt-3">
            <ul class="nav flex-column">
              <li class="nav-item">
                <a class="nav-link" href="#">
                  <span data-feather="file"></span>
                  home
                </a>
              </li>
              <li class="nav-item">
                <a href="#what" @click="clickSmoothScroll('#what')">
                  <a class="nav-link" href="#what">
                    <span data-feather="what"></span>
                    What's Inovange
                  </a>
                </a>
              </li>
              <li class="nav-item">
                <a href="#members" @click="clickSmoothScroll('#members')">
                  <a class="nav-link" href="#members">
                    <span data-feather="file"></span>
                    members
                  </a>
                </a>
              </li>
              <li class="nav-item">
                <a href="#works" @click="clickSmoothScroll('#works')">
                  <a class="nav-link" href="#works">
                    <span data-feather="file"></span>
                    works
                  </a>
                </a>
              </li>
              <li class="nav-item">
                <a href="#contact" @click="clickSmoothScroll('#contact')">
                  <a class="nav-link" href="#contact">
                    <span data-feather="users"></span>
                    contact
                  </a>
                </a>
              </li>
            </ul>
          </div>
        </nav>
        <main role="main" class="col-md-9 ml-sm-auto col-lg-10 px-md-4">
          <div class="mx-auto" style="width: 200px;">
            <canvas class="my-4 w-100" id="myChartc" width="900" height="900"></canvas>
            <h1>Inovange</h1>
            <canvas class="my-4 w-100" id="myChartb" width="900" height="900"></canvas>
          </div>
          <h2 id="what">What's Inovange</h2>
          Inovangeとは令和２年９月１６日に富山県で結成されたクリエイティブチームのことである。メンバーは４人で...
          <canvas class="my-4 w-100" id="myChart" width="900" height="200"></canvas>
          <a href="#members" @click="clickSmoothScroll('#members')"></a>
          <h2 id="members">members</h2>
          <div class="card-deck">
            <div class="card">
              <div class="card-body">
                <h5 class="card-title">aさん</h5>
                <p class="card-text">This is a longer card with supporting text below as a natural lead-in to additional
                  content. This content is a little bit longer.</p>
                <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
              </div>
            </div>
            <div class="card">
              <div class="card-body">
                <h5 class="card-title">bさん</h5>
                <p class="card-text">This card has supporting text below as a natural lead-in to additional content.</p>
                <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
              </div>
            </div>
            <div class="card">
              <div class="card-body">
                <h5 class="card-title">cさん</h5>
                <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional
                  content. This card has even longer content than the first to show that equal height action.</p>
                <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
              </div>
            </div>
          </div>
          <div>
            <canvas class="my-4 w-100" id="myChart2" width="900" height="400"></canvas>
            <a href="#works" @click="clickSmoothScroll('#works')"></a>
            <h2 id="works">works</h2>
            <br><a href="https://www.amazon.co.jp/">2020.10.09完成</a>
            <br><a href="https://www.google.co.jp/">2020.10.10完成</a>
            <canvas class="my-4 w-100" id="myChart4" width="900" height="900"></canvas>
            <p class="example">
              <a href="#contact" @click="clickSmoothScroll('#contact')"></a>
            <h2 id="contact">contact</h2>
            <br>Inovange@sample.com
            <br>Inovange2@sample.com
            <br>Inovange3@sample.com
            </p>
            <canvas class="my-4 w-100" id="myChart5" width="900" height="300"></canvas>
          </div>
        </main>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    clickSmoothScroll (id) {
      event.preventDefault()
      this.$SmoothScroll(
        document.querySelector(id),
        400,
        null,
        null,
        'y'
      )
    }
  }
}
</script>

<style scoped>
body {
  font-size: .875rem;
}

.feather {
  width: 16px;
  height: 16px;
  vertical-align: text-bottom;
}

/*
 * Sidebar
 */

.sidebar {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  z-index: 100; /* Behind the navbar */
  padding: 48px 0 0; /* Height of navbar */
  box-shadow: inset -1px 0 0 rgba(0, 0, 0, .1);
}

@media (max-width: 767.98px) {
  .sidebar {
    top: 5rem;
  }
}

.sidebar-sticky {
  position: relative;
  top: 0;
  height: calc(100vh - 48px);
  padding-top: .5rem;
  overflow-x: hidden;
  overflow-y: auto; /* Scrollable contents if viewport is shorter than content. */
}

@supports ((position: -webkit-sticky) or (position: sticky)) {
  .sidebar-sticky {
    position: -webkit-sticky;
    position: sticky;
  }
}

.sidebar .nav-link {
  font-weight: 500;
  color: #333;
}

.sidebar .nav-link .feather {
  margin-right: 4px;
  color: #999;
}

.sidebar .nav-link.active {
  color: #007bff;
}

.sidebar .nav-link:hover .feather,
.sidebar .nav-link.active .feather {
  color: inherit;
}

.sidebar-heading {
  font-size: .75rem;
  text-transform: uppercase;
}

/*
 * Navbar
 */

.navbar-brand {
  padding-top: .75rem;
  padding-bottom: .75rem;
  font-size: 1rem;
  background-color: rgba(0, 0, 0, .25);
  box-shadow: inset -1px 0 0 rgba(0, 0, 0, .25);
}

.navbar .navbar-toggler {
  top: .25rem;
  right: 1rem;
}

.navbar .form-control {
  padding: .75rem 1rem;
  border-width: 0;
  border-radius: 0;
}

.form-control-dark {
  color: #fff;
  background-color: rgba(255, 255, 255, .1);
  border-color: rgba(255, 255, 255, .1);
}

.form-control-dark:focus {
  border-color: transparent;
  box-shadow: 0 0 0 3px rgba(255, 255, 255, .25);
}

.example {
  text-align: left;
  border: solid;
}
</style>
