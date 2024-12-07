<template>
  <article>
    <section>
      <PagePreview
        is-text-right
        :value="{ title: 'Nikita Chepik', description: 'Fullstack developer' }"
      />
    </section>
    <section>
      <HomeInfo :value="{ title: 'Информация', description: 'На сайте разместил информацию о себе и своих работах. Цель - показать портфолио веб-разработчика. В прошлом инженер в области информационно-аналитических систем, который нашел свое предназначение в мире IT. Получаю огромное удовольствие от своей работы.' }" />
    </section>
    <section>
      <HomeInfo
        is-img-right
        :value="{ title: 'Моя страсть - это создание веб-приложений', description: `Уже более 5 лет занимаюсь созданием приложений для МО. (Расписать больше)` }"
      />
    </section>
    <section>
      <HomeWorks :value="{ value: 'Проекты', description: 'Представляю вам несколько последних проектов, над которыми я работал' }" />
    </section>
  </article>
</template>

<script setup lang="ts">

</script>

<style lang="scss" scoped></style>