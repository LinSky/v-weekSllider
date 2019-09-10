<template>
    <div>
        <week-slider
			@dateClick="dateClickhandler"
      todayTxtColor='#ff0000'
			:showYear="true"
			:defaultDate.sync="default_date" :startdate="startdate" :enddate="enddate">
		</week-slider>
    </div>
</template>

<script>
export default {
    name: 'app',

    data () {
        return {
            default_date: '2019-08-12',
            startdate: '2019-07-25',
            enddate: '2019-09-05'
        }
    },
    methods: {
        dateClickhandler (date) {
            console.log(date);
        }
    }
}
</script>

<style scoped>

</style>
