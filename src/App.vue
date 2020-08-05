<template>
  <div id="app">
    <a-affix :offset-top="0">
      <div class="head">
        <a-row type="flex">
          <a-col
            :xs="{span: 16, order: 2}"
            :sm="{span: 12, order: 2}"
            :md="{span: 15, order: 2}"
            :lg="{span: 6, order: 1}"
            :xl="{span: 4, order: 1}"
          >
            <div class="logo-div">Logo</div>
          </a-col>
          <a-col
            :xs="{span: 4, order: 1}"
            :sm="{span: 4, order: 1}"
            :md="{span: 3, order: 1}"
            :lg="{span: 10, order: 2}"
            :xl="{span: 10, order: 2}"
          >
            <div class="menu-div">
              <div>
                <a-menu v-model="current" mode="horizontal">
                  <a-menu-item key="mail">
                    <a-icon type="mail" />Navigation One
                  </a-menu-item>
                  <a-menu-item key="app" disabled>
                    <a-icon type="appstore" />Navigation Two
                  </a-menu-item>
                  <a-sub-menu>
                    <span slot="title" class="submenu-title-wrapper">
                      <a-icon type="setting" />Navigation Three - Submenu
                    </span>
                    <a-menu-item-group title="Item 1">
                      <a-menu-item key="setting:1">Option 1</a-menu-item>
                      <a-menu-item key="setting:2">Option 2</a-menu-item>
                    </a-menu-item-group>
                    <a-menu-item-group title="Item 2">
                      <a-menu-item key="setting:3">Option 3</a-menu-item>
                      <a-menu-item key="setting:4">Option 4</a-menu-item>
                    </a-menu-item-group>
                  </a-sub-menu>
                  <a-menu-item key="alipay">
                    <a
                      href="https://antdv.com"
                      target="_blank"
                      rel="noopener noreferrer"
                    >Navigation Four - Link</a>
                  </a-menu-item>
                </a-menu>
              </div>
            </div>
          </a-col>
          <a-col
            :xs="{span: 4, order: 3}"
            :sm="{span: 4, order: 3}"
            :md="{span: 3, order: 3}"
            :lg="{span: 2, order: 3}"
            :xl="{span: 6, order: 3}"
          >
            <div class="search-div">
              <a-input-search placeholder="input search text" enter-button @search="onSearch" />
            </div>
          </a-col>
          <a-col
            :xs="{span: 0, order: 4}"
            :sm="{span: 4, order: 4}"
            :md="{span: 3, order: 4}"
            :lg="{span: 6, order: 4}"
            :xl="{span: 4, order: 4}"
          >
            <div class="avatar-div">
              <a-badge :dot="true"><a-icon type="bell" /></a-badge>
               <a-badge count="5"><a-icon type="message" /></a-badge>
              <a-avatar size="large" icon="user" />
            </div>
          </a-col>
        </a-row>
      </div>
    </a-affix>
    <a-row>
      <a-col :xl="24">
        <div class="context-div">
          <a-row>
            <a-col :xs="24" :sm="24" :md="24" :lg="24" :xl="18">
              <div class="left-context">
                <div class="blog-list">
                  <div class="blog-context-div">
                    <a-row>
                      <a-col :xs="0" :sm="0" :md="10" :lg="10" :xl="10">
                        <div class="blog-image-div"></div>
                      </a-col>
                      <a-col :xs="24" :sm="24" :md="14" :lg="14" :xl="14">
                        <div class="intro">
                          <div class="blog-title-div">
                            <div class="title">这是博客的标题</div>
                            <div class="author">作者发布时间等</div>
                          </div>
                          <div class="blog-intro-div">这是博客的简介</div>
                          <div class="blog-other-div">这是阅读点赞信息</div>
                        </div>
                      </a-col>
                    </a-row>
                  </div>
                </div>
              </div>
            </a-col>
            <a-col :xs="0" :sm="0" :md="0" :lg="0" :xl="6">
              <div class="sider"></div>
            </a-col>
          </a-row>
        </div>
      </a-col>
    </a-row>
    <div class="footer"></div>
  </div>
</template>

<style scoped>
#app {
  text-align: center;
}
div {
  /* line-height: 64px;*/
  border-style: solid;
  border-width: 0.5px;
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
  max-width: 900px;
  margin: 0px auto;
  background-color: skyblue;
}
.sider {
  height: 1200px;
  background-color: springgreen;
}
.blog-list {
  /* width: 100%; */
  min-height: 250px;
  background-color: springgreen;
  margin: 10px 10px;
  /* max-width: 900px; */
}
.blog-context-div {
  margin: 10px 10px;
  min-height: 230px;
}
.intro {
  min-height: 230px;
}
.blog-image-div {
  min-height: 230px;
  /* min-height: 230px; */
  /* height: 100%; */
}
.blog-title-blog {
  height: 64px;
}
.blog-intro-div {
  min-height: 146px;
  line-height: 146px;
}
.blog-other-div {
  height: 20px;
  line-height: 20px;
}
.title {
  height: 44px;
  line-height: 44px;
}
.author {
  height: 20px;
  line-height: 20px;
}
.search-div {
  line-height: 64px;
}
.head{
  background-color: #ffffff;
}
.footer{
  width: 100%;
  height: 64px;
  background-color: #000000;
}
</style>
