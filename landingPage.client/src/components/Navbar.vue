<template>
  <nav
    class="navbar mainfont navbar-expand-lg fixed-top navbar-dark bg-dark px-3"
  >
    <router-link class="navbar-brand d-flex" :to="{ name: 'Home' }">
      <div class="d-flex flex-column align-items-center">
        <img
          href="#"
          class="rounded-circle hoverable"
          alt="logo"
          src="src\assets\img\Recurso 31MANDALA.svg"
          height="77"
        />
      </div>
    </router-link>
    <button
      class="navbar-toggler"
      type="button"
      data-bs-toggle="collapse"
      data-bs-target="#navbarText"
      aria-controls="navbarText"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon" />
    </button>
    <div
      style="z-index: 2"
      class="collapse col-2 navbar-collapse"
      id="navbarText"
    >
      <ul class="navbar-nav me-auto">
        <li class="d-flex justify-content-between align-items-end">
          <!-- <span
            href="#about"
            style="z-index: 2"
            class="
              btn
              mx-1
              p-1
              text-primary
              lighten-30
              hoverable2
              text-uppercase
            "
          >
            About
          </span> -->
          <span
            href="#contact"
            style="z-index: 2"
            class="
              textglow
              hoverable2
              btn
              p-1
              mx-1
              text-primary
              lighten-30
              hoverable2
              text-uppercase
            "
          >
            Contact
          </span>
          <a></a>
        </li>
      </ul>
      <span style="z-index: 0; width: 88vw" class="col-12">
        <img
          class="pulse"
          src="src\assets\img\Recurso 15MODERN ICON.svg"
          alt=""
        />
      </span>
      <!-- LOGIN COMPONENT HERE -->
      <Login hidden />
    </div>
  </nav>
</template>

<script>
export default {
  setup() {
    return {};
  },
};
</script>

<style scoped lang="scss">
a:hover {
  text-decoration: none;
}
.nav-link {
  text-transform: uppercase;
}
.navbar-nav .router-link-exact-active {
  border-bottom: 2px solid var(--bs-success);
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0;
}
.hoverable:hover {
  transform: scale(1.08);
  transform: rotate(360deg);
  filter: drop-shadow(0px 0px 15px rgb(63, 255, 98));
  transition: 500ms ease-in-out;
  cursor: pointer;
}
.hoverable:active {
  transform: scale(0.9);
  transition: 50ms ease-in-out;
}
img {
  transition: transform 0.7s ease-in-out;
}

.hoverable2:hover {
  filter: drop-shadow(0px 0px 5px rgb(63, 255, 98));
  transform: scale(1.05);
  transition: 150ms ease-in-out;
  cursor: pointer;
}
.hoverable2:active {
  transform: scale(0.95);
  transition: 10ms ease-in-out;
}
body {
  background: #000;
}
.pulse {
  filter: drop-shadow(0px 10px 10px rgb(61, 255, 54));
  animation: pulsate 3s ease-in-out infinite;
}
@keyframes pulsate {
  0% {
    filter: drop-shadow(0px 0px 5px rgba(50, 248, 43, 0.585));
  }
  10% {
    filter: drop-shadow(0px 0px 4.8px rgba(50, 248, 43, 0.562));
  }
  15% {
    filter: drop-shadow(0px 0px 5.2px rgba(50, 255, 57, 0.808));
  }
  25% {
    filter: drop-shadow(0px 0px 5.4px rgba(50, 255, 57, 0.926));
  }
  35% {
    filter: drop-shadow(0px 0px 5.6px rgba(50, 255, 95, 0.795));
  }
  45% {
    filter: drop-shadow(0px 0px 5.4px rgba(50, 255, 64, 0.696));
  }
  50% {
    filter: drop-shadow(0px 0px 5.8px rgba(50, 255, 53, 0.734));
  }
  60% {
    filter: drop-shadow(0px 0px 5.2px rgba(50, 255, 53, 0.601));
  }
  65% {
    filter: drop-shadow(0px 0px 5.4px rgba(50, 255, 53, 0.879));
  }
  75% {
    filter: drop-shadow(0px 0px 5.8px rgba(50, 255, 81, 0.715));
  }
  85% {
    filter: drop-shadow(0px 0px 5.4px rgba(50, 255, 67, 0.69));
  }
  95% {
    filter: drop-shadow(0px 0px 5px rgba(50, 255, 67, 0.603));
  }
  100% {
    filter: drop-shadow(0px 0px 5.2px rgba(50, 255, 84, 0.574));
  }
}
.mainfont {
  font-family: monospace;
}
p,
.textglow {
  max-width: 55vw;
  white-space: pre-line;
  letter-spacing: 0.1em;
  font-size: 1.1em;
  color: #05e110ce;
  filter: drop-shadow(0 0 2px #4aff3a7e);
}
</style>
