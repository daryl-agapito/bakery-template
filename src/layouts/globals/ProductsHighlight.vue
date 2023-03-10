<script>
import Card from '../../components/homepage/Card.vue'
import BaseButton from '../../components/homepage/BaseButton.vue'

export default {
  components: {
    Card,
    BaseButton
  },
  data() {
    return {
      productsButton: {
        description: 'View all products',
        link: '#'
      },
      storedResources: [
        {
          id: 'cupcake',
          title: 'Velvet Cupcake',
          description:
            'Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui alias animi maiores hic, recusandae ducimus laudantium molestias aliquid veritatis nisi.',
          imageLink:
            'https://images.unsplash.com/photo-1614707267537-b85aaf00c4b7?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=774&q=80'
        },
        {
          id: 'cupcake2',
          title: 'Almond Cupcake',
          description:
            'Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui alias animi maiores hic, recusandae ducimus laudantium molestias aliquid veritatis nisi.',
          imageLink:
            'https://images.unsplash.com/photo-1603532648955-039310d9ed75?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8OHx8Y3VwY2FrZXxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60'
        },
        {
          id: 'cake1',
          title: 'Cake',
          description:
            'Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui alias animi maiores hic, recusandae ducimus laudantium molestias aliquid veritatis nisi.',
          imageLink:
            'https://images.unsplash.com/photo-1627834377411-8da5f4f09de8?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=802&q=80'
        },
        {
          id: 'cake2',
          title: 'Cake Slice',
          description:
            'Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui alias animi maiores hic, recusandae ducimus laudantium molestias aliquid veritatis nisi.',
          imageLink:
            'https://images.unsplash.com/photo-1575919361890-69028a013637?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=774&q=80'
        }
      ]
    }
  }
}
</script>

<template>
  <section class="content-wrapper">
    <div class="container mx-auto">
      <div class="mx-auto text-center b--spacer">
        <h2>Our latest bakery products</h2>
        <p>Check some of our best products and feel the great passion for food.</p>
      </div>

      <div class="grid md:grid-cols-4 gap-6 mx-auto">
        <Card
          v-for="res in storedResources"
          :title="res.title"
          :imageLink="res.imageLink"
          :description="res.description"
        >
        </Card>
      </div>
      <BaseButton :buttonDesc="productsButton.description" :buttonLink="productsButton.link" />
    </div>
  </section>
</template>
