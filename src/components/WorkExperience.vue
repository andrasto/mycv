<template>
    <div>
        <h2>Working Experience</h2>
        <section class="indent">
            <b><p>Nokia Solutions and Networks Kft.</p></b>
            <section class="indent" 
                     v-for="(job, index) in jobs" 
                     :key="index">
                <app-jobs :job="job"></app-jobs>
            </section>
        </section>
    </div>
</template>

<script>
import appJobs from './Jobs.vue'

export default {
    data() {
        return {
            jobs: [
                {
                    title: "Software Development Engineer",
                    timePeriod: "Dec 2018 - ",
                    description: [
                        'Management and development of multiple tools while mentoring the trainees working on these projects',
                        'Programming Languages used: Python, C#, NodeJS, HTML5, CSS3 and jQuery',
                        'Scrum Master on one of the projects and acting as Technical Lead for all of them',
                        'Going for Professional Scrum Master 1 Certificate'
                    ]
                },
                {
                    title: "Full-Stack Developer",
                    timePeriod: "Sep 2017 - Dec 2018",
                    description: [
                        'Marketing page of Nokia Digital Automation Cloud (<a href="https://dac.nokia.com">dac.nokia.com</a>) using Magento2, HTML5, CSS3 and jQuery',
                        'Web UI for indoor positioning tool using Angular2 and NodeJS'
                    ]
                },
                {
                    title: "Software Engineer Trainee",
                    timePeriod: "Sep 2016 - Sep 2017",
                    description: [
                        'Web app for displaying internal tool database using Django, MySQL, HTML5, CSS3 and JS,working with an international team using SCRUM',
                        'Web app for displaying the org tree of the selected organization in a PowerPoint presentation using Flask, HTML5, CSS3, JS and jQuery. After the 6-month development, I received an offer to stay at the company, as a full-time employee'
                    ]
                }
            ]
        }
    },
    components: {
        appJobs
    }
}
</script>

<style scoped>
    p {
        margin: 0.75rem 0;
    }
</style>