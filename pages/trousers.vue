    <template>
      <div class="clothrack">
        <h1 class="element-1">Get Some Trousers Today!</h1>
        <h1 class="element-1">Get Some Trousers Today!</h1>
        <div class="clothes">
                  <p><nuxt-link to="/shirts">Shirts</nuxt-link></p>
          <p><nuxt-link to="/trousers">Trousers</nuxt-link></p>
        </div>
      </div>
    </template>
        <script>
export default {
  asyncData () {
    return new Promise((resolve) => {
      setTimeout(function () {
        resolve({ name: 'world' })
      }, 1000)
    })
  }
}
</script>
