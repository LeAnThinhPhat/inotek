<template>
    <div class="job-list">
        <p>Order by: {{order}}</p>
        <ul>
            <li v-for="job in orderedJobs" :key="job.id">
                <h2>{{job.title}}</h2>
                <p>Salary: {{job.salary}}</p>
                <p>Location: {{job.location}}</p>
            </li>
        </ul>
    </div>
</template>
<script lang="ts">
import OrderTerm from '@/types/OrderTerm'
import { computed, defineComponent, PropType} from 'vue'
import Job from '../types/Job'
export default defineComponent({
    props: {
        jobs: {
            required: true,
            type: Array as PropType<Job[]>
        },
        order: {
            required: true,
            type: String as PropType<OrderTerm>
        },
    },
    setup(props){
        const orderedJobs = computed(()=>{
            return [...props.jobs].sort((a:Job,b:Job)=>{
                return a[props.order] > b[props.order] ? 1 : -1
            });
        })
        return {orderedJobs}
    }
})
</script>
<style scoped lang="scss">
    .job-list {
        max-width: 60%;
        margin: 40px auto;
        ul{
         padding: 0;
        }
        li {
            text-align: center;
            background: burlywood;
            border-radius: 4px;
            list-style-type: none;
            margin: 10px;
            padding: 10px;  
        }
    }
</style>
