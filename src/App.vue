<template>
  <!--root element -->
  <div id="app">
    <div>
      <h1 :class="{ daChon: selected }">lap trinh vien</h1>
      <button @click="selected = !selected">Doi mau</button>

      <hr />
      <input type="text" :disabled="inputDisabled" />
      <button @click="inputDisabled = !inputDisabled">Mo khoa</button>
      <!--chu y co : -->
    </div>

    <hr />
    <div>
      <input type="text" v-model="changemane" />
      {{ changemane }}
    </div>

    <hr />
    <div>
      <input type="text" v-model="changemanes[0]" />
      <input type="text" v-model="changemanes[1]" />
      {{ changemanes }}
    </div>

    <hr />
    <div>
      <input type="text" v-model="channel.name" />
      {{ channel.name }}
    </div>

    <hr />
    <div>
      <input type="text" v-model="channel.name" />
      <button v-on:click="channel.name = 'Aaaaaa'">Go</button>
      <button v-on:mouseover="channel.name = 'Aaaaaa'">Go</button>
    </div>

    <hr />
    <div>
      <form action="/abc">
        <input type="text" v-model="channel.name" />
        <button type="submit" v-on:click.prevent="channel.name = 'Aaaaaa'">
          Send
        </button>
      </form>
    </div>

    <hr />
    <div>
      <div v-if="isShow">Lap trinh vien</div>
      <button @click="(isShow = !isShow)">
        <span v-if="isShow">An</span>
        <span v-else>Hien</span>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      inputDisabled: true,
      isShow: true,
      selected: true,
      changemane: "Gau gau",
      changemanes: ["Gau gau 1", "Gau gau 2"],
      channel: {
        //object
        name: "Gau gau",
      },
    };
  },
};
</script>

<style>
.daChon {
  color: red;
}
</style>
