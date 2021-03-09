<template>
  <div class="flex-col max-w-prose form-container">
    <!--
  This example requires Tailwind CSS v2.0+ 
  
  This example requires some changes to your config:
  
  ```
  // tailwind.config.js
  module.exports = {
    // ...
    plugins: [
      // ...
      require('@tailwindcss/forms'),
    ]
  }
  ```
-->
    <h1 class="text-6xl opacity-50 py-10">PERFIL NUTRICIONAL</h1>

    <div class="mt-10 sm:mt-0">
      <div class="md:grid md:grid-cols-3 md:gap-6">
        <div class="md:col-span-1">
          <div class="px-4 sm:px-0">
            <h3 class="text-lg font-medium leading-6 text-gray-900">
              DATOS PERSONALES
            </h3>
            <p class="mt-1 text-xl text-gray-600">
              Algunos datos para conocerte mejor.
            </p>
          </div>
        </div>
        <div class="mt-5 md:mt-0 md:col-span-2">
          <form action="#" method="POST">
            <div class="shadow overflow-hidden sm:rounded-md">
              <div class="bg-orange-300 px-4 py-5 bg-white sm:p-6">
                <div class="grid grid-cols-12 gap-6">
                  <div class="col-span-6 sm:col-span-3">
                    <label
                      for="first_name"
                      class="block text-sm font-medium text-gray-700"
                      >Nombre</label
                    >
                    <input
                      type="text"
                      name="first_name"
                      id="first_name"
                      autocomplete="given-name"
                      class="mt-1 focus:ring-indigo-500 focus:border-indigo-500 block w-full shadow-sm sm:text-sm border-gray-300 rounded-md"
                    />
                  </div>

                  <div class="col-span-6 sm:col-span-3">
                    <label
                      for="last_name"
                      class="block text-sm font-medium text-gray-700"
                      >Apellido</label
                    >
                    <input
                      type="text"
                      name="last_name"
                      id="last_name"
                      autocomplete="family-name"
                      class="mt-1 focus:ring-indigo-500 focus:border-indigo-500 block w-full shadow-sm sm:text-sm border-gray-300 rounded-md"
                    />
                  </div>

                  <div class="col-span-6 sm:col-span-4">
                    <label
                      for="email_address"
                      class="block text-sm font-medium text-gray-700"
                      >Email</label
                    >
                    <input
                      type="text"
                      name="email_address"
                      id="email_address"
                      autocomplete="email"
                      class="mt-1 focus:ring-indigo-500 focus:border-indigo-500 block w-full shadow-sm sm:text-sm border-gray-300 rounded-md"
                    />
                  </div>

                  <div class="col-span-6 sm:col-span-4">
                    <label
                      for="phone"
                      class="block text-sm font-medium text-gray-700"
                      >Teléfono / Whatsapp
                    </label>
                    <input
                      type="text"
                      name="phone"
                      id="phone"
                      autocomplete="email"
                      class="mt-1 focus:ring-indigo-500 focus:border-indigo-500 block w-full shadow-sm sm:text-sm border-gray-300 rounded-md"
                    />
                  </div>
                  <div class="col-span-6 sm:col-span-4">
                    <label
                      for="birth_date"
                      class="block text-sm font-medium text-gray-700"
                      >Fecha de nacimiento
                    </label>
                    <input
                      type="date"
                      name="birth_date"
                      id="birth_date"
                      autocomplete="email"
                      class="mt-1 focus:ring-indigo-500 focus:border-indigo-500 block w-full shadow-sm sm:text-sm border-gray-300 rounded-md"
                    />
                  </div>
                </div>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>

    <div class="hidden sm:block" aria-hidden="true">
      <div class="py-5">
        <div class="border-t border-gray-200"></div>
      </div>
    </div>

    <div>
      <div class="mt-5 md:grid md:grid-cols-3 md:gap-6">
        <div class="md:col-span-1">
          <div class="px-4 sm:px-0">
            <h3 class="text-lg font-medium leading-6 text-gray-900">
              CARACTERISTICAS PERSONALES
            </h3>
            <p class="mt-1 text-xl text-gray-600">
              Armamos el plan a tu medida.
            </p>
          </div>
        </div>
        <div class="mt-5 md:mt-0 md:col-span-2">
          <form action="#" method="POST">
            <div class="shadow sm:rounded-md sm:overflow-hidden">
              <div class="bg-orange-300 px-4 py-5 bg-white space-y-6 sm:p-6">
                <div class="grid grid-cols-12 gap-6">
                  <div class="grid gap-x-1 col-span-3 sm:col-span-3">
                    <label
                      for="actual_weight"
                      class="col-span-12 block text-sm font-medium text-gray-700"
                      >Peso actual</label
                    >
                    <select
                      id="actual_weight"
                      name="actual_weight"
                      autocomplete="actual_weight"
                      class="col-span-6 mt-1 py-2 px-3 border border-gray-300 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm"
                    >
                      <option v-for="(v, index) in 271" :key="index">
                        {{ index + 30 }}
                      </option>
                    </select>
                    <select
                      id="actual_weight"
                      name="actual_weight"
                      autocomplete="actual_weight"
                      class="col-span-6 mt-1 py-2 px-3 border border-gray-300 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm"
                    >
                      <option v-for="(v, index) in 9" :key="index">
                        {{ `${index + 1}00` }}
                      </option>
                    </select>
                  </div>
                  <div class="grid gap-x-1 col-span-3 sm:col-span-3">
                    <label
                      for="actual_height"
                      class="col-span-12 block text-sm font-medium text-gray-700"
                      >Altura</label
                    >
                    <select
                      id="actual_height"
                      name="actual_height"
                      autocomplete="actual_height"
                      class="col-span-6 mt-1 py-2 px-3 border border-gray-300 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm"
                    >
                      <option v-for="(v, index) in 2" :key="index">
                        {{ index + 1 }}
                      </option>
                    </select>
                    <select
                      id="actual_height"
                      name="actual_height"
                      autocomplete="actual_height"
                      class="col-span-6 mt-1 py-2 px-3 border border-gray-300 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm"
                    >
                      <option v-for="(v, index) in 9" :key="index">
                        {{ `${index + 1}00` }}
                      </option>
                    </select>
                  </div>
                  <div class="grid gap-x-1 col-span-3 sm:col-span-3">
                    <label
                      for="how_much"
                      class="col-span-12 block text-sm font-medium text-gray-700"
                      >¿Cuanto queres adelgazar?</label
                    >
                    <select
                      id="how_much"
                      name="how_much"
                      autocomplete="how_much"
                      class="col-span-12 mt-1 py-2 px-3 border border-gray-300 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm"
                    >
                      <option v-for="(v, index) in 150" :key="index">
                        {{ index + 1 }}
                      </option>
                    </select>
                  </div>
                  <div class="grid gap-x-1 col-span-3 sm:col-span-3">
                    <label
                      for="overweight_years"
                      class="col-span-12 block text-sm font-medium text-gray-700"
                      >Años con sobrepeso</label
                    >
                    <select
                      id="overweight_years"
                      name="overweight_years"
                      autocomplete="overweight_years"
                      class="col-span-12 mt-1 py-2 px-3 border border-gray-300 bg-white rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm"
                    >
                      <option>Menos de 1 año</option>
                      <option>Entre 1 y 5 años</option>
                      <option>Entre 5 y 10 años</option>
                      <option>Entre 10 y 15 años</option>
                      <option>Entre 15 y 20 años</option>
                      <option>Más de 20 años</option>
                    </select>
                  </div>
                </div>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>

    <div class="hidden sm:block" aria-hidden="true">
      <div class="py-5">
        <div class="border-t border-gray-200"></div>
      </div>
    </div>

    <div class="mt-5 sm:mt-0">
      <div class="md:grid md:grid-cols-3 md:gap-6">
        <div class="md:col-span-1">
          <div class="px-4 sm:px-0">
            <h3 class="text-lg font-medium leading-6 text-gray-900">
              OTROS DATOS
            </h3>
          </div>
        </div>
        <div class="mt-5 md:mt-0 md:col-span-2">
          <form action="#" method="POST">
            <div class="shadow overflow-hidden sm:rounded-md">
              <div class="px-4 py-5 bg-orange-300 space-y-6 sm:p-6">
                <fieldset>
                  <div>
                    <legend class="text-base font-medium text-gray-700">
                      ¿Cómo es la cicunferencia de su muñeca?
                    </legend>
                  </div>
                  <div
                    class="mt-4 grid grid-cols-3 gap-x-5 place-items-start place-content-center"
                  >
                    <div class="flex items-center">
                      <input
                        id="push_everything"
                        name="push_notifications"
                        type="radio"
                        class="focus:ring-indigo-500 h-4 w-4 text-indigo-600 border-gray-300"
                      />
                      <label
                        for="push_everything"
                        class="ml-3 block text-sm font-medium text-gray-900"
                      >
                        <img
                          src="https://imagenes2.dietascormillot.com/front//circunferencia-chica.jpg"
                          alt=""
                        />
                        <p class="text-xl uppercase">Chica</p>
                        <p class="text-gray-700">
                          Si un dedo sobrepasa el otro, la circunferencia es
                          pequeña.
                        </p>
                      </label>
                    </div>
                    <div class="flex items-center">
                      <input
                        id="push_email"
                        name="push_notifications"
                        type="radio"
                        class="focus:ring-indigo-500 h-4 w-4 text-indigo-600 border-gray-300"
                      />
                      <label
                        for="push_email"
                        class="ml-3 block text-sm font-medium text-gray-900"
                      >
                        <img
                          src="https://imagenes2.dietascormillot.com/front//circunferencia-med.jpg"
                          alt=""
                        />
                        <p class="text-xl uppercase">Mediana</p>
                        <p class="text-gray-700">
                          Si se tocan, la circunferencia es mediana.
                        </p>
                      </label>
                    </div>
                    <div class="flex items-center">
                      <input
                        id="push_nothing"
                        name="push_notifications"
                        type="radio"
                        class="focus:ring-indigo-500 h-4 w-4 text-indigo-600 border-gray-300"
                      />
                      <label
                        for="push_nothing"
                        class="ml-3 block text-sm font-medium text-gray-900"
                      >
                        <img
                          src="https://imagenes2.dietascormillot.com/front//circunferencia-grande.jpg"
                          alt=""
                        />
                        <p class="text-xl uppercase">Grande</p>
                        <p class="text-gray-700">
                          Si se tocan, la circunferencia es mediana.
                        </p>
                      </label>
                    </div>
                  </div>
                </fieldset>

                <fieldset>
                  <legend class="text-base font-medium text-gray-700">
                    ¿Te encuentras en alguna de estas etapas de la vida?
                  </legend>
                  <div class="mt-4 grid grid-cols-3">
                    <div class="flex items-start">
                      <div class="flex items-center h-5">
                        <input
                          id="comments"
                          name="comments"
                          type="checkbox"
                          class="focus:ring-indigo-500 h-4 w-4 text-indigo-600 border-gray-300 rounded"
                        />
                      </div>
                      <div class="ml-3 text-sm">
                        <label for="comments" class="font-medium text-gray-900"
                          >Embarazo</label
                        >
                      </div>
                    </div>
                    <div class="flex items-start">
                      <div class="flex items-center h-5">
                        <input
                          id="candidates"
                          name="candidates"
                          type="checkbox"
                          class="focus:ring-indigo-500 h-4 w-4 text-indigo-600 border-gray-300 rounded"
                        />
                      </div>
                      <div class="ml-3 text-sm">
                        <label
                          for="candidates"
                          class="font-medium text-gray-900"
                          >Lactancia</label
                        >
                      </div>
                    </div>
                    <div class="flex items-start">
                      <div class="flex items-center h-5">
                        <input
                          id="offers"
                          name="offers"
                          type="checkbox"
                          class="focus:ring-indigo-500 h-4 w-4 text-indigo-600 border-gray-300 rounded"
                        />
                      </div>
                      <div class="ml-3 text-sm">
                        <label for="offers" class="font-medium text-gray-900"
                          >Menopaucia o pre-menopaucia</label
                        >
                      </div>
                    </div>
                  </div>
                </fieldset>
              </div>
              <div class="px-4 py-3 bg-gray-50 text-right sm:px-6">
                <button
                  type="submit"
                  class="inline-flex justify-center py-2 px-4 border border-transparent shadow-sm text-sm font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
                >
                  Enviar
                </button>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>

    <div class="mt-10 sm:mt-0"></div>
  </div>
</template>

<style>
.form-container {
  padding: 0 13%;
}
</style>
