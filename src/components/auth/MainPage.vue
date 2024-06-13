<template>
  <div class="q-pa">
    <q-toolbar class="bg-black text-white">
      <q-btn flat label="Guitar Pro Store" />
      <q-space />

      <q-tabs v-model="tab" shrink>
        <q-tab name="tab1" label="Inicio" />
        <q-tab name="tab2" label="Guitarras" />
        <q-tab name="tab3" label="Contacto" />
      </q-tabs>
    </q-toolbar>
  </div>

  <div class="q-pa-md flex justify-center">
    <div class="q-gutter-md q-flex justify-center">
      <q-input
        v-model="search"
        debounce="500"
        filled
        placeholder="Buscar guitarra"
        dense
        style="max-width: 250px"
      >
        <template v-slot:append>
          <q-icon name="search" />
        </template>
      </q-input>
    </div>
  </div>

  <div class="q-pa-md row items-start q-gutter-md justify-center">
    <q-card class="my-card">
      <img src="https://audiomusica.vtexassets.com/arquivos/ids/160415/1109500-1.jpg?v=638333390457730000" />

      <q-card-section>
        <div class="text-h6">Guitarra eléctrica G&L S-500 Jet Black MN</div>
        <div class="text-subtitle2">G&L</div>
        <div class="text-subtitle2">S/ 13,999.00</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://audiomusica.vtexassets.com/arquivos/ids/160538-300-300?v=638334448590100000&width=300&height=300&aspect=true" />

      <q-card-section>
        <div class="text-h6">Guitarra eléctrica G&L S-500 Graphite Metallic</div>
        <div class="text-subtitle2">G&L</div>
        <div class="text-subtitle2">S/ 13,999.00</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://audiomusica.vtexassets.com/arquivos/ids/161369-300-300?v=638483658223300000&width=300&height=300&aspect=true" />

      <q-card-section>
        <div class="text-h6">Guitarra eléctrica G&L S-500 Tobacco</div>
        <div class="text-subtitle2">G&L</div>
        <div class="text-subtitle2">S/ 13,999.00</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://audiomusica.vtexassets.com/arquivos/ids/160548-300-300?v=638334448636370000&width=300&height=300&aspect=true" />

      <q-card-section>
        <div class="text-h6">Guitarra eléctrica G&L Legacy HSS Old</div>
        <div class="text-subtitle2">G&L</div>
        <div class="text-subtitle2">S/ 12,999.00</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ xd }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://audiomusica.vtexassets.com/arquivos/ids/161280-300-300?v=638453506277770000&width=300&height=300&aspect=true" />

      <q-card-section>
        <div class="text-h6">Guitarra eléctrica G&L Legacy HSS Jet Black</div>
        <div class="text-subtitle2">G&L</div>
        <div class="text-subtitle2">S/ 12,999.00</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://audiomusica.vtexassets.com/arquivos/ids/160542-300-300?v=638334448607500000&width=300&height=300&aspect=true" />

      <q-card-section>
        <div class="text-h6">Guitarra eléctrica G&L Asat Classic Alnico</div>
        <div class="text-subtitle2">G&L</div>
        <div class="text-subtitle2">S/ 12,999.00</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://audiomusica.vtexassets.com/arquivos/ids/160537-300-300?v=638334448586900000&width=300&height=300&aspect=true" />

      <q-card-section>
        <div class="text-h6">Guitarra eléctrica G&L Legacy HSS Midnight</div>
        <div class="text-subtitle2">G&L</div>
        <div class="text-subtitle2">S/ 12,999.00</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://audiomusica.vtexassets.com/arquivos/ids/160541-300-300?v=638334448604770000&width=300&height=300&aspect=true" />

      <q-card-section>
        <div class="text-h6">Guitarra eléctrica G&L Asat Classic 3 Tone</div>
        <div class="text-subtitle2">G&L</div>
        <div class="text-subtitle2">S/ 12,999.00</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://audiomusica.vtexassets.com/arquivos/ids/160545-300-300?v=638334448626130000&width=300&height=300&aspect=true" />

      <q-card-section>
        <div class="text-h6">Guitarra eléctrica G&L Asat Classic Thinline</div>
        <div class="text-subtitle2">G&L</div>
        <div class="text-subtitle2">S/ 11,599.00</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://audiomusica.vtexassets.com/arquivos/ids/160543-300-300?v=638334448609930000&width=300&height=300&aspect=true" />

      <q-card-section>
        <div class="text-h6">Guitarra eléctrica G&L Asat Classic M2</div>
        <div class="text-subtitle2">G&L</div>
        <div class="text-subtitle2">S/ 11,599.00</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://audiomusica.vtexassets.com/arquivos/ids/160544-300-300?v=638334448613800000&width=300&height=300&aspect=true" />

      <q-card-section>
        <div class="text-h6">Guitarra eléctrica G&L Asat Classic Sunburst</div>
        <div class="text-subtitle2">G&L</div>
        <div class="text-subtitle2">S/ 11,599.00</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <img src="https://audiomusica.vtexassets.com/arquivos/ids/161054-300-300?v=638430027335400000&width=300&height=300&aspect=true" />

      <q-card-section>
        <div class="text-h6">Guitarra eléctrica Ibanez AZ2402</div>
        <div class="text-subtitle2">Ibanez</div>
        <div class="text-subtitle2">S/ 9,999.00</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>
  </div>

  <div class="q-pa-lg flex flex-center">
    <q-pagination v-model="current" :max="5" direction-links />
  </div>
</template>

<style lang="sass" scoped>

.my-card
  width: 100%
  max-width: 250px
  margin-left: 18px
  margin-right: 18px
</style>
