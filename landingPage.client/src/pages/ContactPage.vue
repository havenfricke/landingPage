<template>
  <div class="container-fluid">
    <div class="row mt-5 d-flex justify-content-center pt-5">
      <div class="col-10 mt-5 border border-primary p-5">
        <span class="row justify-content-center">
          <p class="fs-1 col-12 mainfont text-center textglow">Contact Form</p>
        </span>

        <form
          class=""
          action="https://formsubmit.co/c830d841a364c6255e3cac86fcd4529a"
          method="POST"
        >
          <div class="row justify-content-around">
            <input
              class="
                bg-black
                mx-1
                col-5
                p-2
                border border-primary
                mainfont
                textglow
              "
              type="text"
              name="name"
              placeholder="Name..."
              required
            />
            <input
              class="
                mx-1
                bg-black
                col-5
                p-2
                border border-primary
                mainfont
                textglow
              "
              type="email"
              name="email"
              placeholder="your@email.com"
              required
            />
          </div>
          <textarea
            class="
              col-12
              p-1
              border border-primary
              mt-5
              text-primary
              textglow
              mainfont
              bg-black
            "
            placeholder="Write a message..."
            name="message"
            type="message"
            id=""
            cols="30"
            rows="10"
          ></textarea>
          <div class="row justify-content-end mx-3">
            <button
              class="
                mt-5
                bg-black
                text-primary
                textglow
                mainfont
                border border-primary
                col-2
                hoverable
              "
              type="submit"
            >
              Send
            </button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Contact',
  setup() {
    return {}
  }
}
</script>

<style scoped>
.textglow {
  white-space: pre-line;
  letter-spacing: 0.1em;
  font-size: 1.1em;
  color: #05e110ce;
  filter: drop-shadow(0 0 2px #4aff3a7e);
}
.mainfont {
  font-family: monospace;
}
.hoverable:hover {
  transform: scale(1.08);
  filter: drop-shadow(0px 0px 15px rgb(63, 255, 98));
  transition: 500ms ease-in-out;
  cursor: pointer;
}
.hoverable:active {
  transform: scale(0.9);
  transition: 50ms ease-in-out;
}
</style>