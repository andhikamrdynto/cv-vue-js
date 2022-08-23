<script setup>
  import WelcomeItem from './WelcomeItem.vue'
  import DocumentationIcon from './icons/IconDocumentation.vue'
  import ToolingIcon from './icons/IconTooling.vue'
  import EcosystemIcon from './icons/IconEcosystem.vue'
  import CommunityIcon from './icons/IconCommunity.vue'
  import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>HTML</template>
    <div class="progress">
      <div class="progress-bar" role="progressbar" aria-label="Example with label" style="width: 90%;"
        aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">90%</div>
    </div>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>CSS</template>
    <div class="progress">
      <div class="progress-bar" role="progressbar" aria-label="Example with label" style="width: 80%;"
        aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">80%</div>
    </div>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>JavaScript</template>
    <div class="progress">
      <div class="progress-bar" role="progressbar" aria-label="Example with label" style="width: 30%;"
        aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">30%</div>
    </div>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Bootstrap</template>
    <div class="progress">
      <div class="progress-bar" role="progressbar" aria-label="Example with label" style="width: 90%;"
        aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">90%</div>
    </div>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Laravel</template>

    <div class="progress">
      <div class="progress-bar" role="progressbar" aria-label="Example with label" style="width: 50%;"
        aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">50%</div>
    </div>
  </WelcomeItem>
</template>