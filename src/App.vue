<template>
  <div id="app">
    <a-row type="flex">
      <a-col
        :xs="{span: 16, order: 2}"
        :sm="{span: 12, order: 2}"
        :md="{span: 15, order: 2}"
        :lg="{span: 6, order: 1}"
        :xl="{span: 4, order: 1}"
      >
        <div class="text-div">Col1</div>
      </a-col>
      <a-col
        :xs="{span: 4, order: 1}"
        :sm="{span: 4, order: 1}"
        :md="{span: 3, order: 1}"
        :lg="{span: 10, order: 2}"
        :xl="{span: 10, order: 2}"
      >
        <div class="text-div">Col2</div>
      </a-col>
      <a-col
        :xs="{span: 4, order: 3}"
        :sm="{span: 4, order: 3}"
        :md="{span: 3, order: 3}"
        :lg="{span: 2, order: 3}"
        :xl="{span: 6, order: 3}"
      >
        <div class="text-div">Col3</div>
      </a-col>
      <a-col
        :xs="{span: 0, order: 4}"
        :sm="{span: 4, order: 4}"
        :md="{span: 3, order: 4}"
        :lg="{span: 6, order: 4}"
        :xl="{span: 4, order: 4}"
      >
        <div class="text-div">Col4</div>
      </a-col>
    </a-row>
    <a-row>
      <a-col :xl="24">
        <div class="context-div">
          <a-row>
            <a-col :xs="24" :sm="24" :md="24" :lg="24" :xl="18">
              <div class="left-context"></div>
            </a-col>
            <a-col :xs="0" :sm="0" :md="0" :lg="0" :xl="6">
              <div class="sider"></div>
            </a-col>
          </a-row>
        </div>
      </a-col>
    </a-row>
  </div>
</template>

<style scoped>
#app {
  text-align: center;
}
div {
  line-height: 64px;
  border-style: solid;
  border-width: 1px;
}
.text-div {
  height: 64px;
  background-color: blanchedalmond;
}
.context-div {
  background-color: cornflowerblue;
  height: 1200px;
  max-width: 1200px;
  margin: 0px auto;
}
.left-context {
  height: 1200px;
  background-color: skyblue;
}
.sider {
  height: 1200px;
  background-color: springgreen;
}
</style>
