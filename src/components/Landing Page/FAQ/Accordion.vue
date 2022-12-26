<template lang="">
  <div class="Expander">
      <div class="Expander__trigger" 
        @click="open=!open" 
        :class="open?'active':'beforeBorder'">
          <svg 
            class="Expander__trigger-Icon" 
            :class="{open:open}" 
            width="40" height="40" 
            :style="{background: '#FBD531', padding:`15px 0 0 0`, 'margin-right':'20px', 'border-radius':`100%`, 'text-align':'center', }"
            stroke="#fff">
            
             <polyline points="12,2 20,10 28,2" stroke-width="3" fill="none"></polyline>
                  
        
          </svg>
      
          <h1 class="cost">{{ title }}</h1>
      </div>
      <transition :name="animation">
          <div class="Expander__body" v-show="open">
              <slot></slot>
          </div>
      </transition>
  </div>
</template>
<script>
export default {
  name: "AccordionVue",
  props: {
    title: {
      type: String,
      default: "title",
    },
    animation: {
      type: String,
      default: "bottomToTop",
      // validator: prop => ['leftToRight', 'bounceIn', 'bottomToTop'].includes(prop)
    },
  },
  data() {
    return {
      open: false,
     
    };
  },
};
</script>
<style scoped>
.Expander {
  position: relative;
  width: 500px;
}
.Expander__trigger {
  cursor: pointer;
  padding: 0.7rem 0.5rem;
  display: inline-flex;
  flex-direction: row;
  justify-content: space-between;
  justify-self: self-start  ;
  width: fit-content;
  border-bottom: 1px solid #efefef;
}


.Expander .active {
  width: fit-content;

 
}
/* //color #777 */

.Expander-Icon {
  transition: transform 0.2s cubic-bezier(0.23, 1, 0.32, 1);
}
.Expander .open {
  max-width: 100%;
  stroke: #fff;
  transform: rotate(180deg);
}

.Expander__body {
  /* max-width: 30%; */
  padding: 2%;
  background: #eff0f2;
  width:90%;
  overflow: hidden;
  text-align: start;
}

.rightToLeft-enter-active {
  animation: rightToLeft 0.5s;
}
.rightToLeft-leave-active {
  animation: rightToLeft 0.5s reverse;
}
@keyframes rightToLeft {
  0% {
    transform: translateX(100vw);
  }
  50% {
    transform: translateX(-2em);
  }
  100% {
    transform: translateX(0);
  }
}

.leftToRight-enter-active {
  animation: leftToRight 0.5s;
}
.leftToRight-leave-active {
  animation: leftToRight 0.5s reverse;
}
@keyframes leftToRight {
  0% {
    transform: translateX(-100vw);
  }
  50% {
    transform: translateX(2em);
  }
  100% {
    transform: translateX(0);
  }
}

.bounceIn-enter-active {
  animation: bounceIn 0.3s;
}
.bounceIn-leave-active {
  animation: bottomToTop 0.2s reverse;
}
@keyframes bounceIn {
  from,
  20%,
  40%,
  60%,
  80%,
  to {
    animation-timing-function: cubic-bezier(0.215, 0.61, 0.355, 1);
  }
  0% {
    opacity: 0;
    transform: scale3d(0.3, 0.3, 0.3);
  }
  20% {
    transform: scale3d(1.1, 1.1, 1.1);
  }
  40% {
    transform: scale3d(0.9, 0.9, 0.9);
  }
  60% {
    opacity: 1;
    transform: scale3d(1.03, 1.03, 1.03);
  }
  80% {
    transform: scale3d(0.97, 0.97, 0.97);
  }
  to {
    opacity: 1;
    transform: scale3d(1, 1, 1);
  }
}

.bottomToTop-enter-active {
  animation: bottomToTop 0.5s forwards;
}
.bottomToTop-leave-active {
  animation: bottomToTop 0.5s reverse;
}
@keyframes bottomToTop {
  0% {
    opacity: 0;
    transform: translateY(100%);
  }
  100% {
    transform: translateY(0);
  }
}
.cost{
font-family: 'Rubik';
font-style: normal;
font-weight: 500;
font-size: 25px;
line-height: 40px;
color: #1D467B;


    }
</style>
