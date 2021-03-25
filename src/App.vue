<template>
  <v-app id="inspire">
    <v-navigation-drawer width="280" v-model="drawer" app>
      <v-sheet class="pa-7">
        <v-avatar class="mb-4" size="50"
          ><img
            src="https://comoequetala.com.br/images/com_vagasejobs/empresa/marca/19-7ca539eaadb583ed8adbfa8ffcc8e48e.png"
            alt="logo"
          />
        </v-avatar>
        <p class="titulo">Iginição Digital</p>
      </v-sheet>

      <v-col >
        <v-select
      id="select"
          dense
          solo
          x-small
          label="Ária do Cliente"
          prepend-inner-icon="mdi-home-variant-outline"
          outlined
          
          background-color="#ECECEC"
        ></v-select
      ></v-col>

      <br /><br />
      <v-container>
        <v-p>Apps</v-p>
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
      <v-app-bar id="nav-bar" width="1025px"  dense >
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
        <v-list-item-content >
          <v-list-item-title class="usuario1">Maria Elza</v-list-item-title>

          <v-list-item-subtitle class="usuario2"> Cliente VIP</v-list-item-subtitle>
        </v-list-item-content>
        <v-avatar size="35" color="grey" />
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

      <v-container >
        <v-row>
        
            <template>
              <v-list-item>
                <v-p class="filtro">Filtros</v-p>

                <v-p class="p1">200 resultados encontrados</v-p>
                <v-col class="d-flex" cols="12" sm="2">
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

      <v-app-bar id="busca"  dense >
        <v-toolbar-title class="toolbar">Buscar</v-toolbar-title>

        <v-spacer></v-spacer>

        <v-btn icon>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>
      </v-app-bar>

      <v-container class="py-8 px-6">
        <v-row>
          <v-card id="card1" width="650" outlined>
            <v-list>
              <template>
                <v-list-item>
                  <v-list-item-avatar
                    tile
                    size="150"
                    color="grey"
                  ></v-list-item-avatar>

                  <v-list-item-content>
                    <div class="div1">Formula de Lançamento</div>
                    <v-list-item-title class="list2">Por <b>Erico Rocha</b></v-list-item-title>

                    <v-list-item-subtitle class="list3">
                      Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                      Nihil repellendus distinctio similique
                    </v-list-item-subtitle>
                  </v-list-item-content>
                  <v-divider vertical></v-divider>

                  <v-col sm="3">
                    <v-btn id="btn4" small dark
                      >3.4<v-icon id="star1">mdi-star-outline</v-icon></v-btn
                    ><v-p class="dinheiro">R$2500</v-p>
                    <v-btn class="botao1" ><v-icon>mdi-heart-outline</v-icon> Amei </v-btn>
                    <v-btn id="botao" dark ><v-icon>mdi-shopping-outline</v-icon> Comprar  </v-btn>
                  </v-col>
                </v-list-item>
              </template>
            </v-list>
          </v-card>
        </v-row>
      </v-container>

      <v-container class="py-8 px-6">
        <v-row>
          <v-card id="card2" max-width="650" outlined>
            <v-list>
              <template>
                <v-list-item>
                  <v-list-item-avatar
                    tile
                    size="150"
                    color="grey"
                  ></v-list-item-avatar>

                  <v-list-item-content>
                    <div>Formula de Lançamento</div>
                    <v-list-item-title>Por <b>Erico Rocha</b></v-list-item-title>

                    <v-list-item-subtitle>
                      Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                      Nihil repellendus distinctio similique
                    </v-list-item-subtitle>
                  </v-list-item-content>
                  <v-divider vertical></v-divider>
                  <v-col sm="3">
                    <v-btn id="btn4" small dark
                      >3.4<v-icon id="star1">mdi-star-outline</v-icon></v-btn
                    ><v-p class="dinheiro">R$2500</v-p>
                    <v-btn class="botao1" ><v-icon>mdi-heart-outline</v-icon> Amei </v-btn>
                    <v-btn id="botao" dark ><v-icon>mdi-shopping-outline</v-icon> Comprar  </v-btn>
                  </v-col>
                </v-list-item>
              </template>
            </v-list>
          </v-card>
        </v-row>
      </v-container>

      <v-container class="py-8 px-6">
        <v-row>
          <v-card id="card3" max-width="650" outlined>
            <v-list>
              <template>
                <v-list-item>
                  <v-list-item-avatar
                    tile
                    size="150"
                    color="grey"
                  ></v-list-item-avatar>

                  <v-list-item-content>
                    <div>Formula de Lançamento</div>
                    <v-list-item-title>Por <b>Erico Rocha</b></v-list-item-title>

                    <v-list-item-subtitle>
                      Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                      Nihil repellendus distinctio similique
                    </v-list-item-subtitle>
                  </v-list-item-content>
                  <v-divider vertical></v-divider>
                  <v-col sm="3">
                    <v-btn id="btn4" small dark
                      >3.4<v-icon id="star1">mdi-star-outline</v-icon></v-btn
                    >
                    <v-p class="dinheiro">R$2500</v-p>
                    <v-btn class="botao1" ><v-icon>mdi-heart-outline</v-icon> Amei </v-btn>
                    <v-btn id="botao" dark ><v-icon>mdi-shopping-outline</v-icon> Comprar  </v-btn>
                  </v-col>
                </v-list-item>
              </template>
            </v-list>
          </v-card>
        </v-row>
      </v-container>

      <v-container class="py-8 px-6">
        <v-row>
          <v-card id="card4" max-width="650" outlined cols="12">
            <v-list>
              <template>
                <v-list-item>
                  <v-list-item-avatar
                    tile
                    size="150"
                    color="grey"
                  ></v-list-item-avatar>

                  <v-list-item-content>
                     <div>Formula de Lançamento</div>
                    <v-list-item-title>Por <b>Erico Rocha</b></v-list-item-title>

                    <v-list-item-subtitle>
                      Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                      Nihil repellendus distinctio similique
                    </v-list-item-subtitle>
                  </v-list-item-content>
                  <v-divider vertical></v-divider>
                  <v-col sm="3">
                    <v-btn id="btn4" small dark
                      >3.4<v-icon id="star1">mdi-star-outline</v-icon></v-btn
                    >
                    <v-p class="dinheiro">R$2500</v-p>
                   <v-btn class="botao1" ><v-icon>mdi-heart-outline</v-icon> Amei </v-btn>
                    <v-btn id="botao" dark ><v-icon>mdi-shopping-outline</v-icon> Comprar  </v-btn>
                  </v-col>
                </v-list-item>
              </template>
            </v-list>
          </v-card>
        </v-row>
      </v-container>

      <v-container class="py-8 px-6">
        <v-row>
          <v-card id="card5" max-width="650" outlined cols="12">
            <v-list>
              <template>
                <v-list-item>
                  <v-list-item-avatar
                    tile
                    size="150"
                    color="grey"
                  ></v-list-item-avatar>

                  <v-list-item-content>
                     <div>Formula de Lançamento</div>
                    <v-list-item-title>Por <b>Erico Rocha</b></v-list-item-title>

                    <v-list-item-subtitle>
                      Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                      Nihil repellendus distinctio similique
                    </v-list-item-subtitle>
                  </v-list-item-content>
                  <v-divider vertical></v-divider>
                  <v-col sm="3">
                    <v-btn id="btn4" small dark
                      >3.4<v-icon id="star1">mdi-star-outline</v-icon></v-btn
                    >
                    <v-p class="dinheiro">R$2500</v-p>
                   <v-btn class="botao1" ><v-icon>mdi-heart-outline</v-icon> Amei </v-btn>
                    <v-btn id="botao" dark ><v-icon>mdi-shopping-outline</v-icon> Comprar  </v-btn>
                  </v-col>
                </v-list-item>
              </template>
            </v-list>
          </v-card>
        </v-row>
      </v-container>
    </v-main>

    <v-main>
      <v-container>
        <v-row>
          <v-card class="form" width="371px" height="1170px" outlined>
            <v-container>
              <h3>Preços</h3>
              <v-radio-group>
                <v-radio label="R$10" value="radio-1"></v-radio>
                <v-radio label="R$10-$100" value="radio-2"></v-radio>
                <v-radio label="R$100-$500" value="radio-3"></v-radio>
                <v-radio label="R$500" value="radio-4"></v-radio>
                <v-radio label="Todos" value="radio-5"></v-radio>
              </v-radio-group>
              <v-divider></v-divider>
            </v-container>
            <v-container>
              <h3>Valores</h3>
              <h3 class="valores">1.99-4098</h3>
              <v-card-text>
                <v-range-slider v-model="value" step="10"></v-range-slider>
              </v-card-text>
              <v-divider></v-divider>
            </v-container>

            <v-container>
              <h3>Categorias</h3>

              <v-checkbox label="Érico Rocha"></v-checkbox>
              <p id="check">1920</p>
              <v-checkbox label="Desafio 6 em 7"></v-checkbox>
              <p id="check">1820</p>
              <v-checkbox label="Formula de Lançamento"></v-checkbox>
              <p id="check">462</p>
              <v-checkbox label="KlickPages "></v-checkbox>
              <p id="check">6556</p>
              <v-checkbox label="Audios"></v-checkbox>
              <p id="check">120</p>

              <v-divider></v-divider>
            </v-container>

            <v-container>
              <h3>Avaliação</h3>
              <v-row class="mt-1">
                <v-col sm="8">
                  <v-btn icon disabled>
                    <v-icon>mdi-star</v-icon>
                  </v-btn>
                  <v-btn icon disabled>
                    <v-icon>mdi-star</v-icon>
                  </v-btn>
                  <v-btn icon disabled>
                    <v-icon>mdi-star</v-icon>
                  </v-btn>
                  <v-btn icon disabled>
                    <v-icon>mdi-star</v-icon>
                  </v-btn>
                  <v-btn icon disabled>
                    <v-icon>mdi-star</v-icon>
                  </v-btn>
                </v-col>
                <p class="avaliacao">8500</p>
              </v-row>

              <v-row class="mt-1">
                <v-col sm="8">
                  <v-btn icon disabled>
                    <v-icon>mdi-star</v-icon>
                  </v-btn>
                  <v-btn icon disabled>
                    <v-icon>mdi-star</v-icon>
                  </v-btn>
                  <v-btn icon disabled>
                    <v-icon>mdi-star</v-icon>
                  </v-btn>
                  <v-btn icon disabled>
                    <v-icon>mdi-star</v-icon>
                  </v-btn>
                  <v-btn icon disabled>
                    <v-icon>mdi-star-outline</v-icon>
                  </v-btn>
                </v-col>
                <p class="avaliacao">3250</p>
              </v-row>

              <v-row class="mt-1">
                <v-col sm="8">
                  <v-btn icon disabled>
                    <v-icon>mdi-star</v-icon>
                  </v-btn>
                  <v-btn icon disabled>
                    <v-icon>mdi-star</v-icon>
                  </v-btn>
                  <v-btn icon disabled>
                    <v-icon>mdi-star</v-icon>
                  </v-btn>
                  <v-btn icon disabled>
                    <v-icon>mdi-star-outline</v-icon>
                  </v-btn>
                  <v-btn icon disabled>
                    <v-icon>mdi-star-outline</v-icon>
                  </v-btn>
                </v-col>
                <p class="avaliacao">1120</p>
              </v-row>
            </v-container>
            <br />
            <br /><br /><br /><br /><br /><br />

            <v-btn id="btn3" dark>Limpar Filtros</v-btn>
          </v-card>
        </v-row>
      </v-container>
    </v-main>
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />

    <div class="text-center">
      <v-pagination v-model="page" :length="10" circle></v-pagination>
    </div>
  </v-app>
</template>


<script>
export default {
  data: () => ({
    drawer: null,
    links: [
      ["mdi-email-outline", "Email"],
      ["mdi-message-outline", "Conversar"],
      ["mdi-checkbox-marked-outline", "Todo"],
      ["mdi-calendar-outline", "Calendário"],
    ],
    value: [0, 80],
    page: 6,
  }),
};
</script>
<style >
#inspire{
  background-color: #F9F9F9;
  font-family: 'Montserrat', sans-serif;
}
#botao {
  border-radius: 10px;
  background:#686868;
  
  font-size:14px;
  margin: 15px;
  width: 140px;
  top: 25px;
  left:-10px
}
.botao1 {
 
  font-size:14px;
color:#E5E5E5;
  border-radius: 10px;
  margin: 15px;
  width: 140px;
  top: 45px;
  left:-10px
  
}

#card1 {
  position: absolute;
  border-radius: 10px;
  margin-left: 400px;
  margin-top: 0px;
}
#card2 {
  position: absolute;
  border-radius: 10px;
  margin-left: 400px;
  margin-top: 160px;
}
#card3 {
  position: absolute;
  border-radius: 10px;
  margin-left: 400px;
  margin-top: 320px;
}
#card4 {
  position: absolute;
  border-radius: 10px;
  border-radius: 10px;
  margin-left: 400px;
  margin-top: 480px;
}
#card5 {
  position: absolute;
  border-radius: 10px;
  margin-left: 400px;
  margin-top: 640px;
}
.form {
  margin-top: -365px;
  margin-left: 20px;
}
#nav-bar {
  background:white;
  margin-left: 314px;
  border-radius: 8px;
  top: 10px;
}
.usuario1 {

  margin-left: 250px;
  font-size: 14px;
  color:#2C2C2C
 
}
.usuario2{
  margin-left: 259px;
  font-size: 11px;
  color:#2C2C2C

}
.btn1 {
  left: 255px;
}
.btn2 {
  left: 240px;
}
#btn3 {
  width: 230px;
 
  font-size: 18px;

  left: 75px;
  background: #696969;
  height: 4%;
  border-radius: 8px;
  
}
#btn4 {
  left: 80px;
  top: -10px;
  background:#787878;
}
.titulo {
  color: #FF7B1B;
  margin-top: -50px;
  margin-left: 55px;
  
  font-size:16px
}
.p {
  font-size: 24px;
  margin-left: 10px;
  
  color:#2C2C2C;
}
.p1 {
  color:#2C2C2C;
  
  margin-left: 340px;
  margin-top: 20px;
  font-size: 18px;
}
.p2 {
  margin-top: 20px;
  margin-left: 3px;
  color:#000000;
  
  font-size: 14px;
}

.divider {
  margin-left: 20px;
}
#icon1 {
  color:#000000;
  margin-left: 10px;
  font-size:20px
  
}

.avatar1 {
  margin-left: 785px;
}
.imagem {
  max-width: 23px;
  max-height: 23px;
}
.menu {
  border-radius: 8px;
  left: 230px;
  background-color:white
}
.view {
  border-radius: 8px;
  left: 220px;
  background-color:white
}
.listagem {
  left: 220px;
  top: 15px;
  border-radius: 8px;
}
#busca {
  background:white;
  
  font-size:22px;
  border-radius: 8px;
  width: 650px;
  margin-left: 410px;
  top: 3px;
}
.valores {
  margin-left: 230px;
  margin-top: -25px;
}

#star1 {
  font-size: 12px;
}
.filtro {
  margin-left: 10px;
  margin-top: 25px;
  
font-size: 18px;
color:#2C2C2C;
}

#check {
  margin-top: -45px;
  margin-left: 300px;
}

.avaliacao {
  margin-top: -40px;
  margin-left: 310px;
}

.dinheiro {
  position: absolute;
  margin-left: -10px;
  margin-top: 50px;
}
#select {
  border-radius: 4px;
  

color:#ECECEC ;
}

.list2{

font-size: 12px;
}
.list3{

font-size: 14px;

}
#icon2{
color:#606060;
}
.div1{
 

font-size: 16px;
}
.toolbar{
  color:#999999;
}
</style>
