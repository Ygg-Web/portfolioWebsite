<template>
  <article>
    <section class="font-custom">
      <div class="relative isolate h-[100vh] overflow-hidden bg-gray-900 py-24 sm:py-32 flex items-center">
        <img alt=""
          src="https://images.unsplash.com/photo-1521737604893-d14cc237f11d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&crop=focalpoint&fp-y=.8&w=2830&h=1500&q=80&blend=111827&sat=-100&exp=15&blend-mode=multiply"
          class="absolute inset-0 -z-10 size-full object-cover object-right md:object-center">
        <div class="mx-auto px-6 lg:px-8">
          <div class="mx-auto max-w-2xl lg:mx-0">
            <p class="text-5xl text-center font-semibold text-white sm:text-7xl lg:text-8xl">Nikita Chepik
            </p>
            <p class="text-2xl text-end sm:text-4xl lg:text-5xl">Fullstack developer</p>
          </div>
        </div>
      </div>
    </section>
    <section>
      <div class="px-6 py-12 sm:px-12 lg:px-16 h-[100vh] overflow-hidden">
        <div class="grid lg:grid-flow-col gap-10 mx-auto">
          <div class="lg:w-[400px] lg:h-[800px] bg-slate-600">
            Изображение
          </div>
          <div>
            <div class="py-2 text-xl sm:text-2xl lg:text-3xl">
              Информация
            </div>
            <div class="text-base sm:text-lg lg:text-xl">
              <p>
                На сайте разместил информацию о себе и своих работах. Цель - показать портфолио веб-разработчика.
                В прошлом инженер в области информационно-аналитических систем, который нашел свое предназначение в мире
                IT.
                Получаю огромное удовольствие от своей работы. <NuxtLink to="/about" class="text-[#B8B799]">Узнать
                  больше</NuxtLink>
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section>
      <div class="px-6 py-12 sm:px-12 lg:px-16 h-[100vh] overflow-hidden">
        <div class="grid lg:grid-flow-col lg:gap-10 mx-auto">
          <div class="lg:w-[400px] lg:h-[800px] bg-slate-600 lg:order-last">
            Изображение
          </div>
          <div>
            <div class="py-2 text-xl sm:text-2xl lg:text-3xl">
              Моя страсть - это создание веб-приложений
            </div>
            <div class="text-base sm:text-lg lg:text-xl">
              <p>
                Уже более 5 лет занимаюсь созданием приложений для МО. (Расписать больше) <NuxtLink to="/about"
                  class="text-[#B8B799]">Узнать больше</NuxtLink>
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section>
      <div class="px-6 py-12 sm:px-12 lg:px-16 mx-auto">
        <div>
          <div class="text-center py-2 text-xl sm:text-2xl lg:text-3xl">Проекты</div>
          <div class="text-base sm:text-lg lg:text-xl">
            <p>
              Представляю вам несколько последних проектов, над которыми я работал <NuxtLink to="/projects"
                class="text-[#B8B799]">Узнать больше</NuxtLink>
            </p>
          </div>
        </div>
      </div>
    </section>
  </article>
</template>

<script setup lang="ts">

</script>

<style lang="scss" scoped></style>