    <template>
      <div class="clothrack">
        <h1 class="element-1">Get a Shirt Today!</h1>
        <div class="clothes">
          <p><nuxt-link to="/shirts">Shirts</nuxt-link></p>
          <p><nuxt-link to="/trousers">Trousers</nuxt-link></p>
        </div>
      </div>
    </template>
    <script>
    import { TweenLite } from 'gsap'

    export default {
      asyncData () {
        return new Promise((resolve) => {
          setTimeout(function () {
            resolve({ name: 'world' })
          }, 1000)
        })
      },
    }
</script>
<script>
import { gsap } from 'gsap'
  export default {
    transition: {
      enter(el, done) {
        gsap.set(el, {
          autoAlpha: 0,
          yPercent: 50
      })
      gsap.to(el, {
        autoAlpha: .5,
        yPercent: 0,
        color: 'green',
        duration: .4
      })
      }
    }
  }
</script>
  
