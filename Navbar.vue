<template>
  <nav>
       <v-toolbar app d-flex-all class="overflow-hidden">
      <v-app-bar-nav-icon class="grey--text" @click="drawer = !drawer"></v-app-bar-nav-icon>
     
      <v-row class="mt-4">
        <v-col cols="16" sm="9">
          <v-text-field class="text"
            lebel="outlined"
            single-line
            outlined
            placeholder="Keyword"
          >
          </v-text-field>
        </v-col>
      </v-row>

      <v-btn icon class="magni">
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
      <v-space></v-space>
      <v-btn depressed small class="transparent blue--text icon1">
        <v-icon small>mdi-email</v-icon>
        <v-badge 
        color="red"
        content="10"
        >
          <span style="font-weight:bold">Inbox</span>
        </v-badge>
        
      </v-btn>
      <v-btn depressed small class="transparent blue--text ">
        <v-icon small>mdi-bell</v-icon>
        <v-badge
        color="red"
        content="6"
        >
          <span style="font-weight:bold">Messages</span>
        </v-badge>
      </v-btn>
      <v-btn depressed small class="transparent blue--text ">
        <v-icon small>mdi-account</v-icon>
        <span style="font-weight:bold">User</span>
      </v-btn>
    </v-toolbar>
    <v-navigation-drawer v-model="drawer" app class="indigo">
      
      <v-list-item>
        <v-list-item-content>
           
             <v-list-item-title class="title red white--text" >
            DASHBOARD
          </v-list-item-title>
          
          <v-list class="my-3">
            <v-list-tile v-for="link in links" :key="link.text" router :to="link.route">
              <v-list-tile-contnent>
                <v-icon small class="ml-3 black--text">{{link.icon}}</v-icon>
              </v-list-tile-contnent>
              <v-list-tile-title>
                <v-tile-title class="ml-4" style="font-size:13px; font-weight:bold">{{link.text}}</v-tile-title>
              </v-list-tile-title>
            </v-list-tile>
          </v-list>

          <v-list-item-title class="title black white--text" >
            PAGES
          </v-list-item-title>

          <v-list-item-subtitle>
            <v-btn depressed small class="transparent">
            <v-icon small>mdi-account</v-icon>
            <span class="sub">Account</span>
            </v-btn>
            <v-btn depressed small class="transparent">
              <v-icon small right>mdi-plus</v-icon>
            </v-btn>
          </v-list-item-subtitle>

          <v-list-item-subtitle>
            <v-btn depressed small class="transparent">
            <v-icon small>mdi-post</v-icon>
            <span class="sub">Posts</span>
            </v-btn>
            <v-btn depressed small class="transparent plus1">
              <v-icon right small >mdi-plus</v-icon>
            </v-btn>
          </v-list-item-subtitle>
          
          <v-list-item-subtitle>
            <v-btn depressed small class="transparent">
            <v-icon small>mdi-bag-personal</v-icon>
            <span class="sub">Products</span>
            </v-btn>
            <v-btn depressed small class="transparent">
              <v-icon small >mdi-plus</v-icon>
            </v-btn>
          </v-list-item-subtitle>
          
          <v-list-item-subtitle>
            <v-btn depressed small class="transparent">
            <v-icon small>mdi-cart</v-icon>
            <span class="sub">Orders</span>
            </v-btn>
            <v-btn depressed small class="transparent plus2">
              <v-icon right small>mdi-plus</v-icon>
            </v-btn>
          </v-list-item-subtitle>
          
          <v-list-item-subtitle>
            <v-btn depressed small class="transparent">
            <v-icon small>mdi-chat-processing</v-icon>
            <span class="sub">Comments</span>
            </v-btn>
            <v-btn depressed small class="transparent">
              <v-icon left small>mdi-plus</v-icon>
            </v-btn>
          </v-list-item-subtitle>
          
          <v-list-item-subtitle>
            <v-btn depressed small class="transparent">
            <v-icon small>mdi-frequently-asked-questions</v-icon>
            <span class="sub">faq</span>
            </v-btn>
          </v-list-item-subtitle>

          <v-list-item-title class="title black white--text element">
            UI ELEMENTS
          </v-list-item-title>

          <v-list-item-subtitle>
            <v-btn depressed small class="transparent">
            <v-icon small>mdi-table</v-icon>
            <span class="sub">Tables</span>
            </v-btn>
          </v-list-item-subtitle>

          <v-list-item-subtitle>
            <v-btn depressed small class="transparent">
            <v-icon small>mdi-file</v-icon>
            <span class="sub">form</span>
            </v-btn>
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
      </v-navigation-drawer>
  </nav>

</template>

<script>

export default {
    data() {
      return {
        drawer: false,
        links: [
          { icon: 'mdi-view-dashboard', text: 'DASHBOARD', route: '/dashboard'}
        ]
      }
    }
}
</script>

<style scoped>
.magni{
  position: absolute;
  margin-left: 290px;
  
}

.v-btn > .v-btn__content .v-icon{
    color: rgb(0 0 0);
}
.icon1{
  position: relative;
  margin-left: 480px;
}
.title{
  padding: 15px;
}
.sub{
  padding-left:25px;
  font-weight: bold;
}
.plus1{
  margin-left: 20px;
  padding: 0;
}
.plus2{
  margin-left: 11px;
  padding: 0;
}
.transparent{
  margin-top: 15px;
}
.element{
  margin-top: 30px;
}
.sub1{
  margin-bottom: 15px;
}
</style>