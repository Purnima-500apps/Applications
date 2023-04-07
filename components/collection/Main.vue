<template>
  <div>
    <div class="m-3" v-if="showNodal">
      <CollectionAdd />
    </div>
    <div class="mt-4 sm:ml-16 sm:mt-0 sm:flex-none flex justify-end">
      <button
        type="button"
        class="block rounded-md bg-indigo-600 px-3 py-2 text-center text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
        @click="showCreateModal"
        v-if="!showNodal"
      >
        Add
      </button>
    </div>
    <div class="m-3" v-if="!showNodal">
        <CollectionList  :applicationData="applicationData"/>
    </div>
  </div>
  
</template>

<script setup>
  import {ref } from 'vue'
  
  const showNodal = ref(false);

  
  const showCreateModal = () => {
    showNodal.value = true;
  };

const getData = await useAuthLazyFetch("https://v7-stark-db-orm.mercury.infinity-api.net/api/applications/",);

console.log("*****jhju",getData)
 const applicationData = getData.data._rawValue
 console.log("applicationData----?",applicationData)

</script>
