<template>
  <footer class="footer">
    <div
      class="container grid h-full grid-flow-row-dense gap-8 md:grid-flow-col auto-cols-max"
    >
      <div class="flex items-start space-x-2">
        <TelegramIcon class="w-4 h-auto" />
        <div class="flex flex-col text-sm leading-none">
          <span class="mb-1">Telegram</span>
          <a href="https://t.me/ez_cash_gg" target="_blank">
            <strong>@patachapaa</strong>
          </a>
        </div>
      </div>
      <div class="flex items-start space-x-2">
        <VkIcon class="w-4 h-auto" />
        <div class="flex flex-col text-sm leading-none">
          <span class="mb-1">Call</span>
          <a href="https://vk.com/ezcash_official" target="_blank">
            <strong>0720 123 456</strong>
          </a>
        </div>
      </div>
      <div class="flex items-start space-x-2">
        <EmailIcon class="w-4 h-auto" />
        <div class="flex flex-col text-sm leading-none">
          <span class="mb-1">Email</span>
          <a href="mailto:help@ezcash.gg" target="_blank">
            <strong>help@patachapaa.com</strong>
          </a>
        </div>
      </div>
      <div class="flex flex-col space-y-1 leading-none">
        <a href="#" class="font-semibold">Terms of use</a>
        <a href="#" class="font-semibold">Privacy Policy</a>
        <nuxt-link :to="{ name: 'help' }" class="font-semibold">Help</nuxt-link>
      </div>
    </div>
  </footer>
</template>

<script>
import TelegramIcon from '@/static/img/icon/social/telegram.svg?inline'
import VkIcon from '@/static/img/icon/social/vk.svg?inline'
import EmailIcon from '@/static/img/icon/email.svg?inline'

export default {
  components: { TelegramIcon, VkIcon, EmailIcon },
}
</script>

<style lang="scss">
.footer {
  @apply border-t-1 border-secondary py-5;
}
</style>
