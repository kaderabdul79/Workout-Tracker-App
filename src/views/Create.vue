<template>
    <div class="max-w-screen-md mx-auto px-4 py-10">
      
      <!-- Create -->
      <div class="p-8 flex items-start bg-light-grey rounded-md shadow-lg">
        <!-- Form -->
        <form class="flex flex-col gap-y-5 w-full">
          <h1 class="text-2xl text-at-light-green">Record Workout</h1>
  
          <!-- Workout Name -->
          <div class="flex flex-col">
            <label for="workout-name" class="mb-1 text-sm text-at-light-green"
              >Workout Name</label
            >
            <input
              type="text"
              required
              class="p-2 text-gray-500 focus:outline-none"
              id="workout-name"
              v-model="workoutName"
            />
          </div>
  
          <!-- Workout Type -->
          <div class="flex flex-col">
            <label for="workout-type" class="mb-1 text-sm text-at-light-green"
              >Workout Type</label
            >
            <select
              id="workout-type"
              class="p-2 text-gray-500 focus:outline-none"
              required
              v-model="workoutType"
            >
              <option value="select-workout">Select Workout</option>
              <option value="strength">Strength Training</option>
              <option value="cardio">Cardio</option>
            </select>
          </div>
  
          <button
            type="submit"
            class="mt-6 py-2 px-6 rounded-sm self-start text-sm
        text-white bg-at-light-green duration-200 border-solid
        border-2 border-transparent hover:border-at-light-green hover:bg-white
        hover:text-at-light-green"
          >
            Record Workout
          </button>
        </form>
      </div>
    </div>
  </template>
  
  <script>
import { ref } from 'vue';

  export default {
    name: "create",
    setup() {
    // Create data
    const workoutName = ref("");
    const workoutType = ref("select-workout");
    const exercises = ref([]);
    const statusMsg = ref(null);
    const errorMsg = ref(null);


    return {
      workoutName,
      workoutType,
      exercises,
      statusMsg,
      errorMsg,};
    },
  };
  </script>
  