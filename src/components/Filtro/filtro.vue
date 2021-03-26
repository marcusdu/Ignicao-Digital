<template>
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
</template>
<script>
export default {
    data: () => ({
        value: [0, 80]
    })
}
</script>
<style>
#form {
  width: 35%;
  height: 1333px;
  margin-top: -365px;
  margin-left: 20px;
  border-radius: 8px;
}
#btn3 {
  width: 70%;

  font-size: 18px;

  margin-left: 15%;
  background: #696969;
  height: 4%;
  border-radius: 8px;
}
.p3 {
  font-size: 18px;
}
.valores {
  margin-left: 48%;
  margin-top: -25px;
  font-size: 20px;
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
</style>