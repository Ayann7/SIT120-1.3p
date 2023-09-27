<template>
    <div class="skills-container">
      <h2 class="skills-title">My Skills!</h2>
      <ul class="skills-list">
        <li class="skills-item">HTML</li>
        <li class="skills-item">CSS</li>
        <li class="skills-item">JavaScript</li>
        <li class="skills-item">Vue.js</li>
        <li class="skills-item">React.js</li>
        <li class="skills-item">C++</li>
        <li class="skills-item">API Integration</li>
      </ul>
    </div>
  </template>

<style scoped>
.skills-section {
  margin-top: 20px;
}

.skills-section h2 {
  font-size: 24px;
  color: #333;
}

.skills-section ul {
  list-style: none;
  padding: 0;
}

.skills-section li {
  font-size: 18px;
  color: #666;
  margin-bottom: 10px;
}
.skills-container {
  background-color: #f5f5f5;
  padding: 20px;
  margin-top: 20px;
}

.skills-title {
  font-size: 24px;
  color: #333;
  margin-bottom: 20px;
}

.skills-list {
  list-style: none;
  padding: 0;
}

.skills-item {
  font-size: 18px;
  color: #666;
  margin-bottom: 10px;
}

.skills-item:hover {
  color: #007BFF;
  cursor: pointer;
  transition: color 0.3s ease;
}
</style>



<script>
export default {
  name: 'SkillsComponent'
}
</script>