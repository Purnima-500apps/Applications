<template>
  <div>
    <h1 class="mt-3 mb-3">Create Application</h1>
  <div class="mb-6">
    <label
      for="large-input"
      class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
      >Enter candidate id</label
    >
    <input
      placeholder=" Candidate ID"
      v-model="candidate_id"
      type="text"
      id="large-input"
      class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 sm:text-md focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
    />
  </div>
  <div class="mb-6">
    <label
      for="base-input"
      class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
      >Enter Job posting id</label
    >
    <input
      placeholder="Job Posting ID"
      v-model="job_id"
      type="text"
      id="base-input"
      class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
    />
  </div>
  <div>
    <label
      for="small-input"
      class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
      >Status</label
    >
    <input
      placeholder="Status"
      v-model="status"
      type="text"
      
      id="small-input"
      class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 sm:text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
    />
  </div>
  <div>
    <label
      for="small-input"
      class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
      >Resume URL</label
    >
    <input
      placeholder="Enter resume url"
      v-model="resume_url"
      type="text"
      
      id="small-input"
      class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 sm:text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
    />
  </div>
  <div>
    <label
      for="small-input"
      class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
      >Cover URL</label
    >
    <input
      placeholder="Enter cover url"
      v-model="cover_letter_url"
      type="text"
      id="small-input"
      class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 sm:text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
    />
  </div>

  <div class="mt-5">
      
    <button @click="save" type="button" class="text-white bg-blue-700 hover:bg-blue-800 focus:outline-none focus:ring-4 focus:ring-blue-300 font-medium rounded-full text-sm px-5 py-2.5 text-center mr-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Save</button>
    <button type="button" class="text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-full text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Cancel</button>

    </div>
  </div>    
</template>

<script setup>
 
const candidate_id = ref("");
const job_id = ref("");
const status = ref("");
const resume_url = ref("");
const cover_letter_url = ref("");

const save = () =>{
  
}

</script>
