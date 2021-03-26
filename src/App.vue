<template>
  <v-app id="inspire">
    <v-navigation-drawer width="280" v-model="drawer" app cols="12">
      <v-sheet class="pa-7">
        <v-avatar class="mb-4" size="50"
          ><img
            src="https://comoequetala.com.br/images/com_vagasejobs/empresa/marca/19-7ca539eaadb583ed8adbfa8ffcc8e48e.png"
            alt="logo"
          />
        </v-avatar>
        <p class="titulo">Iginição Digital</p>
      </v-sheet>

      <v-col>
        <v-select
          id="select"
          dense
          solo
          x-small
          label="Área do Cliente"
          prepend-inner-icon="mdi-home-variant-outline"
          background-color="#ECECEC"
        ></v-select
      ></v-col>

      <br />
      <v-container>
        <v-p class="app"><b>Apps</b></v-p>
      </v-container>

      <v-list>
        <v-list-item v-for="[icon, text] in links" :key="icon" link>
          <v-list-item-icon>
            <v-icon id="icon2">{{ icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title class="list1">{{ text }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <div>
      <v-app-bar id="nav-bar" dense>
        <v-btn icon>
          <v-icon id="icon2">mdi-checkbox-marked-outline</v-icon>
        </v-btn>
        <v-btn icon>
          <v-icon id="icon2">mdi-message-outline</v-icon>
        </v-btn>
        <v-btn icon>
          <v-icon id="icon2">mdi-email-outline</v-icon>
        </v-btn>

        <v-btn icon>
          <v-icon id="icon2">mdi-calendar-outline</v-icon>
        </v-btn>
        <v-btn icon disabled>
          <v-icon>mdi-star-outline</v-icon>
        </v-btn>

        <v-spacer></v-spacer>

        <v-btn icon class="btn1">
          <v-icon id="icon2">mdi-bell-outline</v-icon>
        </v-btn>

        <v-btn icon class="btn2">
          <v-icon id="icon2">mdi-magnify</v-icon>
        </v-btn>
        <v-list-item-content>
          <v-list-item-title class="usuario1">Maria Elza</v-list-item-title>

          <v-list-item-subtitle class="usuario2">
            Cliente VIP</v-list-item-subtitle
          >
        </v-list-item-content>
        <v-avatar class="logo-avatar" size="35"
          ><img
            src="https://img2.gratispng.com/20180703/ya/kisspng-computer-icons-user-avatar-user-5b3bafe2381423.1933594815306383062297.jpg"
            alt="logo-avatar"
        /></v-avatar>
      </v-app-bar>
    </div>

    <v-main>
      <v-container class="py-8 px-6">
        <v-row>
          <template>
            <v-list-item>
              <v-p class="p">Resultados</v-p>

              <v-divider class="divider" vertical></v-divider>
              <v-icon id="icon1">mdi-home-variant-outline</v-icon>
              <p class="p2">>></p>
              <p class="p2">Cursos</p>
              <v-avatar class="avatar1" size="35" color="grey">
                <img
                  class="imagem"
                  src="https://e7.pngegg.com/pngimages/548/792/png-clipart-gear-symbol-computer-icons-encapsulated-postscript-logo-setting-miscellaneous-logo.png"
                  alt="logo-config"
              /></v-avatar>
            </v-list-item>
          </template>
        </v-row>
      </v-container>
    </v-main>

      <v-container>
        <v-row>
          <template>
            <v-list-item>
              <v-p class="filtro">Filtros</v-p>

              <v-p class="p1">200 resultados encontrados</v-p>
              <v-col sm="2">
                <v-select
                  class="listagem"
                  dense
                  solo
                  x-small
                  label="Listagem"
                ></v-select
              ></v-col>
              <v-btn class="view" icon tile elevation="2"
                ><v-icon>mdi-view-grid-outline</v-icon></v-btn
              >
              <v-btn class="menu" icon tile elevation="2"
                ><v-icon>mdi-menu</v-icon></v-btn
              >
            </v-list-item>
          </template>
        </v-row>
      </v-container>

      <v-app-bar id="busca" dense>
        <v-toolbar-title class="toolbar">Buscar</v-toolbar-title>

        <v-spacer></v-spacer>

        <v-btn icon>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>
      </v-app-bar>

     <meu-card></meu-card>

    <meu-filtro></meu-filtro>
    <br />
    <br />
    <br />
    <br />

    <div class="pagina">
      <v-pagination
        v-model="page"
        :length="10"
        color="#969696"
        circle
      ></v-pagination>
    </div>
    <br />
  </v-app>
</template>


<script>
import Card from './components/Card/card.vue'
import Filtro from './components/Filtro/filtro.vue'
export default {
  data: () => ({
    drawer: null,
    links: [
      ["mdi-email-outline", "E-mail"],
      ["mdi-message-outline", "Conversar"],
      ["mdi-checkbox-marked-outline", "Todo"],
      ["mdi-calendar-outline", "Calendário"],
    ],
    page: 6,
  }),
  components:{
    'meu-card':Card,
    'meu-filtro':Filtro
  
}
};
</script>
<style >
#inspire {
  background-color: #f9f9f9;
  font-family: "Montserrat", sans-serif;
}

#nav-bar {
  background: white;
  width: 76%;
  margin-left: 23%;
  border-radius: 8px;
  top: 15%;
}
.usuario1 {
  margin-left: 77%;
  font-size: 14px;
  color: #2c2c2c;
}
.usuario2 {
  margin-left: 80%;
  font-size: 11px;
  color: #2c2c2c;
}
.btn1 {
  left: 25.5%;
}
.btn2 {
  left: 24%;
}
#btn3 {
  width: 70%;

  font-size: 18px;

  margin-left: 15%;
  background: #696969;
  height: 4%;
  border-radius: 8px;
}

.titulo {
  color: #ff7b1b;
  margin-top: -50px;
  margin-left: 60px;

  font-size: 16px;
}
.p {
  font-size: 24px;
  margin-left: 0.5%;

  color: #2c2c2c;
}
.p1 {
  color: #2c2c2c;

  margin-left: 29%;
  margin-top: 20px;
  font-size: 18px;
}
.p2 {
  margin-top: 2%;
  margin-left: 0.5%;
  color: #000000;

  font-size: 14px;
}


.divider {
  margin-left: 2%;
}
#icon1 {
  color: #000000;
  margin-left: 1%;
  font-size: 20px;
}

.avatar1 {
  margin-left: 73.5%;
}
.imagem {
  max-width: 70%;
  max-height: 70%;
}
.menu {
  border-radius: 8px;
  left: 12.5%;
  background-color: white;
}
.view {
  border-radius: 8px;
  left: 11.5%;
  background-color: white;
}
.listagem {
  left: 75%;
  top: 15px;
  border-radius: 8px;
}
#busca {
  background: white;

  font-size: 22px;
  border-radius: 8px;
  width: 48%;
  margin-left: 51%;
  top: 3px;
}


.filtro {
  margin-left: 19%;
  margin-top: 3%;

  font-size: 18px;
  color: #2c2c2c;
}

#select {
  border-radius: 4px;

  color: #ececec;
}
.list1 {
  color: #2c2c2c;
}

#icon2 {
  color: #606060;
}

.toolbar {
  color: #999999;
}
.app {
  color: #999999;
  font-size: 14px;
}
.pagina {
  margin-left: 25%;
}
.logo-avatar {
  margin-left: 0%;
}
</style>
