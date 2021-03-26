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

      <v-container class="py-8 px-6">
        <v-row>
          <v-card id="card1" outlined>
            <v-list>
              <template>
                <v-list-item>
                  <v-list-item-avatar tile size="170"
                    ><img
                      src="https://s3-alpha-sig.figma.com/img/e45c/591e/213b8d3b1b6988b738678826168031af?Expires=1617580800&Signature=HOM6DAeRV~1u4YoYPU1ESeNf-blO0CSMt5Tp3LgyzeDAFAXKWv0LpaTZd0eyKFSFv~EcvJTSCM10MA45Xp85geU1s6H3ppdQU21626TC2yQ~hYQloKCpW-e2ZSfLN4D3C6iI-JamUjLVg-Dc3QylixRinOntucHeSFR~ZAzAjSL~TyTtukrv1jq84es7ZXWVkTPQ7PvJ1Mdz3IgDuQaLJmKjxbd5TSpGa4pugt-SbbodqO~sAPJZDXcUla1NQho6lB1Gt9cS7vSAUsxWQCOf7ZHXoe-U9tWzljlPPfRbUYqjkhd2DQCq-ngl~JropEnpC8TIsTHwq7USvibLLUduOg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA"
                      alt="logo-img"
                  /></v-list-item-avatar>

                  <v-list-item-content>
                    <div class="div1">Fórmula de Lançamento</div>
                    <v-list-item-title class="list3"
                      >Por <b>Érico Rocha</b></v-list-item-title
                    >

                    <v-list-item-subtitle class="list2">
                      Lorem ipsum dolor sit amet, consectetur adipisicing
                    </v-list-item-subtitle>
                  </v-list-item-content>
                  <v-divider vertical></v-divider>

                  <v-col cols="12" sm="3">
                    <v-btn id="btn4" small dark
                      >3.4<v-icon id="star1">mdi-star-outline</v-icon></v-btn
                    ><v-p class="dinheiro">R$2500</v-p>
                    <v-btn class="botao1"
                      ><v-icon id="icon3">mdi-heart-outline</v-icon><b> Amei</b>
                    </v-btn>
                    <v-btn id="botao" dark
                      ><v-icon id="icon3">mdi-shopping-outline</v-icon> Comprar
                    </v-btn>
                  </v-col>
                </v-list-item>
              </template>
            </v-list>
          </v-card>
        </v-row>
      </v-container>

      <v-container class="py-8 px-6">
        <v-row>
          <v-card id="card2" outlined>
            <v-list>
              <template>
                <v-list-item>
                  <v-list-item-avatar tile size="170"
                    ><img
                      src="https://s3-alpha-sig.figma.com/img/e45c/591e/213b8d3b1b6988b738678826168031af?Expires=1617580800&Signature=HOM6DAeRV~1u4YoYPU1ESeNf-blO0CSMt5Tp3LgyzeDAFAXKWv0LpaTZd0eyKFSFv~EcvJTSCM10MA45Xp85geU1s6H3ppdQU21626TC2yQ~hYQloKCpW-e2ZSfLN4D3C6iI-JamUjLVg-Dc3QylixRinOntucHeSFR~ZAzAjSL~TyTtukrv1jq84es7ZXWVkTPQ7PvJ1Mdz3IgDuQaLJmKjxbd5TSpGa4pugt-SbbodqO~sAPJZDXcUla1NQho6lB1Gt9cS7vSAUsxWQCOf7ZHXoe-U9tWzljlPPfRbUYqjkhd2DQCq-ngl~JropEnpC8TIsTHwq7USvibLLUduOg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA"
                      alt="logo-img"
                  /></v-list-item-avatar>

                  <v-list-item-content>
                    <div class="div1">Fórmula de Lançamento</div>
                    <v-list-item-title class="list3"
                      >Por <b>Érico Rocha</b></v-list-item-title
                    >

                    <v-list-item-subtitle class="list2">
                      Lorem ipsum dolor sit amet, consectetur adipisicing
                    </v-list-item-subtitle>
                  </v-list-item-content>
                  <v-divider vertical></v-divider>
                  <v-col sm="3">
                    <v-btn id="btn4" small dark
                      >3.4<v-icon id="star1">mdi-star-outline</v-icon></v-btn
                    ><v-p class="dinheiro">R$2500</v-p>
                    <v-btn class="botao1"
                      ><v-icon id="icon3">mdi-heart-outline</v-icon>
                      <b> Amei</b>
                    </v-btn>
                    <v-btn id="botao" dark
                      ><v-icon id="icon3">mdi-shopping-outline</v-icon> Comprar
                    </v-btn>
                  </v-col>
                </v-list-item>
              </template>
            </v-list>
          </v-card>
        </v-row>
      </v-container>

      <v-container class="py-8 px-6">
        <v-row>
          <v-card id="card3" outlined>
            <v-list>
              <template>
                <v-list-item>
                  <v-list-item-avatar tile size="170"
                    ><img
                      src="https://s3-alpha-sig.figma.com/img/e45c/591e/213b8d3b1b6988b738678826168031af?Expires=1617580800&Signature=HOM6DAeRV~1u4YoYPU1ESeNf-blO0CSMt5Tp3LgyzeDAFAXKWv0LpaTZd0eyKFSFv~EcvJTSCM10MA45Xp85geU1s6H3ppdQU21626TC2yQ~hYQloKCpW-e2ZSfLN4D3C6iI-JamUjLVg-Dc3QylixRinOntucHeSFR~ZAzAjSL~TyTtukrv1jq84es7ZXWVkTPQ7PvJ1Mdz3IgDuQaLJmKjxbd5TSpGa4pugt-SbbodqO~sAPJZDXcUla1NQho6lB1Gt9cS7vSAUsxWQCOf7ZHXoe-U9tWzljlPPfRbUYqjkhd2DQCq-ngl~JropEnpC8TIsTHwq7USvibLLUduOg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA"
                      alt="logo-img"
                  /></v-list-item-avatar>

                  <v-list-item-content>
                    <div class="div1">Fórmula de Lançamento</div>
                    <v-list-item-title class="list3"
                      >Por <b>Érico Rocha</b></v-list-item-title
                    >

                    <v-list-item-subtitle class="list2">
                      Lorem ipsum dolor sit amet, consectetur adipisicing
                    </v-list-item-subtitle>
                  </v-list-item-content>
                  <v-divider vertical></v-divider>
                  <v-col sm="3">
                    <v-btn id="btn4" small dark
                      >3.4<v-icon id="star1">mdi-star-outline</v-icon></v-btn
                    >
                    <v-p class="dinheiro">R$2500</v-p>
                    <v-btn class="botao1"
                      ><v-icon id="icon3">mdi-heart-outline</v-icon>
                      <b> Amei</b>
                    </v-btn>
                    <v-btn id="botao" dark
                      ><v-icon id="icon3">mdi-shopping-outline</v-icon> Comprar
                    </v-btn>
                  </v-col>
                </v-list-item>
              </template>
            </v-list>
          </v-card>
        </v-row>
      </v-container>

      <v-container class="py-8 px-6">
        <v-row>
          <v-card id="card4" outlined>
            <v-list>
              <template>
                <v-list-item>
                  <v-list-item-avatar tile size="170"
                    ><img
                      src="https://s3-alpha-sig.figma.com/img/e45c/591e/213b8d3b1b6988b738678826168031af?Expires=1617580800&Signature=HOM6DAeRV~1u4YoYPU1ESeNf-blO0CSMt5Tp3LgyzeDAFAXKWv0LpaTZd0eyKFSFv~EcvJTSCM10MA45Xp85geU1s6H3ppdQU21626TC2yQ~hYQloKCpW-e2ZSfLN4D3C6iI-JamUjLVg-Dc3QylixRinOntucHeSFR~ZAzAjSL~TyTtukrv1jq84es7ZXWVkTPQ7PvJ1Mdz3IgDuQaLJmKjxbd5TSpGa4pugt-SbbodqO~sAPJZDXcUla1NQho6lB1Gt9cS7vSAUsxWQCOf7ZHXoe-U9tWzljlPPfRbUYqjkhd2DQCq-ngl~JropEnpC8TIsTHwq7USvibLLUduOg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA"
                      alt="logo-img"
                  /></v-list-item-avatar>

                  <v-list-item-content>
                    <div class="div1">Fórmula de Lançamento</div>
                    <v-list-item-title class="list3"
                      >Por <b>Érico Rocha</b></v-list-item-title
                    >

                    <v-list-item-subtitle class="list2">
                      Lorem ipsum dolor sit amet, consectetur adipisicing
                    </v-list-item-subtitle>
                  </v-list-item-content>
                  <v-divider vertical></v-divider>
                  <v-col sm="3">
                    <v-btn id="btn4" small dark
                      >3.4<v-icon id="star1">mdi-star-outline</v-icon></v-btn
                    >
                    <v-p class="dinheiro">R$2500</v-p>
                    <v-btn class="botao1"
                      ><v-icon id="icon3">mdi-heart-outline</v-icon><b> Amei</b>
                    </v-btn>
                    <v-btn id="botao" dark
                      ><v-icon id="icon3">mdi-shopping-outline</v-icon> Comprar
                    </v-btn>
                  </v-col>
                </v-list-item>
              </template>
            </v-list>
          </v-card>
        </v-row>
      </v-container>

      <v-container class="py-8 px-6">
        <v-row>
          <v-card id="card5" outlined>
            <v-list>
              <template>
                <v-list-item>
                  <v-list-item-avatar tile size="170"
                    ><img
                      src="https://s3-alpha-sig.figma.com/img/e45c/591e/213b8d3b1b6988b738678826168031af?Expires=1617580800&Signature=HOM6DAeRV~1u4YoYPU1ESeNf-blO0CSMt5Tp3LgyzeDAFAXKWv0LpaTZd0eyKFSFv~EcvJTSCM10MA45Xp85geU1s6H3ppdQU21626TC2yQ~hYQloKCpW-e2ZSfLN4D3C6iI-JamUjLVg-Dc3QylixRinOntucHeSFR~ZAzAjSL~TyTtukrv1jq84es7ZXWVkTPQ7PvJ1Mdz3IgDuQaLJmKjxbd5TSpGa4pugt-SbbodqO~sAPJZDXcUla1NQho6lB1Gt9cS7vSAUsxWQCOf7ZHXoe-U9tWzljlPPfRbUYqjkhd2DQCq-ngl~JropEnpC8TIsTHwq7USvibLLUduOg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA"
                      alt="logo-img"
                  /></v-list-item-avatar>

                  <v-list-item-content>
                    <div class="div1">Fórmula de Lançamento</div>
                    <v-list-item-title class="list3"
                      >Por <b>Érico Rocha</b></v-list-item-title
                    >

                    <v-list-item-subtitle class="list2">
                      Lorem ipsum dolor sit amet, consectetur adipisicing
                    </v-list-item-subtitle>
                  </v-list-item-content>
                  <v-divider vertical></v-divider>
                  <v-col sm="3">
                    <v-btn id="btn4" small dark
                      >3.4<v-icon id="star1">mdi-star-outline</v-icon></v-btn
                    >
                    <v-p class="dinheiro">R$2500</v-p>
                    <v-btn class="botao1"
                      ><v-icon id="icon3">mdi-heart-outline</v-icon>
                      <b> Amei</b>
                    </v-btn>
                    <v-btn id="botao" dark
                      ><v-icon id="icon3">mdi-shopping-outline</v-icon> Comprar
                    </v-btn>
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
          <v-card id="form" outlined>
            <v-container>
              <v-p class="p3"><b>Preços</b></v-p>
              <v-radio-group>
                <v-radio label="R$10" color="#969696" value="radio-1"></v-radio>
                <v-radio
                  label="R$10-R$100"
                  color="#969696"
                  value="radio-2"
                ></v-radio>
                <v-radio
                  label="R$100-R$500"
                  color="#969696"
                  value="radio-3"
                ></v-radio>
                <v-radio
                  label="R$500"
                  color="#969696"
                  value="radio-4"
                ></v-radio>
                <v-radio
                  label="Todos"
                  color="#969696"
                  value="radio-5"
                ></v-radio>
              </v-radio-group>
              <v-divider></v-divider>
            </v-container>
            <v-container>
              <v-p class="p3"><b>Valores</b></v-p>
              <v-p class="valores"><b>1.99 - 4098</b></v-p>
              <v-card-text>
                <v-range-slider
                  v-model="value"
                  step="10"
                  color="#606060"
                ></v-range-slider>
              </v-card-text>
              <v-divider></v-divider>
            </v-container>

            <v-container>
              <v-p class="p3"><b>Categorias</b></v-p>

              <v-checkbox label="Érico Rocha" color="#969696"></v-checkbox>
              <p id="check">1920</p>
              <v-checkbox label="Desafio 6 em 7" color="#969696"></v-checkbox>
              <p id="check">1820</p>
              <v-checkbox
                label="Fórmula de Lançamento"
                color="#969696"
              ></v-checkbox>
              <p id="check">462</p>
              <v-checkbox label="KlickPages " color="#969696"></v-checkbox>
              <p id="check">6556</p>
              <v-checkbox label="Audios" color="#969696"></v-checkbox>
              <p id="check">120</p>

              <v-divider></v-divider>
            </v-container>

            <v-container>
              <v-p class="p3"><b>Avaliação</b></v-p>
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
    <br /><br><br>

    <v-col cols="12" sm="11">
      <div class="pagina">
        <v-pagination
          v-model="page"
          :length="10"
          color="#969696"
          circle
        ></v-pagination>
      </div>
    </v-col>

    <br />
  </v-app>
</template>


<script>
export default {
  data: () => ({
    drawer: null,
    links: [
      ["mdi-email-outline", "E-mail"],
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
#inspire {
  background-color: #f9f9f9;
  font-family: "Montserrat", sans-serif;
}
#botao {
  border-radius: 10px;
  background: #686868;

  font-size: 14px;
  margin: 10%;
  width: 110%;
  margin-top: -3%;
  margin-left: 3%;
}
.botao1 {
  font-size: 14px;
  color: #e5e5e5;
  border-radius: 10px;
  margin: 10%;
  width: 110%;
  margin-top: 60%;
  margin-left: 3%;
}

#card1 {
  position: absolute;
  width: 60.5%;
  border-radius: 10px;
  margin-left: 37.5%;
  
}
#card2 {
  position: absolute;
  width: 60.5%;
  border-radius: 10px;
  margin-left: 37.5%;
  margin-top: 18%;
}
#card3 {
  position: absolute;
  width: 60.5%;
  border-radius: 10px;
  margin-left: 37.5%;
  margin-top: 36%;
}
#card4 {
  position: absolute;
  width: 60.5%;
  border-radius: 10px;
  border-radius: 10px;
  margin-left: 37.5%;
  margin-top: 54%;
}
#card5 {
  position: absolute;
  width: 60.5%;
  border-radius: 10px;
  margin-left: 37.5%;
  margin-top: 72%;
}
#form {
  width:35%; 
  height:1333px; 
  margin-top: -365px;
  margin-left: 20px;
  border-radius: 8px;
}
#nav-bar {
  background: white;
  width:76%;
  margin-left: 23%;
  border-radius: 8px;
  top: 15%;
}
.usuario1 {
  margin-left:77%;
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
  left:24% ;
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
  left:70%;
  top: -10px;
  background: #787878;
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

  margin-left: 33%;
  margin-top: 20px;
  font-size: 18px;
}
.p2 {
  margin-top: 2%;
  margin-left: 0.5%;
  color: #000000;

  font-size: 14px;
}
.p3 {
  font-size: 18px;
}

.divider {
  margin-left: 2%;
}
#icon1 {
  color: #000000;
  margin-left: 1%;
  font-size: 20px;
}
#icon3 {
  font-size: 16px;
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
  left: 15.5%;
  background-color: white;
}
.view {
  border-radius: 8px;
  left: 14.5%;
  background-color: white;
}
.listagem {
  left: 103%;
  top: 15px;
  border-radius: 8px;
}
#busca {
  background: white;

  font-size: 22px;
  border-radius: 8px;
  width: 60.5%;
  margin-left: 38.5%;
  top: 3px;
}
.valores {
  margin-left: 48%;
  margin-top: -25px;
  font-size: 20px;
}

#star1 {
  font-size: 12px;
}
.filtro {
  margin-left: 1%;
  margin-top:3%;

  font-size: 18px;
  color: #2c2c2c;
}
#check1 {
  background-color: #2c2c2c;
}

#check {
  margin-top: -15%;
  margin-left: 87%;
  font-size: 14px;
}

.avaliacao {
  margin-top: -12%;
  margin-left: 85%;
  font-size: 14px;
}

.dinheiro {
  position: absolute;
  margin-left: -3%;
  margin-top: 8%;
  font-size: 110%;
}
#select {
  border-radius: 4px;

  color: #ececec;
}
.list1 {
  color: #2c2c2c;
}

.list2 {
  font-size: 12px;
}
.list3 {
  font-size: 14px;
}
#icon2 {
  color: #606060;
}
.div1 {
  font-size: 16px;
}
.toolbar {
  color: #999999;
}
.app {
  color: #999999;
  font-size: 14px;
}
.pagina {
  margin-left: 350px; 
}
.logo-avatar{
  margin-left:0%;
}
</style>
