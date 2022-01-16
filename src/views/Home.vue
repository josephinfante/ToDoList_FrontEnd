<template>
  <div class="home">
    <h1 class="text-7xl font-black">Crea tus tareas</h1>
    <h3 class="text-2xl">Manten organizadas tus tareas</h3>
    <h5>asignandoles una categoria</h5>
    <div class="grid gap-4 grid-cols-2 my-10 w-1/3 mx-auto">
      <div class="place-self-center" v-for="t in tasks" :key="t.id">
        <TaskCard class="mx-5" :id="t.id" :task_name="t.name"/>
      </div>
    </div>
    <Button btn_link="/" btn_text="Comenzar"/>
  </div>
</template>

<script>
import TaskCard from '@/components/TaskCard';
import Button from '@/components/Button';
export default {
  name: 'Home',
  components: {
    TaskCard,
    Button
  },
  data() {
    return {
      tasks: [
        {
          id: 1,
          name: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
        },
        {
          id: 2,
          name: 'Etiam non quam lacus suspendisse faucibus.'
        },
        {
          id: 3,
          name: 'Sed pulvinar proin gravida hendrerit lectus a. Blandit aliquam.'
        },
        {
          id: 4,
          name: 'Ullamcorper eget nulla facilisi etiam dignissim diam quis.'
        }
      ]
    }
  }
}
</script>
