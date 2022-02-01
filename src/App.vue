<script setup>
const courses = [
    { courseId: 'INT201', courseName: 'Client I', credit: 2 },
    { courseId: 'INT202', courseName: 'Client II', credit: 2 },
    { courseId: 'INT210', courseName: 'Architecture and Deployment', credit: 3 }
]
</script>

<template>
    <ul>
        <li
            v-for="(course, index) in courses "
            :key="index"
        >{{ course.courseId }} : {{ course.credit }}</li>
    </ul>
</template>

<style></style>
 




 