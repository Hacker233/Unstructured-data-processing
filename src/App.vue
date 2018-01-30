<template>
  <div id="app">
    <head1></head1>
    <router-view></router-view>
    <foot></foot>
  </div>
</template>

<script>
import foot from '@/components/foot'
import head1 from '@/components/head1'
export default {
  name: 'App',
  components:{
    foot,head1
  }
}
</script>

<style>
@keyframes fadein{
    0%{opacity: 0;
         }
    100%{
        opacity: 1;

    }
}
@-webkit-keyframes fadein{
        0%{opacity: 0;
         }
    100%{
        opacity: 1;

    }
}
@-moz-keyframes fadein{
        0%{opacity: 0;
         }
    100%{
        opacity: 1;

    }
}
@-o-keyframes fadein{
        0%{opacity: 0;
         }
    100%{
        opacity: 1;

    }
}
@-ms-keyframes fadein{
        0%{opacity: 0;
         }
    100%{
        opacity: 1;

    }
}
body{
    animation:fadein 2s linear 1;
    -webkit-animation:fadein 2s linear 1;
    -moz-animation:fadein 2s linear 1;
    -o-animation:fadein 2s linear 1;
    -ms-animation:fadein 2s linear 1;
}
</style>
