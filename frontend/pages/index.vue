<template>
  <div>
    <ul>
      <li v-for="job in jobs" :key="job.id">{{ jobTitle(job) }}</li>
    </ul>
  </div>
</template>

<script lang="ts">
import "vue-apollo";
import { Vue, Component } from 'vue-property-decorator'
import JobsGQL from '~/apollo/queries/jobs.graphql'
import { Job } from "~/apollo/types/gql-types"

@Component({
  apollo: {
    jobs: {
      query: JobsGQL,
    },
  },
})
export default class Index extends Vue {
  jobTitle(job: Job): string {
    return `${job.id} - ${job.title}`
  }
}
</script>

<style>
</style>
