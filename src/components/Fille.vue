 <template>
  <div class="col-lg-4">
    <a href="#">
      <img
        :src="require(`@/assets/${image}`)"
        width="300"
        height="400"
        class="img-fluid"
        alt="..."
        bg-image
        hover-overlay
      />
    </a>
    <h5 class="titre">{{ titre }}</h5>
    <p>{{ description }}</p>
    <span>{{ prix }}</span>
  </div>
</template>

<script>


export default {
  name: 'Filles',
  props: {
    titre: String,
    image: String,
    prix: String,
    description: String

  }
}
</script>