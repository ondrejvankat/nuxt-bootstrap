<template>
  <div class="col">
    <div class="card shadow-sm">
      <img :src="linkToImage"/>

      <div class="card-body">
        <p class="card-text">Pro otevření klikněte na "View"</p>
        <div class="d-flex justify-content-between align-items-center">
          <div class="btn-group">
            <button type="button" @click="onClick" class="btn btn-sm btn-outline-secondary">View</button>
          </div>
          <small class="text-muted">Youtube</small>
        </div>
      </div>
    </div>
  </div>
</template>
<script>

export default {
  props: {
    link:{
      required: true,
      type: String
    },
    linkToImage:{
      required: true,
      type: String
    }
  },
  methods: {
    onClick (){
    window.open(this.link);
    }
  }
}

</script>
