<script setup lang="ts">
const { data: page } = await useAsyncData('index', () => queryContent('/').findOne())

useSeoMeta({
  title: page.value.title,
  ogTitle: page.value.title,
  description: page.value.description,
  ogDescription: page.value.description
})

const pages: number = ref(1)
const items = ref(Array(55))
</script>

<template>
  <div>
    <ULandingHero
      :title="page.hero.title"
      :description="page.hero.description"
    />
    <ULandingSection :title="page.blogs.title">
      <UPageGrid
        id="features"
        class="grid grid-cols-1 md:grid-cols-1 lg:grid-cols-2 xl:grid-cols-2 gap-6"
      >
        <!-- Card structure similar to the UI in the image -->
        <ULandingCard class="flex">
          <!-- Image Section -->
          <div class="flex flex-col md:flex-row lg:flex-col ">
            <div class="flex-shrink-0">
              <img
                src="https://img.freepik.com/free-photo/abstract-autumn-beauty-multi-colored-leaf-vein-pattern-generated-by-ai_188544-9871.jpg?size=626&ext=jpg&ga=GA1.1.2008272138.1726531200&semt=ais_hybrid"
                alt="Blog Image"
                class=" w-full md:w-48 lg:w-full h-60 lg:h-60 md:h-full object-cover"
              >
            </div>

            <!-- Content Section -->
            <div class="flex flex-col justify-between p-4">
              <!-- Date Section -->
              <div class="text-blue-500 text-sm mb-2">
                Sunday, 1 Jan 2023
              </div>

              <!-- Title -->
              <h2 class="text-lg font-semibold text-white mb-2">
                Migrating to Linear 101
              </h2>

              <!-- Description -->
              <p class="text-gray-400 text-sm mb-4">
                Linear helps streamline software projects, sprints, tasks, and bug tracking. Here's how to get...
              </p>

              <!-- Tags Section -->
              <div class="flex space-x-2">
                <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded-full text-xs">Design</span>
                <span class="bg-pink-100 text-pink-800 px-2 py-1 rounded-full text-xs">Research</span>
              </div>
            </div>
          </div>
        </ULandingCard>
        <div class="flex flex-col gap-6">
          <ULandingCard class="flex">
            <!-- Image Section -->
            <div class="flex flex-col md:flex-row ">
              <div class="flex-shrink-0">
                <img
                  src="https://img.freepik.com/free-photo/abstract-autumn-beauty-multi-colored-leaf-vein-pattern-generated-by-ai_188544-9871.jpg?size=626&ext=jpg&ga=GA1.1.2008272138.1726531200&semt=ais_hybrid"
                  alt="Blog Image"
                  class=" w-full md:w-48 md:h-full h-60 object-cover"
                >
              </div>

              <!-- Content Section -->
              <div class="flex flex-col justify-between p-4">
                <!-- Date Section -->
                <div class="text-blue-500 text-sm mb-2">
                  Sunday, 1 Jan 2023
                </div>

                <!-- Title -->
                <h2 class="text-lg font-semibold text-white mb-2">
                  Migrating to Linear 101
                </h2>

                <!-- Description -->
                <p class="text-gray-400 text-sm mb-4">
                  Linear helps streamline software projects, sprints, tasks, and bug tracking. Here's how to get...
                </p>

                <!-- Tags Section -->
                <div class="flex space-x-2">
                  <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded-full text-xs">Design</span>
                  <span class="bg-pink-100 text-pink-800 px-2 py-1 rounded-full text-xs">Research</span>
                </div>
              </div>
            </div>
          </ULandingCard>
          <ULandingCard class="flex">
            <!-- Image Section -->
            <div class="flex flex-col md:flex-row ">
              <div class="flex-shrink-0">
                <img
                  src="https://img.freepik.com/free-photo/abstract-autumn-beauty-multi-colored-leaf-vein-pattern-generated-by-ai_188544-9871.jpg?size=626&ext=jpg&ga=GA1.1.2008272138.1726531200&semt=ais_hybrid"
                  alt="Blog Image"
                  class=" w-full md:w-48 md:h-full h-60 object-cover"
                >
              </div>

              <!-- Content Section -->
              <div class="flex flex-col justify-between p-4">
                <!-- Date Section -->
                <div class="text-blue-500 text-sm mb-2">
                  Sunday, 1 Jan 2023
                </div>

                <!-- Title -->
                <h2 class="text-lg font-semibold text-white mb-2">
                  Migrating to Linear 101
                </h2>

                <!-- Description -->
                <p class="text-gray-400 text-sm mb-4">
                  Linear helps streamline software projects, sprints, tasks, and bug tracking. Here's how to get...
                </p>

                <!-- Tags Section -->
                <div class="flex space-x-2">
                  <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded-full text-xs">Design</span>
                  <span class="bg-pink-100 text-pink-800 px-2 py-1 rounded-full text-xs">Research</span>
                </div>
              </div>
            </div>
          </ULandingCard>
        </div>
        <ULandingCard class="flex">
          <!-- Image Section -->
          <div class="flex flex-col md:flex-row ">
            <div class="flex-shrink-0">
              <img
                src="https://img.freepik.com/free-photo/abstract-autumn-beauty-multi-colored-leaf-vein-pattern-generated-by-ai_188544-9871.jpg?size=626&ext=jpg&ga=GA1.1.2008272138.1726531200&semt=ais_hybrid"
                alt="Blog Image"
                class=" w-full md:w-48 md:h-full h-60 object-cover"
              >
            </div>

            <!-- Content Section -->
            <div class="flex flex-col justify-between p-4">
              <!-- Date Section -->
              <div class="text-blue-500 text-sm mb-2">
                Sunday, 1 Jan 2023
              </div>

              <!-- Title -->
              <h2 class="text-lg font-semibold text-white mb-2">
                Migrating to Linear 101
              </h2>

              <!-- Description -->
              <p class="text-gray-400 text-sm mb-4">
                Linear helps streamline software projects, sprints, tasks, and bug tracking. Here's how to get...
              </p>

              <!-- Tags Section -->
              <div class="flex space-x-2">
                <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded-full text-xs">Design</span>
                <span class="bg-pink-100 text-pink-800 px-2 py-1 rounded-full text-xs">Research</span>
              </div>
            </div>
          </div>
        </ULandingCard>
        <ULandingCard class="flex">
          <!-- Image Section -->
          <div class="flex flex-col md:flex-row ">
            <div class="flex-shrink-0">
              <img
                src="https://img.freepik.com/free-photo/abstract-autumn-beauty-multi-colored-leaf-vein-pattern-generated-by-ai_188544-9871.jpg?size=626&ext=jpg&ga=GA1.1.2008272138.1726531200&semt=ais_hybrid"
                alt="Blog Image"
                class=" w-full md:w-48 md:h-full h-60 object-cover"
              >
            </div>

            <!-- Content Section -->
            <div class="flex flex-col justify-between p-4">
              <!-- Date Section -->
              <div class="text-blue-500 text-sm mb-2">
                Sunday, 1 Jan 2023
              </div>

              <!-- Title -->
              <h2 class="text-lg font-semibold text-white mb-2">
                Migrating to Linear 101
              </h2>

              <!-- Description -->
              <p class="text-gray-400 text-sm mb-4">
                Linear helps streamline software projects, sprints, tasks, and bug tracking. Here's how to get...
              </p>

              <!-- Tags Section -->
              <div class="flex space-x-2">
                <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded-full text-xs">Design</span>
                <span class="bg-pink-100 text-pink-800 px-2 py-1 rounded-full text-xs">Research</span>
              </div>
            </div>
          </div>
        </ULandingCard>
      </UPageGrid>
    </ULandingSection>

    <ULandingSection :title="page.posts.title">
      <UPageGrid
        id="features"
        class="grid grid-cols-1 md:grid-cols-1 lg:grid-cols-3 xl:grid-cols-3 gap-6"
      >
        <!-- Card structure similar to the UI in the image -->
        <ULandingCard
          v-for="index in 6"
          :key="index"
          class="flex"
        >
          <!-- Image Section -->
          <div class="flex flex-col md:flex-row lg:flex-col ">
            <div class="flex-shrink-0">
              <img
                src="https://img.freepik.com/free-photo/abstract-autumn-beauty-multi-colored-leaf-vein-pattern-generated-by-ai_188544-9871.jpg?size=626&ext=jpg&ga=GA1.1.2008272138.1726531200&semt=ais_hybrid"
                alt="Blog Image"
                class=" w-full md:w-48 lg:w-full h-60 lg:h-60 md:h-full object-cover"
              >
            </div>

            <!-- Content Section -->
            <div class="flex flex-col justify-between p-4">
              <!-- Date Section -->
              <div class="text-blue-500 text-sm mb-2">
                Sunday, 1 Jan 2023
              </div>

              <!-- Title -->
              <h2 class="text-lg font-semibold text-white mb-2">
                Migrating to Linear 101
              </h2>

              <!-- Description -->
              <p class="text-gray-400 text-sm mb-4">
                Linear helps streamline software projects, sprints, tasks, and bug tracking. Here's how to get...
              </p>

              <!-- Tags Section -->
              <div class="flex space-x-2">
                <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded-full text-xs">Design</span>
                <span class="bg-pink-100 text-pink-800 px-2 py-1 rounded-full text-xs">Research</span>
              </div>
            </div>
          </div>
        </ULandingCard>
      </UPageGrid>
      <UPagination
        v-model="pages"
        :total="items.length"
        :ui="{ rounded: 'first-of-type:rounded-s-md last-of-type:rounded-e-md' }"
        class=" mx-auto"
      >
        <template #prev="{ onClick }">
          <UTooltip text="Previous page">
            <UButton
              icon="i-heroicons-arrow-small-left-20-solid"
              color="primary"
              :ui="{ rounded: 'rounded-full' }"
              class="rtl:[&_span:first-child]:rotate-180 me-2"
              @click="onClick"
            />
          </UTooltip>
        </template>

        <template #next="{ onClick }">
          <UTooltip text="Next page">
            <UButton
              icon="i-heroicons-arrow-small-right-20-solid"
              color="primary"
              :ui="{ rounded: 'rounded-full' }"
              class="rtl:[&_span:last-child]:rotate-180 ms-2"
              @click="onClick"
            />
          </UTooltip>
        </template>
      </UPagination>
    </ULandingSection>

    <!-- <ULandingSection
      :title="page.features.title"
      :description="page.features.description"
      :headline="page.features.headline"
    >
      <UPageGrid
        id="features"
        class="scroll-mt-[calc(var(--header-height)+140px+128px+96px)]"
      >
        <ULandingCard
          v-for="(item, index) in page.features.items"
          :key="index"
          v-bind="item"
        />
      </UPageGrid>
    </ULandingSection> -->

    <!-- <ULandingSection
      :title="page.pricing.title"
      :description="page.pricing.description"
      :headline="page.pricing.headline"
    >
      <UPricingGrid
        id="pricing"
        compact
        class="scroll-mt-[calc(var(--header-height)+140px+128px+96px)]"
      >
        <UPricingCard
          v-for="(plan, index) in page.pricing.plans"
          :key="index"
          v-bind="plan"
        />
      </UPricingGrid>
    </ULandingSection> -->

    <!-- <ULandingSection
      :headline="page.testimonials.headline"
      :title="page.testimonials.title"
      :description="page.testimonials.description"
    >
      <UPageColumns
        id="testimonials"
        class="xl:columns-4 scroll-mt-[calc(var(--header-height)+140px+128px+96px)]"
      >
        <div
          v-for="(testimonial, index) in page.testimonials.items"
          :key="index"
          class="break-inside-avoid"
        >
          <ULandingTestimonial v-bind="testimonial" />
        </div>
      </UPageColumns>
    </ULandingSection> -->

    <!-- <ULandingSection class="bg-primary-50 dark:bg-primary-400 dark:bg-opacity-10">
      <ULandingCTA
        v-bind="page.cta"
        :card="false"
      />
    </ULandingSection> -->

    <!-- <ULandingSection
      id="faq"
      :title="page.faq.title"
      :description="page.faq.description"
      class="scroll-mt-[var(--header-height)]"
    >
      <ULandingFAQ
        multiple
        :items="page.faq.items"
        :ui="{
          button: {
            label: 'font-semibold',
            trailingIcon: {
              base: 'w-6 h-6'
            }
          }
        }"
        class="max-w-4xl mx-auto"
      />
    </ULandingSection> -->
  </div>
</template>
