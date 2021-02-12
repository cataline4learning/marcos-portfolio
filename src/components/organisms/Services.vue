<template>
  <div class="services">
    <Service
      title="Front End"
      description="Lorem, ipsum dolor sit amet consectetur adipisicing elit. Consectetur iste minima nam neque? Quam voluptatibus fugiat explicabo necessitatibus, maxime perspiciatis sed eaque sequi dolores nesciunt ducimus asperiores? Fugit, at accusamus."
    />

    <Service
      title="Back End"
      description="Lorem, ipsum dolor sit amet consectetur adipisicing elit. Consectetur iste minima nam neque? Quam voluptatibus fugiat explicabo necessitatibus, maxime perspiciatis sed eaque sequi dolores nesciunt ducimus asperiores? Fugit, at accusamus."
    />
    <Service
      title="Manutenção"
      description="Lorem, ipsum dolor sit amet consectetur adipisicing elit. Consectetur iste minima nam neque? Quam voluptatibus fugiat explicabo necessitatibus, maxime perspiciatis sed eaque sequi dolores nesciunt ducimus asperiores? Fugit, at accusamus."
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Service } from '@/components/molecules'

export default defineComponent({
  components: { Service }
})
</script>

<style lang="scss" scoped>
.services {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 5rem;
  @include screen('small', 'medium') {
    grid-template-columns: 1fr;
  }
}
</style>
