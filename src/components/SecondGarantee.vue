<template>
  <div id="SecondGarantee">
    <div class="container-fluid" style="background-color: #f5f5f5; height: 100vh">
      <div
        class="row mb-2 pt-3 pl-3 pr-3 pb-2"
        style="background-color: #FFFFFF"
      >
        <div class="col-1 p-0" style="min-width: 5em">
          <img class="logo" src="../svg/logo_bg.svg" style="width: 100%" />
        </div>
        <div class="col-8 pl-3">
          <div class="h1" style="line-height: 0.6; ">Банковские гарантии</div>
        </div>
        <div class="col d-flex justify-content-end">
          <a class="prev-button mr-1" @click='arrowPrev'> </a>
          <a class="next-button" @click='arrowNext'> </a>
        </div>
      </div>
      <div class="m-1 d-flex flex-column justify-content-between" style="height: calc(100vh - 2.5em - 2em)">
        <div class="row h5">
          <div class="col"></div>
          <div class="col">
            На текущий день
          </div>
          <div class="col p-0">
            Динамика месяца
          </div>
          <div class="col">
            Доля рынка
          </div>
        </div>

        <div class="row white pt-2 flex-fill">
          <div
            class="col my-auto h5 text-uppercase"
            style="font-weight: normal"
          >
            Объем <strong>портфеля</strong>
          </div>

          <div class="col my-auto num">
            <div class="row">
              <div class="col bigDigits">17.8 <span class="h5">млрд</span></div>
              <!-- не нашёл переменной -->
            </div>
            <div class="row">
              <div class="col decrease h5">
                32%
                <!-- {{ strict(data.plan) }}% -->
              </div>
              <div class="col increase h5">
                104%
                <!-- {{ strict(data.year) }}% -->
              </div>
            </div>
            <div class="row">
              <small class="text-uppercase col">от плана</small>
              <small class="text-uppercase col text-center">за год</small>
            </div>
          </div>

          <div class="col my-auto num">
            <div class="row">
              <div class="col bigDigits">1.1 <span class="h5">млрд</span></div>
              <!-- не нашёл переменной -->
            </div>
            <div class="row">
              <div class="col decrease h5">
                85%
                <!-- {{ strict(data.plan) }}% -->
              </div>
              <div class="col increase h5">
                406%
                <!-- {{ strict(data.year) }}% -->
              </div>
            </div>
            <div class="row">
              <small class="text-uppercase col">от плана</small>
              <small class="text-uppercase col text-center">за год</small>
            </div>
          </div>
          <div class="col my-auto num">
            <div class="row">
              <div class="col bigDigits">2.9%</div>
              <!-- не нашёл переменной -->
            </div>
            <div class="row">
              <div class="col increase2 h5">
                192%
                <!-- {{ strict(data.plan) }}% -->
              </div>
              <div class="col increase h5">
                4%
                <!-- {{ strict(data.year) }}% -->
              </div>
            </div>
            <div class="row">
              <small class="text-uppercase col"
                >наша доля
                <p class="m-0">за год</p></small
              >
              <small class="text-uppercase col text-center"
                >рынок
                <p class="m-0" >за год</p></small
              >
            </div>
          </div>
        </div>

        <div class="row white pt-2 flex-fill mt-2 mb-2">
          <div
            class="col my-auto h5 text-uppercase"
            style="font-weight: normal;"
          >
            Количество <strong>сделок</strong>
          </div>

          <div class="col my-auto num">
            <div class="row">
              <div class="col bigDigits">18.1 <span class="h5">млрд</span></div>
              <!-- не нашёл переменной -->
            </div>
            <div class="row">
              <div class="col decrease h5">
                16%
                <!-- {{ strict(data.plan) }}% -->
              </div>
              <div class="col increase h5">
                46%
                <!-- {{ strict(data.year) }}% -->
              </div>
            </div>
            <div class="row">
              <small class="text-uppercase col">от плана</small>
              <small class="text-uppercase col text-center">за год</small>
            </div>
          </div>

          <div class="col my-auto num">
            <div class="row">
              <div class="col bigDigits">2.3 <span class="h5">тыс</span></div>
              <!-- не нашёл переменной -->
            </div>
            <div class="row">
              <div class="col decrease h5">
                13%
                <!-- {{ strict(data.plan) }}% -->
              </div>
              <div class="col increase h5">
                13%
                <!-- {{ strict(data.year) }}% -->
              </div>
            </div>
            <div class="row">
              <small class="text-uppercase col">от плана</small>
              <small class="text-uppercase col text-center">за год</small>
            </div>
          </div>
          <div class="col my-auto num">
            <div class="row">
              <div class="col bigDigits">15.6%</div>
              <!-- не нашёл переменной -->
            </div>
            <div class="row">
              <div class="col decrease h5">
                21%
                <!-- {{ strict(data.plan) }}% -->
              </div>
              <div class="col increase h5">
                68%
                <!-- {{ strict(data.year) }}% -->
              </div>
            </div>
            <div class="row">
              <small class="text-uppercase col"
                >наша доля
                <p class="m-0">за год</p></small
              >
              <small class="text-uppercase col text-center"
                >рынок
                <p class="m-0">за год</p></small
              >
            </div>
          </div>
        </div>

        <div class="row white pt-2 pb-2 mb-1 flex-fill">
          <div
            class="col my-auto h5 text-uppercase"
            style="font-weight: normal;"
          >
            Сделки по <strong>новым клиентам</strong>
          </div>
          <div class="col bigDigits my-auto">14.4 <span class="h5">тыс</span></div>
          <div class="col bigDigits my-auto">0.7</div>
          <div class="col"></div>
        </div>

        <!-- <div class="row" style="height: 250px;margin-top: 10px;">
          <div
            class="col-md-2 title"
            style="margin-top:auto;margin-bottom: auto;font-size: 40px;"
          >
            Количество сделок
          </div>
          <div class="col-md-10 white" style="height: 100%; padding: 20px;">
            <div class="row">
              <div
                class="col-md-4"
                style="background-color:#fff;"
                ng-repeat="data in sdelki2"
              >
                <div class="row">
                  <div
                    class="col-md-12 h1 hand"
                    ng-bind-html="abbreviateNumber(data.value, 1)"
                    data-ng-attr-title="{{declension(data.value, ['сделка', 'сделки', 'сделок'])}}"
                  ></div>
                </div>
                <div class="row">
                  <div
                    class="col-md-5 {{data.plan < 100 ? 'decrease2' : 'increase2'}}"
                  >
                    {{ strict(data.plan) }}%
                  </div>
                  <div
                    class="col-md-5 {{data.year < 0 ? 'decrease' : 'increase'}}"
                  >
                    {{ strict(data.year) }}%
                  </div>
                </div>
                <div class="row">
                  <div class="col-md-5 h3">от плана</div>
                  <div class="col-md-5 h3">за год</div>
                </div>
              </div>

              <div class="col-md-4" style="background-color:#fff;">
                <div class="row">
                  <div
                    class="col-md-12 h1"
                    ng-bind-html="percentStyle(market[1].value, 1)"
                  ></div>
                </div>
              </div>
            </div>
          </div>
        </div> -->
        <!-- <div class="row" style="height: 250px;margin-top: 10px;">
          <div
            class="col-md-2 title"
            style="margin-top:auto;margin-bottom: auto;font-size: 40px;"
          >
            Сделки по новым клиентам
          </div>
          <div class="col-md-10 white" style="height: 100%; padding: 20px;">
            <div class="row">
              <div
                class="col-md-4"
                style="background-color:#fff;"
                ng-repeat="data in new_sdelki"
              >
                <div class="row">
                  <div
                    class="col-md-12 h1"
                    ng-bind-html="abbreviateNumber(data.value, 1)"
                    data-ng-attr-title="{{declension(data.value, ['сделка', 'сделки', 'сделок'])}}"
                  ></div>
                </div>
              </div>
            </div>
          </div>
        </div> -->
      </div>
    </div>
  </div>
</template>

<script>
// import { BCard } from "bootstrap-vue";

export default {
  name: "SecondGarantee",
  data() {
    return {
      comissions: [
        { label: "Сегодня", value: 1098754 },
        { label: "Вчера", value: 257272 },
        { label: "Неделю назад", value: 1402503 },
        { label: "Год назад", value: 2974769 }
      ],
      sdelki: [
        { value: 70, avg_cheque: "" },
        { value: 2, avg_cheque: "" }
      ],
      rest: [{ value: 2 }, { value: 10 }]
    };
  },
  methods: {
     arrowPrev() { 
      this.$emit('arrowClick', 'prev')
    },
    arrowNext() { 
      this.$emit('arrowClick', 'next')
    },
    getPercent(array, value, key) {
      var max = 0;
      array.forEach(item => {
        max = item[key] > max ? item[key] : max;
      });
      console.log((value * 100) / max + "%");
      return (value * 100) / max + +"%";
    }
  },
  computed: {
    comissionsWithoutFirst() {
      return this.comissions.filter(e => this.comissions.indexOf(e) > 0);
    }
  }
};
</script>

<style>
.white {
  background-color: #ffffff;
  border-radius: 20px;
}

div.col.my-auto.num {
  padding-bottom: 2rem;
}
/* .white:nth-child(2n+1) {
  margin-top: 1rem;
} */

/* html {
  font-size: 40px;
  font-family: Roboto-Bold;
}
* {
  font-weight: bold !important;
}

@media screen and (max-width: 1281px) {
  html {
    font-size: 20px;
  }
}

.prev-button,
.next-button {
  display: block;
  width: 2em;
  height: 2em;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  opacity: 0.5;
  background-size: 2em 2em;
}

.prev-button:hover,
.next-button:hover {
  opacity: 1;
  cursor: pointer;
}

.prev-button {
  background-image: url("./svg/arrow-left.svg");
}
.next-button {
  background-image: url("./svg/arrow-right.svg");
}

.bigDigits {
  font-size: 3em;
}
.progress-bar {
  border-radius: 20px;
  background-color: #503aeb;
}

.text-uppercase {
} */
</style>
