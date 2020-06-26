<template>
    <div id="particles-js">
        <div id="home" class="home_title">
            <img src="../assets/profile.png" alt="" class="my_home_pic">
            <h1>Welcome to my Portfolio page</h1>
            <a href="https://twitter.com/SunamiJun" class="btn-twitter">
              <font-awesome-icon :icon="['fab', 'twitter']"  size="3x"/>
            </a>
            <a href="https://github.com/junsunami" class="btn-github">
              <font-awesome-icon :icon="['fab', 'github']" size="3x" />
            </a>
        </div>
    </div>
</template>

<script>
export default {
  name: 'ParticlesJS',

  mounted () {
    require('particles.js')
    this.$nextTick(() => {
      this.initParticlesJS()
    })
  },

  methods: {
    initParticlesJS () {
      /* eslint-disable */
      particlesJS('particles-js', {
        'particles': {
          'number': {
            'value': 80,
            'density': {
              'enable': true,
              'value_area': 800
            }
          },
          'color': {
            'value': '#ffffff'
          },
          'shape': {
            'type': 'circle',
            'stroke': {
              'width': 0,
              'color': '#000000'
            },
            'polygon': {
              'nb_sides': 5
            },
            'image': {
              'src': 'img/github.svg',
              'width': 100,
              'height': 100
            }
          },
          'opacity': {
            'value': 0.5,
            'random': false,
            'anim': {
              'enable': false,
              'speed': 0.5,
              'opacity_min': 0.1,
              'sync': false
            }
          },
          'size': {
            'value': 10,
            'random': true,
            'anim': {
              'enable': false,
              'speed': 80,
              'size_min': 0.1,
              'sync': false
            }
          },
          'line_linked': {
            'enable': true,
            'distance': 150,
            'color': '#ffffff',
            'opacity': 0.4,
            'width': 1
          },
          'move': {
            'enable': true,
            'speed': 6,
            'direction': 'none',
            'random': false,
            'straight': false,
            'out_mode': 'out',
            'bounce': false,
            'attract': {
              'enable': false,
              'rotateX': 600,
              'rotateY': 1200
            }
          }
        },
        'interactivity': {
          'detect_on': 'canvas',
          'events': {
            'onhover': {
              'enable': true,
              'mode': 'repulse'
            },
            'onclick': {
              'enable': true,
              'mode': 'push'
            },
            'resize': true
          },
          'modes': {
            'grab': {
              'distance': 400,
              'line_linked': {
                'opacity': 1
              }
            },
            'bubble': {
              'distance': 400,
              'size': 40,
              'duration': 2,
              'opacity': 8,
              'speed': 3
            },
            'repulse': {
              'distance': 200,
              'duration': 0.4
            },
            'push': {
              'particles_nb': 4
            },
            'remove': {
              'particles_nb': 2
            }
          }
        },
        'retina_detect': true
      })
    }
  }

}
</script>

<style lang="scss" scoped>
    .home_title{
        position: absolute;
        top: 20%;
        right: 0;
        bottom: 0;
        left: 0;
        padding: 1.25rem;
    }

    .my_home_pic{
    width: 15em;
    height: 15em;
    border-radius : 50%;
  }

  .btn-twitter{
    color:#DAD3CB;
    margin-right:4em;
    :hover{
    color:#1DA1F2;
    cursor: pointer;
    }
  }

  .btn-github{
    color:#DAD3CB;
    :hover{
    color:black;
    cursor: pointer;
    }
  }
</style>