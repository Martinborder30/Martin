<div id="app">
    <h1>Treningsprogram</h1>
    <div class="exercise-list">
      <h2>Øvelser</h2>
      <ul>
        <li v-for="exercise in exercises" :key="exercise.id">
          {{ exercise.name }} ({{ exercise.duration }} sekunder)
        </li>
      </ul>
    </div>
    <div class="controls">
      <button @click="startWorkout" :disabled="isWorkoutRunning">Start treningsøkt</button>
      <button @click="stopWorkout" :disabled="!isWorkoutRunning">Stopp treningsøkt</button>
    </div>
  </div>

<script>
    const exercises = [
  { id: 1, name: "Knebøy", duration: 30 },
  { id: 2, name: "Push-ups", duration: 30 },
  { id: 3, name: "Sit-ups", duration: 30 }
];

const app = new App({
  target: document.getElementById("app"),
  data: {
    exercises,
    isWorkoutRunning: false,
    intervalId: null
  },
  methods: {
    startWorkout() {
      this.set({ isWorkoutRunning: true });
      const startTime = new Date().getTime();
      let totalTime = 0;
      let currentExerciseIndex = 0;
      const tick = () => {
        const currentTime = new Date().getTime();
        const elapsedTime = currentTime - startTime;
        totalTime += elapsedTime;
        if (totalTime >= exercises[currentExerciseIndex].duration * 1000) {
          currentExerciseIndex++;
          totalTime = 0;
        }
        if (currentExerciseIndex >= exercises.length) {
          clearInterval(this.get("intervalId"));
          this.set({ isWorkoutRunning: false });
        }
      };
      const intervalId = setInterval(tick, 100);
      this.set({ intervalId });
    },
    stopWorkout() {
      clearInterval(this.get("intervalId"));
      this.set({ isWorkoutRunning: false });
    }
  }
});

</script>

<style>

#app {
  max-width: 600px;
  margin: 0 auto;
  text-align: center;
}

.exercise-list {
  margin-bottom: 20px;
}

.controls button {
  margin: 0 10px;
  padding: 10px;
  font-size: 16px;
  cursor: pointer;
  border: none;
  background-color: #4CAF50;
  color: white;
  border-radius: 4px;
}

.controls button:disabled {
  background-color: #ccc;
  cursor: not-allowed;
}

</style>