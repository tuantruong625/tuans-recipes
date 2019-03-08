<template>
  <app-navigation></app-navigation>
</template>

<script>
import { StackNavigator } from "vue-native-router";
import SplashScreen from './src/screens/SplashScreen.vue';
const AppNavigation = StackNavigator(
  {
    Home: SplashScreen,
  },
  {
    initialRouteName: 'Home',
  }
);
export default {
  components: { AppNavigation },
}
</script>
