<template>
  <header>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container-fluid">
        <!-- Bootstrap 5 Navbar image and text https://getbootstrap.com/docs/5.3/components/navbar/#image-and-text -->
        <RouterLink class="navbar-brand" to="/">
          <img src="@/assets/logo.svg" alt="Logo" width="30" height="24" class="d-inline-block align-text-top">
          Vue 3
        </RouterLink>
        <!-- <a class="navbar-brand" href="#">
          <img src="@/assets/logo.svg" alt="Logo" width="30" height="24" class="d-inline-block align-text-top">
          Vue 3
        </a> -->
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <RouterLink class="nav-link" to="/"><span><i class="bi bi-house-door-fill"></i> Home</span>
              </RouterLink>
            </li>
            <li class="nav-item">
              <RouterLink class="nav-link p-2" to="/about">About</RouterLink>
            </li>
            <li class="nav-item">
              <RouterLink class="nav-link p-2" to="/bootstrap">Bootstrap</RouterLink>
            </li>
            <li class="nav-item">
              <RouterLink class="nav-link p-2" to="/default">Default</RouterLink>
            </li>
          </ul>
        </div>

      </div>
    </nav>
  </header>
</template>
