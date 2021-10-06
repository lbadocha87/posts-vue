<template>
    <div>
        <h2>{{post.id}} {{post.title}}</h2>
        <p>{{post.body}}</p>
    </div>
</template>

<script>
export default {
  name: 'PostItem',
  props: ['post']
}
</script>
