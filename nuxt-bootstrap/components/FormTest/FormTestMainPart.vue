<template>
  <main>

    <section class="py-5 text-center container">
      <div class="row py-lg-5">
        <div class="col-lg-6 col-md-8 mx-auto">
          <h1 class="fw-light">Test formulářů</h1>
        </div>
      </div>
    </section>

    <div class="album py-5 bg-light">
      <div class="container text-center">
        <form-test/>
      </div>
    </div>

  </main>
</template>

<script>
import FormTest from "~/components/FormTest/FormTest"

export default {
  components: {
    FormTest
  }
}

</script>
