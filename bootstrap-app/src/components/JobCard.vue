<template>
  <div>
    <b-col>
        <b-card :title="name" 
        img-src="https://picsum.photos/600/300/?image=25"
        img-alt="Job-info"
        img-top
        tag="article"
        style="max-width:20rem"
        class="mb-2"
        footer="card-footer"
        >
        <b-card-text>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Odio, consequuntur?
        </b-card-text>
        <b-button variant="primary">Apply</b-button>
        </b-card>
    </b-col>
  </div>
</template>

<script>
export default {
    props: ['name']
}
</script>

<style>

</style>